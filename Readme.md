# GIT COURSE

Este é um repositório para aprender a utilizar o Git e GitHub.

Quer saber mais sobre mim? Dá uma olhadinha no meu [LinkedIn](https://www.linkedin.com/in/marquesemanuel/)

**Aprendi sobre:**
- Inicialização de repositórios
- Ciclo de vida dos status
- Commits
    - git commit -am "Mensagem" (comando que já adiciona o arquivo para o *staged* e faz o *commit* com uma mensagem)
- Status
- Logs
- Diffs
- Checkout (desfaz o que foi alterado no arquivo, antes de ser enviado ao *staged*)
- Reset
    - git reset HEAD file.name (remove o arquivo do *staged*)
    - git reset --soft **commit_hash** (remove o *commit* e retorna o arquivo para o *staged*)
    - git reset --mixed **commit_hash** (remove o *commit* e retorna o arquivo para antes do *staged*)
    - git reset --hard **commit_hash** (remove tudo que foi feito no *commit*)
    * Tem que ser informado o hash do commit anterior ao que deseja resetar
