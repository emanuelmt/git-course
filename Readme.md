# GIT COURSE

Este é um repositório que fiz enquanto aprendi a utilizar o Git e GitHub.

Quer saber mais sobre mim? Dá uma olhadinha no meu [LinkedIn](https://www.linkedin.com/in/marquesemanuel/)

**Aprendi sobre:**
- Inicialização de repositórios
- Status dos arquivos
    - **untracked** (o arquivo ainda não é monitorado pelo git)
    - **unmodified** (o arquivo já foi adicionado mas não possui modificações)
        - Ocorre após o commit do arquivo que estava como **staged**
    - **modified** (o arquivo foi modificado mas ainda não foi adicionado à uma nova versão)
    - **staged** (o arquivo foi adicionado à nova versão e aguarda o commit)
    - ***COMANDOS***
        - git add **file_name** (adiciona o arquivo para o *staged*)
        - git commit -m "message" (faz o *commit* dos arquivos que estão no *staged* passando a ficarem com o status *unmodified*)
        - git commit -am "message" (adiciona o arquivo para o *staged* e faz o *commit* com uma mensagem)
        - git status (mostra os status dos arquivos)
        - git log (mostra o histórico de *commits*)
        - git log --graph (mostra o histórico de *commits* com a árvore)
        - git show **commit_hash** (mostra as alterações que foram feitas no commit informado)
        - git diff (mostra as alterações feitas nos arquivos **modified**)
- Defazendo ações
    - git checkout **file_name** (desfaz o que foi alterado no arquivo, antes de ser enviado ao *staged*)
    - git reset HEAD **file_name** (remove o arquivo do *staged*)
    - git revert **commit_hash** (cria um novo *commit* removendo as alterações efetuadas no *commit* informado)
    - git reset --soft **commit_hash** (remove o *commit* e retorna o(s) arquivo(s) para o *staged*)
    - git reset --mixed **commit_hash** (remove o *commit* e retorna o(s) arquivo(s) para antes do *staged*)
    - git reset --hard **commit_hash** (remove tudo que foi feito no *commit*)
    ***Para o comando reset tem que ser informado o hash do commit anterior ao que deseja resetar***
- Branchs
    - git branch (mostras as *branchs*)
    - git checkout **branch_name** (muda para a *branch* selecionada)
    - git checkout -b **branch_name** (cria uma nova *branch* e muda para a *branch* nova)
    - git merge **branch_name** (mescla a *branch* atual com a *branch* informada mantendo um histórico ramificado)
    - git rebase **branch_name** (mescla a *branch* atual com a *branch* informada, mantendo um histórico linear)
- Versionamento
    - git tag **version** -m "message" (adiciona uma *tag* de versionamento do código)
    - git tag (mostra as *tags* criadas)
    - git tag -d **version** (remove a *tag* informada)
    - git push origin master --tags (envia as *tags* criadas para o repositório remoto)
**Repositórios Remotos**
Após criar um repósitório no GitHub, serão apresentadas instruções para vincular o repositório local com o remoto:
- git remote add origin https://github.com/gituser/repo.git (irá fazer o vínculo com o repositório informado)
- git push -u origin master (envia as alterações locais para o repositório remoto) 
- git pull origin (busca as alterações remotas e faz um merge com o repositório local)
- git clone git@github.com:gituser/repo.git (realiza o clone do repositório localmente utilizando SSH)
- git clone https://github.com/gituser/repo.git (realiza o clone do repositório localmente utilizando HTTPS)
