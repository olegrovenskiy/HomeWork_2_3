# HomeWork_2_3

1.
Создан новый репозиторий и склонирован на локальный комп

https://github.com/olegrovenskiy/HomeWork_2_3

2. Созданы файлы и коммит

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git add branching/merge.sh branching/rebase.sh
warning: LF will be replaced by CRLF in branching/merge.sh.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in branching/rebase.sh.
The file will have its original line endings in your working directory

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   branching/merge.sh
        new file:   branching/rebase.sh


(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git commit -m "prepare for merge and rebase"
[main 3c45a69] prepare for merge and rebase
 2 files changed, 16 insertions(+)
 create mode 100644 branching/merge.sh
 create mode 100644 branching/rebase.sh

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git log
commit 3c45a69e90742a6a07128d0d69a65a3cba8dea9b (HEAD -> main)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 11:51:25 2021 +0300

    prepare for merge and rebase

commit 3829acf255e6739dd3c683239f4da41e904da089 (origin/main, origin/HEAD)
Author: olegrovenskiy <83588609+olegrovenskiy@users.noreply.github.com>
Date:   Sat May 15 11:34:02 2021 +0300

    Initial commit

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>

Подготовка файла merge.sh


1. Создание ветки

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git checkout -b git-merge
Switched to a new branch 'git-merge'

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git status
On branch git-merge
nothing to commit, working tree clean

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>


2 и 3 пункты

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git commit -m "merge: @ instead *"
[git-merge 94af17f] merge: @ instead *
 1 file changed, 2 insertions(+), 2 deletions(-)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git status
On branch git-merge
nothing to commit, working tree clean

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git log
commit 94af17f967ca08d65109850c98992e858de388cd (HEAD -> git-merge)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 12:22:32 2021 +0300

    merge: @ instead *

commit 3c45a69e90742a6a07128d0d69a65a3cba8dea9b (main)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 11:51:25 2021 +0300

    prepare for merge and rebase

commit 3829acf255e6739dd3c683239f4da41e904da089 (origin/main, origin/HEAD)
Author: olegrovenskiy <83588609+olegrovenskiy@users.noreply.github.com>
Date:   Sat May 15 11:34:02 2021 +0300

    Initial commit




(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git push origin git-merge
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 822 bytes | 274.00 KiB/s, done.
Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'git-merge' on GitHub by visiting:
remote:      https://github.com/olegrovenskiy/HomeWork_2_3/pull/new/git-merge
remote:
To https://github.com/olegrovenskiy/HomeWork_2_3
 * [new branch]      git-merge -> git-merge

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>

Пункты 4 и 5

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git add branching/merge.sh
warning: LF will be replaced by CRLF in branching/merge.sh.
The file will have its original line endings in your working directory

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git commit -m "merge: use shift"
[git-merge e2924cb] merge: use shift
 1 file changed, 3 insertions(+), 2 deletions(-)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git log
commit e2924cb5b916da9161c502eeb43e6f7d7b100346 (HEAD -> git-merge)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 12:30:11 2021 +0300

    merge: use shift

commit 94af17f967ca08d65109850c98992e858de388cd (origin/git-merge)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 12:22:32 2021 +0300

    merge: @ instead *

commit 3c45a69e90742a6a07128d0d69a65a3cba8dea9b (main)
Author: oleg.rovenskiy <roleg_n@mail.ru>
Date:   Sat May 15 11:51:25 2021 +0300

    prepare for merge and rebase

commit 3829acf255e6739dd3c683239f4da41e904da089 (origin/main, origin/HEAD)
Author: olegrovenskiy <83588609+olegrovenskiy@users.noreply.github.com>
Date:   Sat May 15 11:34:02 2021 +0300

    Initial commit

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>
(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git push origin git-merge
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 481 bytes | 240.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/olegrovenskiy/HomeWork_2_3
   94af17f..e2924cb  git-merge -> git-merge

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>



Изменение main

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git add branching/rebase.sh
warning: LF will be replaced by CRLF in branching/rebase.sh.
The file will have its original line endings in your working directory

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   branching/rebase.sh


(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git commit -m "New Main"
[main 9269c10] New Main
 1 file changed, 4 insertions(+), 2 deletions(-)



(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 414 bytes | 207.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/olegrovenskiy/HomeWork_2_3
   3829acf..9269c10  main -> main

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>



Подготовка файла rebase.sh.

промежуточный итог

https://c2n.me/4c2c7sO.png

Пункт merge

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git merge git-merge
Merge made by the 'recursive' strategy.
 branching/merge.sh | 5 +++--
 1 file changed, 3 insertions(+), 2 deletions(-)

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 390 bytes | 195.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/olegrovenskiy/HomeWork_2_3
   9269c10..bb60512  main -> main

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3>


Результат

https://c2n.me/4c2cdKK.png


После Rebase

https://c2n.me/4c2eSA1.png


(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3\branching>git merge git-rebase
Auto-merging branching/rebase.sh
CONFLICT (content): Merge conflict in branching/rebase.sh
Automatic merge failed; fix conflicts and then commit the result.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3\branching>git add rebase.sh
warning: LF will be replaced by CRLF in branching/rebase.sh.
The file will have its original line endings in your working directory

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3\branching>git merge git-rebase
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3\branching>git commit -m "BEFOR MERGE"
[main af2668f] BEFOR MERGE

(venv) C:\Users\Олег\PycharmProjects\New_Netology\HomeWork_2_3\branching>git merge git-rebase
Already up to date.

