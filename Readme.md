# GIT COURSE

Este é um repositório que fiz enquanto aprendi a utilizar o Git e GitHub.

Quer saber mais sobre mim? Dá uma olhadinha no meu [LinkedIn](https://www.linkedin.com/in/marquesemanuel/)

**Aprendi sobre:**
- Inicialização de repositórios

*Status dos arquivos*
<ul>
    <li>»» untracked (o arquivo ainda não é monitorado pelo git)</li>
    <li>»» unmodified (o arquivo já foi adicionado mas não possui modificações)</li>
    <li>   - Ocorre após o commit do arquivo que estava como **staged**</li>
    <li>»» modified (o arquivo foi modificado mas ainda não foi adicionado à uma nova versão)</li>
    <li>»» staged (o arquivo foi adicionado à nova versão e aguarda o commit)</li>
    <li>
        <ul>
            <li>**»» COMANDOS**</li>
            <li>⇸ git add **file_name** (adiciona o arquivo para o *staged*)</li>
            <li>⇸ git commit -m "message" (faz o *commit* dos arquivos que estão no *staged* passando a ficarem com o status *unmodified*)</li>
            <li>⇸ git commit -am "message" (adiciona o arquivo para o *staged* e faz o *commit* com uma mensagem)</li>
        </ul>
    </li>
</ul>
- Status
- Logs
- Diffs
- Checkout (desfaz o que foi alterado no arquivo, antes de ser enviado ao *staged*)
- Reset
    - git reset HEAD **file_name** (remove o arquivo do *staged*)
    - git reset --soft **commit_hash** (remove o *commit* e retorna o arquivo para o *staged*)
    - git reset --mixed **commit_hash** (remove o *commit* e retorna o arquivo para antes do *staged*)
    - git reset --hard **commit_hash** (remove tudo que foi feito no *commit*)
    * Tem que ser informado o hash do commit anterior ao que deseja resetar
- Branchs
    - git checkout -b **branch_name** (cria uma nova *branch*)
    - git merge **branch_name** (mescla a *branch* atual com a *branch* informada)
