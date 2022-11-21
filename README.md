# Praticando comandos do git para o github #
 
 ## passo a passo que foi usado pra o versionamento ##
 

user ~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git init
Initialized empty Git repository in C:/Users/maria/OneDrive/Área de Trabalho/Nova pasta/.git/

user ~/OneDrive/Área de Trabalho/Nova pasta (master)
$ code .

 user~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.hrml
        style.css

nothing added to commit but untracked files present (use "git add" to track)

user ~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git add .

user~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git commit -m "Praticando git e github"
[master (root-commit) f717d46] Praticando git e github
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.hrml
 create mode 100644 style.css

user~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git status
On branch master
nothing to commit, working tree clean

user ~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git remote add origin https://github.com/MarianaFariano/praticagit.git

user ~/OneDrive/Área de Trabalho/Nova pasta (master)
$ git branch -M main

user ~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 239 bytes | 59.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/MarianaFariano/praticagit.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.



 ~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    index.hrml
        modified:   style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

no changes added to commit (use "git add" and/or "git commit -a")

 user~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git add .

user~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git commit -m "arrumando ex e estrutura basica"
[main e84fc87] arrumando ex e estrutura basica
 3 files changed, 17 insertions(+)
 delete mode 100644 index.hrml
 create mode 100644 index.html

user~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

 user~/OneDrive/Área de Trabalho/Nova pasta (main)
$ git push origin "main"
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 531 bytes | 531.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/MarianaFariano/praticagit.git
   f717d46..e84fc87  main -> main

