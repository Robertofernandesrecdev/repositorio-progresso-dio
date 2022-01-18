# Prodemos usar o gitbash, cmd ou terimnal do editor vscode!
### Auto-Open Markdown-Preview -> extensão para visualizar como está ficando no vscode o README.md obs: se certificar que vc etá dentro da pasta do projeto desejado!

<u>git init</u> - para iniciar um repositório, dentro da pasta selcionada do projeto onde voce quer salvar!

<u>git status</u> - verificar o status do repositório!

<u>git add  nome do arquivo</u> - adiciona só o arquivo desejado a ficar monitorado! Ex. git add curriculo.txt

<u>git add .</u> - adiciona todos os arquivos para o repoitório para ser monitorado e  para ficar disponivel para commitar! os arquivos não trackeados, começam a ser trackeados pelo git!

<u>git commit -m " nome do commit que vc quer dar"</u> - para comitar todos os arquivos que estão preparados. salvar as informações 

<u>git commit nome do arquivo -m " nome do commit que vc deseja"</u> - para commitar uma arquivo só específico!  Ex. git commit empresa.txt -m "criando o arquivo do nome da empresa"

<u>git branch -M main</u> - criar a branch main

<u>git remote add origin mais o link do repositótio criado no github</u> - para adicionar o link do repositório que vc vai fazer o push. Ex. git remote add origin http://github.com/repo

<u>git push -u origin main</u> - para subir o projeto para o repositório que voce criou! na branch principal. obs: na primeira vez, vai pedir o username e senha do github!

<u>git push</u> - para subir o repositório  

<u>git branch -a</u>  - vai listar todos os commits 

<u><u>git pull link do repositório</u> </u> - vai buscar do repositório e tras pra maquina, baixa e sicronizar os arquivos com nosso projeto ! 

**// Clonando Repositorios** 

<u>git clone mais url que eu quero clonar</u> ! Ex. git clone http://urldoclone 

<u>git clone mais url que eu quero clonar</u> ! Ex. git clone http://urldoclone .  obs: ao adicionar o ponto, clona os arquivos direto na pasta especificada.

<u>git log</u> - dar detalhadamente todos os detalhes commits e suas auterações do projeto! clicar q para sair! mostra todas as descrições que vc fez....



<u>git checkout nome do arquivo</u>  -  da  um rollback ou seja, volta para o estado anterior que vc deseja! volta a o status original. Ex. git checkout index.html

<u>.gitignore</u> -  é só colocar o nome do arquivo ou pasta dentro do arquivo .gitignore. - onde voce coloca os arquivos que vc não quer que sejam vistos no seu repositório do github, tipo arquivos .env, /node_modules, etc... 

<u>git reset --hard origin/main</u> - volta o status mais este muito cuidado que não tem volta! volta ao status do último commit.

**//Branches**

Branch - maneira de separar versões do projeto, gerenciar melhor o projeto! 

Quando criamos um novo projeto, ele inicia sempre na branch main!

<u>git branch</u> - ele vai mostrar todas as branches que tem no projeto.

<u>git branch nome da branch a ser criada</u> - para criar uma nova branch. obs: não pode ter espaços! Ex. git branch page_home

**//mudando para outra branch**

<u>git checkout page_home</u>  -  git checkout mais o nome da branch para mudar de branch! obs: antes de mudar de branch salve e commit todas as auterações!

<u>git checkout -b "home_home"</u> - cria uma nova branch e já trocar  pra ela! 

<u>git branch -d home_home</u> - para deletar uma branch que vc desejar. git branch -d mais o nome da branch!

**// unir branches** 

<u>git merge nome da branch que vc quer unir</u>! Ex. git merge home_home. obs: vc tem que estar na branch main. Após a junção vc pode dar um push... voce também pode estar em outra branch e dar ume merge na main, a depender da necessidade.

<u>git stash</u> - volta para o último estado inicial 

<u>git stash list</u> - lista as todas as stash criadas, salva pelo id entre chaves  { id}  

<u>git stash apply id</u> - muda para a stash que vc quer! Ex. git stash apply 0 , o numero da stash! 

<u>git stash show -p id</u> - para saber o que tem de mudança na stash! 

**// trabalhando com Tags**

<u>criar tag = git tag -a v1.0 -m "Primeira versão do sistema"</u> - cria uma tag e nomeia entre aspas. 

<u>git tag</u> - lista todas as tags criadas 

<u>git show v1.0</u> - git show mais nome da tag voce vê o que tem nela! Mostra todos os commits e alterações! 

<u>git checkout v1.0</u> - git checkout mais a versão da tag ele muda para a tag! 

**// enviando tag para o repo**

<u>git push origin v1.0</u> - enviar a tag v1.0 para o repositório no  github.  Fica em Releases Tags..

<u>git push origin --tags</u> - vai enviar todas as tags no projeto!

**//buscando branches** 

<u>git fetch -a</u> - vai no repositório no github procurar todas as branches e vai trazer as que vc não tem! 

Após buscar para entrar - git checkout nome da brach. Ex. git checkout cadastro. 

<u>git gc</u> - compime alguns arquivos desnecessários para dar mais performance! As vezes o projeto está muito 

grande, ficando lento para baixar é uma opção!

<u>git shortlog</u> - trás alguns commits que os usuários fizeram. Legal para lembrar onde paramos.

<u>git diff</u> - comparar arquivos locais e romotos para saber quais alterações foram feitas.

<u>git diff HEAD: nome.txt</u> - para comparar arquivos específicos.  

<u>git reflog</u> - Exibe todos os detalhes feitos no repositório. tem tempo de expiração por default de 30 dias. 