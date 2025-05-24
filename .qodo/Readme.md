# Git exercises
## Bundle 1
### Exercise 1

```zsh
➜  git-exercises2 git:(main) ✗ git init
Initialized empty Git repository in /Users/apple/git-exercises2/.git/
➜  git-exercises2 git:(master) ✗ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Readme.md

nothing added to commit but untracked files present (use "git add" to track)
➜  git-exercises2 git:(master) ✗ git branch -M main
error: refname refs/heads/master not found
fatal: Branch rename failed
➜  git-exercises2 git:(master) ✗ git branch -M main
error: refname refs/heads/master not found
fatal: Branch rename failed
➜  git-exercises2 git:(master) git branch 
➜  git-exercises2 git:(master) git add .
➜  git-exercises2 git:(master) git commit -m "the first ever commit"
On branch master

Initial commit

nothing to commit
➜  git-exercises2 git:(master) git commit -m "the first ever commit"
On branch master

Initial commit

Untracked files:
        .qodo/

nothing added to commit but untracked files present
➜  git-exercises2 git:(master) ✗ git add .
➜  git-exercises2 git:(master) ✗ git commit -m "adding qodo"
[master (root-commit) fae335f] adding qodo
 1 file changed, 1 insertion(+)
 create mode 100644 .qodo/Readme.md
➜  git-exercises2 git:(master) git branch
* master
➜  git-exercises2 git:(master) git branch -M main
➜  git-exercises2 git:(main) git add Readme.md
fatal: pathspec 'Readme.md' did not match any files
➜  git-exercises2 git:(main) ✗ git remote add origin https://github.com/Allan-lang/Git_exercises.git
➜  git-exercises2 git:(main) ✗ status 
zsh: command not found: status
➜  git-exercises2 git:(main) ✗ git status 
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   .qodo/Readme.md

no changes added to commit (use "git add" and/or "git commit -a")
➜  git-exercises2 git:(main) ✗ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

➜  git-exercises2 git:(main) ✗ git push --set-upstream origin main
Counting objects: 4, done.
Writing objects: 100% (4/4), 272 bytes | 136.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/Allan-lang/Git_exercises.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
➜  git-exercises2 git:(main) ✗ git push 
Everything up-to-date
➜  git-exercises2 git:(main) ✗ git checkout -b dev
M       .qodo/Readme.md
Switched to a new branch 'dev'
➜  git-exercises2 git:(dev) ✗ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

➜  git-exercises2 git:(dev) ✗ git push origin dev
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Allan-lang/Git_exercises/pull/new/dev
remote: 
To https://github.com/Allan-lang/Git_exercises.git
 * [new branch]      dev -> dev
➜  git-exercises2 git:(dev) ✗ git checkout -b test
M       .qodo/Readme.md
Switched to a new branch 'test'
➜  git-exercises2 git:(test) ✗ git push origin test
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Allan-lang/Git_exercises/pull/new/test
remote: 
To https://github.com/Allan-lang/Git_exercises.git
 * [new branch]      test -> test
➜  git-exercises2 git:(test) ✗ git checkout dev
M       .qodo/Readme.md
Switched to branch 'dev'
➜  git-exercises2 git:(dev) ✗ git branch -D test
Deleted branch test (was fae335f).
➜  git-exercises2 git:(dev) ✗ git push origin --delete test
To https://github.com/Allan-lang/Git_exercises.git
 - [deleted]         test
➜  git-exercises2 git:(dev) ✗ 
```