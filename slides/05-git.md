# git
## intro
- every commit is actually a snapshot
  - a commit always has an ancestor
  - all commits are part of a tree
  - multiple branches
    - e.g. master
- git tracks every added blob
- we have created and use multiple repos
  - local
  - gogs 
  - your team mates

## what is a merge conflict?
- git compares the history when sync
  - sync succesfull if common ancestor is last commit
  - conflict if history differs
- git comes with a few options to handle merge conflicts
  - rebase: search for common ancestor and reapply commits on it
  - git mergetool
  - manual merge: conflict section are marked. get rid of one!

### NO PANIC
git normaly tells you what to do!  
Keep calm and resolv!

## useful comments
### git blame
- tells you which line was changed by whom

### git log
- shows all commits (searchable)

### git reverse
- reverse a single commit

### git cherrypick
- copies a single commit and execute it on the HEAD

## tipps
- use on daily base
- read first, google second
- checkout the [book](https://git-scm.com/book/en/v2) and the [tutorial](https://try.github.io)
- always rebase
- use branches if you want to test something
- you can recover stashes
- keep your `.gitignore` up to date
- more files, less conflicts
- mindful commit messages
  - what will be changed vs what this will change
- evey subtask should be one commit

