# Git Exercisesss

## Bundle 1

### Exercise 1

```bash

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (master)
$ git branch -M main

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ touch README.md

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ mv "README.md" "readme.md"

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git add .

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git status

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git remote add origin https://github.com/Aubin13/gym-exercise.git

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git add .

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git push --set-upstream origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Aubin13/gym-exercise.git'

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git commit -m "First exercise commit"
[main (root-commit) df6f42b] First exercise commit
 1 file changed, 3 insertions(+)
 create mode 100644 readme.md

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 281 bytes | 31.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Aubin13/gym-exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git checkout dev
error: pathspec 'dev' did not match any file(s) known to git

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (test)
$ git checkout dev
Switched to branch 'dev'

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (dev)
$ git branch -d test
Deleted branch test (was df6f42b).

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (dev)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Aubin13/gym-exercise/pull/new/dev
remote:
To https://github.com/Aubin13/gym-exercise.git
 * [new branch]      dev -> dev
```


### Exercise 2

```bash

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git add home.html

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash
Saved working directory and index state WIP on dev: 65a8650 changes

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git add about.html

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash
Saved working directory and index state WIP on dev: 65a8650 changes

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git add team.html

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash
Saved working directory and index state WIP on dev: 65a8650 changes

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash list
stash@{0}: WIP on dev: 65a8650 changes
stash@{1}: WIP on dev: 65a8650 changes
stash@{2}: WIP on dev: 65a8650 changes

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (3943f52e113a326beaabf356582dabe7786a6c5d)

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (8035f07908b0df5160a17cba152a66fbdfed5d2c)

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git add -A

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git commit -m "pushed about and team"
[dev ab8a3fd] pushed about and team
 2 files changed, 2 insertions(+), 2 deletions(-)

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git push --set-upstream origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 390 bytes | 195.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/Aubin13/the-gym-bundle1-ex2.git
   65a8650..ab8a3fd  dev -> dev
branch 'dev' set up to track 'origin/dev'.

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash list
stash@{0}: WIP on dev: 65a8650 changes

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git stash pop stash@{0}
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   home.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   about.html

The stash entry is kept in case you need it again.

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git add --all

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git commit -m "pushed home"
[dev d00cc01] pushed home
 2 files changed, 5 insertions(+), 1 deletion(-)

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git reset --hard
HEAD is now at d00cc01 pushed home

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise2 (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

```

