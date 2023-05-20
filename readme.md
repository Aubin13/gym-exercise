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
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git add all
fatal: pathspec 'all' did not match any files

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git add .

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git status'
> ^C

DASH@DASH-PC MINGW64 ~/Documents/Git/the-gym-rwanda-pt/exercise1 (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md


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