\# Ver se o git funciona



C:\\Users\\Windows>git --version

git version 2.51.0.windows.1



---



c:\\>cd c:\\gittutorialseries



---

\# iniciar o git



c:\\gittutorialseries>git init

Initialized empty Git repository in C:/gittutorialseries/.git/



---

\# registrar o nome do usuario



c:\\gittutorialseries>git config --global user.name

Weverton



\# registrar o nome do usuário como email



c:\\gittutorialseries>git config --global user.name "wevertonluiznsan@gmail.com"







---

\# ver qtd de commits da branch in staging



c:\\gittutorialseries>git status

Untracked files:

  (use "git add <file>..." to include in what will be committed)

        README.md



nothing added to commit but untracked files present (use "git add" to track)



---



\# ver add a file as it looks now to your next commit (stage)



c:\\gittutorialseries>git add README.md





\# status para ver

c:\\gittutorialseries>git status

On branch master



No commits yet



Changes to be committed:

  (use "git rm --cached <file>..." to unstage)

        new file:   README.md





---



\# commit



git commit -m "This is the first commit"



\[master (root-commit) f097c77] This is the first commit

 1 file changed, 6 insertions(+)

 create mode 100644 README.md





\# ver o branch



c:\\gittutorialseries>git branch

\* master





\# renomear a branch

c:\\gittutorialseries>git branch -M main



---

\# criar um repositório online



**c:\\gittutorialseries>git remote add origin https://github.com/wevertonluizsan/gittutorias.git**



\# verificar o repositório online conectadado



**c:\\gittutorialseries>git remote -v**



**origin  https://github.com/wevertonluizsan/gittutorias.git (fetch)**

**origin  https://github.com/wevertonluizsan/gittutorias.git (push)**



**------------------------------------------------------------------------------------------------------**



**# fazer um push**

**git push -u origin main**





**# fazer um restauro**

**git restore README.md**



**-------------------------------------------------------------------------------**



**# criei elementos novos** 



**c:\\gittutorialseries>git status**







**On branch main**

**Your branch is up to date with 'origin/main'.**



**Changes to be committed:**

  **(use "git restore --staged <file>..." to unstage)**

        **modified:   README.md**



**Changes not staged for commit:**

  **(use "git add <file>..." to update what will be committed)**

  **(use "git restore <file>..." to discard changes in working directory)**

        **modified:   README.md**



**Untracked files:**

  **(use "git add <file>..." to include in what will be committed)**

        **teste.txt.txt**









**-------------------------------------------------------------------------------**



**#quero adicionar todas as mudanças**



c:\\gittutorialseries>git add .





\# checo



git status





On branch main

Your branch is up to date with 'origin/main'.



Changes to be committed:

&nbsp; (use "git restore --staged <file>..." to unstage)

&nbsp;       modified:   README.md

&nbsp;       new file:   teste.txt.txt







\# commit 



git commit -m "this is my second commit"





\# git remote -v







\# EXEMPLO DE CLONE DE PASTA CRIEI UMA PASTA CHAMADA GIT NO COMPUTADOR E CLONEI 



c:\\>cd c:\\git



c:\\GIT>git clone https://github.com/wevertonluizsan/gittutorias.git





Cloning into 'gittutorias'...

remote: Enumerating objects: 7, done.

remote: Counting objects: 100% (7/7), done.

remote: Compressing objects: 100% (4/4), done.

remote: Total 7 (delta 1), reused 7 (delta 1), pack-reused 0 (from 0)

Receiving objects: 100% (7/7), done.

Resolving deltas: 100% (1/1), done.



------------------------------------------------------------------------------------------



\# entrar na pasta



cd c:\\git\\gittutorias

git status

git add .

git commit -m "This is third commit"

git push origin main 





-----------------------------------------------------------------------------------------------------------



\# crio arquivo novo chamado de files.txt



git add .

git restore --staged "files.txt"





\# ou



**git reset "files.txt"**



-----------------------------------------



c:\\GIT\\gittutorias>git add .



c:\\GIT\\gittutorias>git diff --staged



c:\\GIT\\gittutorias>git commit -m "this is a new document"



c:\\GIT\\gittutorias>git status



c:\\GIT\\gittutorias> git push origin main







-------------------------------------------



\# criar um novo ramo (branch) chamando o de developer



git branch

\* main



git branch developer





--------------------------------



\# mudar para a o ramo developer, criar alguns arquivos



git checkout developer

git add .

git commit -m "This is a new story that I'm working as developer"

git status



\# mudar para a o ramo main e fazer o merge do developer como main



git merge developer



\# ver os commits em andamento



git status





git push origin main



-----------------------------------------------------------------



\#LOG depois pressione a letra Q



git log





commit 3aa638182a770af559aff6491c4c451559bb3067 (HEAD -> main, origin/main, origin/HEAD, developer)

Author: wevertonluizsan <wevertonluizsan@gmail.com>

Date:   Fri Sep 12 21:51:01 2025 -0300



&nbsp;   This is a new story that I'm working as developer



commit 9419b950a25a86c3274ca98435236e74bf16d7d2

Author: wevertonluizsan <wevertonluizsan@gmail.com>

Date:   Fri Sep 12 21:04:17 2025 -0300



&nbsp;   this is a new document



commit 7f45ed42d36824c865a9e37c9f383637f116552b

Author: wevertonluizsan <wevertonluizsan@gmail.com>

Date:   Fri Sep 12 20:06:14 2025 -0300



&nbsp;   This is third commit



commit 6e454124e54371c1d74f6428846eabd5dd803292

Author: wevertonluizsan <wevertonluizsan@gmail.com>

Date:   Fri Sep 12 19:36:12 2025 -0300



&nbsp;   this is my second commit



commit f097c775d495be24c9865d54543f9f9b30558f08

Author: wevertonluiznsan@gmail.com <wevertonluizsan@gmail.com>

Date:   Thu Sep 11 02:02:41 2025 -0300



&nbsp;   This is the first commit















