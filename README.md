All commands

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment
$ ls

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment
$ ls -a
./  ../

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment
$ git init
Initialized empty Git repository in D:/GitBasic_Assignment/.git/

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (master)
$ ls -a
./  ../  .git/

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (master)
$ git branch -M main

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git branch

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ echo "Hii I am First" > f1.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ ls
f1.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ cat f1.txt
Hii I am First

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ echo "All commands" >> README.md

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ ls
README.md  f1.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'f1.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git commit -m "initial commit"
[main (root-commit) c1a885e] initial commit
 2 files changed, 2 insertions(+)
 create mode 100644 README.md
 create mode 100644 f1.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git status
On branch main
nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=mehulcharak@gmail.com
user.name=mehulsingh010
core.autocrlf=true
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --local user.name "mehulsingh010"

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --local user.email "mehul.singh@joshsoftware.com"

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=mehulcharak@gmail.com
user.name=mehulsingh010
core.autocrlf=true
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
user.name=mehulsingh010
user.email=mehul.singh@joshsoftware.com

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --local user.email mehul.singh@joshsoftware.com

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=mehulcharak@gmail.com
user.name=mehulsingh010
core.autocrlf=true
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
user.name=mehulsingh010
user.email=mehul.singh@joshsoftware.com

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --local user.name
mehulsingh010

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git config --local user.email
mehul.singh@joshsoftware.com

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git remote add origin git@github.com:mehulsingh010/GitBasic_Assignment.git

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 281 bytes | 281.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:mehulsingh010/GitBasic_Assignment.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git checkout -b feature1
Switched to a new branch 'feature1'

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ echo "feature 1 work" >> feature11.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ echo "feature 12 work" >> feature12.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git add feature11.txt feature12.txt
warning: in the working copy of 'feature11.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'feature12.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git commit -m "work on feature1"
[feature1 1fcddf7] work on feature1
 2 files changed, 2 insertions(+)
 create mode 100644 feature11.txt
 create mode 100644 feature12.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git branch
* feature1
  main

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git checkout -b feature2
Switched to a new branch 'feature2'

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git branch
  feature1
* feature2
  main

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ echo "feature 21 work" >> feature21.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ echo "feature 22 work" >> feautre22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git add feature21.txt feature22.txt
fatal: pathspec 'feature22.txt' did not match any files

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ rm feautre22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt  feature21.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ echo "feature 22 work" >> feature22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt  feature21.txt  feature22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git add feature21.txt feature22.txt
warning: in the working copy of 'feature21.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'feature22.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git commit -m "work on feature2"
[feature2 3d6587e] work on feature2
 2 files changed, 2 insertions(+)
 create mode 100644 feature21.txt
 create mode 100644 feature22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ echo "temporary changes on feature2" >> temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
temporary changes on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        temp.txt

