# Create a new file named README.md and add some basic information about your project.
# Use Git to stage and commit the README.md file with a meaningful commit message.
# Make some changes to the README.md file and commit these changes with another meaningful commit message.


madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git init
Initialized empty Git repository in C:/Users/madhu/Desktop/assignments1okcoders/git/gitcommands/.git/

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (master)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (master)
$ git add README.md

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (master)
$ git git commit -m "first commit"
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (master)
$ git commit -m "first commit"
[master (root-commit) 715af85] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (master)
$ git branch -m main

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git remote add origin https://github.com/bareddymadhu/Git-commands_23-6-2026.git

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 216 bytes | 216.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/bareddymadhu/Git-commands_23-6-2026.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        image.png

no changes added to commit (use "git add" and/or "git commit -a")

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git add .

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git commit -m "updating readme.md file"
[main eb210a7] updating readme.md file
 2 files changed, 4 insertions(+)
 create mode 100644 image.png

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git remote add origin https://github.com/bareddymadhu/Git-commands_23-6-2026.git
error: remote origin already exists.

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 189.84 KiB | 21.09 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/bareddymadhu/Git-commands_23-6-2026.git
   715af85..eb210a7  main -> main
branch 'main' set up to track 'origin/main'.

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git log --online
fatal: unrecognized argument: --online

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git log
commit eb210a7250fb38ef865f76c1be78a738772fb314 (HEAD -> main, origin/main)
Author: bareddymadhu <madhusudhan6755@gmail.com>
Date:   Sat Jun 27 15:34:29 2026 +0530

    updating readme.md file

commit 715af85c6b41cb20f5839574cb7845c6b556575d
Author: bareddymadhu <madhusudhan6755@gmail.com>
Date:   Sat Jun 27 15:30:24 2026 +0530

    first commit

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git branch feature/new-feature

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git checkout feature/new-feature
Switched to branch 'feature/new-feature'

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git add new-feature.txt
fatal: pathspec 'new-feature.txt' did not match any files

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git add new-feature.txt
fatal: pathspec 'new-feature.txt' did not match any files

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git add new-feature.txt

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git push
fatal: The current branch feature/new-feature has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin feature/new-feature

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git commit -m "text file"
[feature/new-feature 72c6503] text file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new-feature.txt

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (feature/new-feature)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git merge ^C

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git merge ^C

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git merge feature/new-feature
Updating eb210a7..72c6503
Fast-forward
 new-feature.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new-feature.txt

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$ git log
commit 72c6503dd5c966ab9612d527aed26e2aac932788 (HEAD -> main, feature/new-feature)
Author: bareddymadhu <madhusudhan6755@gmail.com>
Date:   Sat Jun 27 15:39:58 2026 +0530

    text file

commit eb210a7250fb38ef865f76c1be78a738772fb314 (origin/main)
Author: bareddymadhu <madhusudhan6755@gmail.com>
Date:   Sat Jun 27 15:34:29 2026 +0530

    updating readme.md file

commit 715af85c6b41cb20f5839574cb7845c6b556575d
Author: bareddymadhu <madhusudhan6755@gmail.com>
Date:   Sat Jun 27 15:30:24 2026 +0530

    first commit

madhu@MadhuSudhanReddy MINGW64 ~/Desktop/assignments1okcoders/git/gitcommands (main)
$

![alt text](image.png)
