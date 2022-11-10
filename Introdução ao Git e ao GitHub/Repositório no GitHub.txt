# Passo a passo para a criação, atualização e sincronização de um Repositório no GitHub

É possível criar um repositório no GitHub para armazenar e colaborar nos arquivos de projetos. O repositório pode ser criado com propriedade individual ou compartilhada com outras pessoas em uma organização.Também é possível restringir quem tem acesso a um repositório escolhendo a visibilidade do mesmo. Você pode usar repositórios para gerenciar seu trabalho ou ainda você pode trabalhar com colaboradores ilimitados em repositórios públicos ilimitados, com um conjunto completo de recursos. 

## Criando um novo Repositório:

1.Para criar um novo Repositório no GitHub você pode acessar o link https://github.com/new (acessível pelo site através do botão "+", depois "Novo repositório"). 

2.No menu suspenso Proprietário, selecione a conta na qual deseja criar o repositório.

	2.1.Digite um nome para o seu repositório e uma descrição opcional;
	2.2.Escolha uma visibilidade do repositório (recomenda-se deixar público);
	2.3.Você pode criar um README, que é um documento que descreve seu projeto.

3.Clique em Criar repositório.

4.Alternativamente, também é comum utilizar o conceito de "fork" em um projeto base disponibilidado pelo expert (esta funcionalidade encontra-se no canto superior direito da página do repositório no GitHub). 

	4.1.Tecnicamente, um "fork" cria uma cópia exata do projeto em seu GitHub, mantendo assim uma referência direta ao código original, o que é muito útil para projeto com uma base sólida a ser seguida.


## Atualizando um Repositório:

1.Abra o Git Bash ou terminal na pasta onde está o seu projeto.

2.Todos os arquivos adicionados ou alterados e salvos devem ser validados como upload através do comando git add .

	2.1.Para selecionarmos todas as alterações feitas em ambiente local, usamos: git add .
	2.2.Para adicionarmos apenas um arquivo específico, usamos: git add ./nome do arquivo
	2.3.E para selecionar todos os arquivos numa pasta específica, usamos: git add ./nome da pasta/*

3.Incorpore as mudanças do seu projeto remoto com seu projeto local usando git pull origin master

	3.1.Você pode checar quais foram as alterações no arquivo ou código através do comando git status.

4.Confirme as alterações entre o projeto remoto e o projeto local usando o comando git commit -m "descrição do commit"

5.Depois de fazermos nossos commits (pacotes de atualizações locais), precisamos subir esses pacotes para que outros possam acessar essas atualizações também. Fazemos isso através do git push.

	5.1 O terminal irá pedir o seu login e senha do GitHub para realizar esse processo e você terá seu projeto atualizado.


## Sincronizando um Repositório:

Uma vez feito o push dos commits para o seu projeto em GitHub, você poderá manter o seu repositório local sincronizado com seu repositório remoto enquanto faz alterações em qualquer um deles. No Git, o termo remoto descreve o servidor em que o seu código está armazenado. No seu caso, esse servidor é um repositório no GitHub.


###Sobre a sincronização do branch

Você pode sincronizar o seu branch local com o repositório remoto, puxando quaisquer commits adicionados ao branch no GitHub desde a última vez que você sincronizou. Se você fizer commits de outro dispositivo ou se várias pessoas contribuem para um projeto, você precisará sincronizar seu branch local para mantê-lo atualizado.

Quando você puxa para o branch local, você só atualiza sua cópia local do repositório. Para atualizar o seu branch em GitHub, você deve fazer push das suas alterações.


###Sobre o envio de alterações para GitHub

Quando você faz push das alterações, você envia as alterações confirmadas em seu repositório local para o repositório remoto no GitHub. Se você alterar seu projeto localmente e desejar que outras pessoas tenham acesso às alterações, você deve fazer push das alterações para GitHub.

Antes de fazer push das alterações, você deve atualizar seu branch local para incluir quaisquer commits adicionados ao repositório remoto. Se alguém fez commits no controle remoto que não estão em seu branch local, GitHub Desktop solicitará que você bosque os novos commits antes de fazer push de suas alterações para evitar conflitos de merge. 