nothing added to commit but untracked files present (use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git stash
No local changes to save

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        temp.txt

nothing added to commit but untracked files present (use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git add temp.txt
warning: in the working copy of 'temp.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git stash
Saved working directory and index state WIP on feature2: 3d6587e work on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
cat: temp.txt: No such file or directory

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git stash list
stash@{0}: WIP on feature2: 3d6587e work on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git stash apply
On branch feature2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
temporary changes on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git add temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git commit -m "restore temporary changes"
[feature2 98252d2] restore temporary changes
 1 file changed, 1 insertion(+)
 create mode 100644 temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git log
commit 98252d2011f1cd8322701e62258deaf08dc9fab8 (HEAD -> feature2)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:27:23 2025 +0530

    restore temporary changes

commit 3d6587eeb5f8c0f294abf56b1d99ccaed618fa64
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:11:43 2025 +0530

    work on feature2

commit 1fcddf75857849aa58c08579c071dc4b5cc5eb0a (feature1)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:04:29 2025 +0530

    work on feature1

commit c1a885efba1559148dc58377dde11abbe4e72b1c (origin/main, main)
Author: mehulsingh010 <mehulcharak@gmail.com>
Date:   Sun Jan 5 00:46:15 2025 +0530

    initial commit

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git reset --soft HEAD~1

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git log
commit 3d6587eeb5f8c0f294abf56b1d99ccaed618fa64 (HEAD -> feature2)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:11:43 2025 +0530

    work on feature2

commit 1fcddf75857849aa58c08579c071dc4b5cc5eb0a (feature1)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:04:29 2025 +0530

    work on feature1

commit c1a885efba1559148dc58377dde11abbe4e72b1c (origin/main, main)
Author: mehulsingh010 <mehulcharak@gmail.com>
Date:   Sun Jan 5 00:46:15 2025 +0530

    initial commit

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt  feature21.txt  feature22.txt  temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
temporary changes on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git commit -m "commit once agaain after the reset soft HEAD~1"
[feature2 41da1ba] commit once agaain after the reset soft HEAD~1
 1 file changed, 1 insertion(+)
 create mode 100644 temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git log
commit 41da1bad2fa60053b90355c51c30e1e4d1eb9231 (HEAD -> feature2)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:50:14 2025 +0530

    commit once agaain after the reset soft HEAD~1

commit 3d6587eeb5f8c0f294abf56b1d99ccaed618fa64
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:11:43 2025 +0530

    work on feature2

commit 1fcddf75857849aa58c08579c071dc4b5cc5eb0a (feature1)
Author: mehulsingh010 <mehul.singh@joshsoftware.com>
Date:   Sun Jan 5 01:04:29 2025 +0530

    work on feature1

commit c1a885efba1559148dc58377dde11abbe4e72b1c (origin/main, main)
Author: mehulsingh010 <mehulcharak@gmail.com>
Date:   Sun Jan 5 00:46:15 2025 +0530

    initial commit

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
temporary changes on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt  feature21.txt  feature22.txt  temp.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git reset --hard HEAD~1
HEAD is now at 3d6587e work on feature2

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt  feature21.txt  feature22.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git status
On branch feature2
nothing to commit, working tree clean

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ cat temp.txt
cat: temp.txt: No such file or directory

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git diff main feature1
diff --git a/feature11.txt b/feature11.txt
new file mode 100644
index 0000000..de3b980
--- /dev/null
+++ b/feature11.txt
@@ -0,0 +1 @@
+feature 1 work
diff --git a/feature12.txt b/feature12.txt
new file mode 100644
index 0000000..ea82668
--- /dev/null
+++ b/feature12.txt
@@ -0,0 +1 @@
+feature 12 work

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git diff

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ echo "uncommit change" >> uncommit.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git add uncommit.txt
warning: in the working copy of 'uncommit.txt', LF will be replaced by CRLF the next time Git touches it

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git diff

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git branch -d feature2
error: Cannot delete branch 'feature2' checked out at 'D:/GitBasic_Assignment'

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git branch -D feature2
error: Cannot delete branch 'feature2' checked out at 'D:/GitBasic_Assignment'

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature2)
$ git checkout main
Switched to branch 'main'
A       uncommit.txt
Your branch is up to date with 'origin/main'.

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git branch -d feature1
error: The branch 'feature1' is not fully merged.
If you are sure you want to delete it, run 'git branch -D feature1'.

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git branch -D feature2
Deleted branch feature2 (was 3d6587e).

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git remote -v
origin  git@github.com:mehulsingh010/GitBasic_Assignment.git (fetch)
origin  git@github.com:mehulsingh010/GitBasic_Assignment.git (push)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git branch
  feature1
* main

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (main)
$ git checkout feature1
Switched to branch 'feature1'
A       uncommit.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git status
On branch feature1
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   uncommit.txt


Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git restore --staged uncommit.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git status
On branch feature1
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        uncommit.txt

nothing added to commit but untracked files present (use "git add" to track)

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ rm uncommit.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ ls
README.md  f1.txt  feature11.txt  feature12.txt

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git push -u origin feature1
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 379 bytes | 379.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feature1' on GitHub by visiting:
remote:      https://github.com/mehulsingh010/GitBasic_Assignment/pull/new/feature1
remote:
To github.com:mehulsingh010/GitBasic_Assignment.git
 * [new branch]      feature1 -> feature1
branch 'feature1' set up to track 'origin/feature1'.

Mehul@hppavilion MINGW64 /d/GitBasic_Assignment (feature1)
$ git branch
* feature1
  main

