# LaTeX

###  Terminal compile

Simple latex to pdf command : 
	> pdflatex  base.tex 

guide : [http://aty.sdsu.edu/bibliog/latex/LaTeXtoPDF.html]




# GIT

## Commandos Uteis
GIT <command>
* **[add](https://git-scm.com/docs/git-add)** - este comando adiciona ficheiros ao pre commit. 
* **[commit](https://git-scm.com/docs/git-commit)** - este comando realiza o commit dos ficheiros que adicionaste antes. Requer sempre uma mensagem para tal podes usar a opção -m (Exemplo "git commit -m "msg"). O commit apenas adiciona os teus commits ao repositorio local, o que significa que o commit apenas esta na tua maquina, ou seja, quem esta a trabalhar contigo usando o mesmo git ainda não tem acesso as alterações que commitaste, para isso tens de realizar o "push".
* **[push](https://git-scm.com/docs/git-push)** - envia para o repositorio online os commits locais que tu tenhas feito. Depois de um push as outras pessoas podem fazer obter as alterações que tenhas feito ao codigo usando um "pull".
* **[pull](https://git-scm.com/docs/git-pull)** - faz download de alterações realizadas no repositorio online para o teu repositorio local. Quando fazes pull e houver conflitos (ficheiros que tenhas alterado que tenham sofrido alterações no repositorio online) tens de resolver os conflitos, ou seja ver no resultado da operação em que ficheiros é que houve conflitos e corrigir. A seguir mostro como é que os conflitos são mostrados nos ficheiros de codigo, basicamente tens de apagar o codigo que não faz sentido, e remover as linhas com as tags "<<<<<", "====" e ">>>>>".
    ```
     <<<<<<< HEAD:mergetest
     This is my third line
     =======
     This is a fourth line I am adding
     >>>>>>> 4e2b407f501b68f8588aa645acafffa0224b9b78:mergetest
    ```
* **[status](https://git-scm.com/docs/git-status)** - este comando mostra te o estado do Stage atual, ou seja mostra te todos os documentos prontos para serem commitados e os que não estão para ser commitados.


Para mais informações ver [git Reference](https://git-scm.com/docs)


## Ficheiros 
	
**.gitignore** - é um ficherio que diz ao git para ignorar ficheiros quando fazes commit. Util para não encher o repositorio com ficheiros gerados automaticamente quando compilas o teu projecto.


    Exemplo:
    
    depois de fazeres "pdflatex  base.tex" para gerar o documento latex.
    compara o resultado do commando "git status" tendo o ficheiro .gitignore e sem o ter.


O link a seguir tem varios templates de gitignore para diferentes linguagens.
[https://github.com/github/gitignore]




### Markdown language for Readme.md

Um editor de markdown que podes usar é o [dillinger](https://dillinger.io/)

Para mais informação de como escrever com a linguagem Markdown [https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet]
