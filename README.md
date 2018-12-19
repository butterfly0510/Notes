# Notes

- [Bash](#bash-scripting)
  - [Cheatsheets and Tutorials](#cheatsheets-and-tutorials)
- [Useful Git Commands](#useful-git-commands)
  - [Status and Logs](#status-and-logs)
  - [Branching and Commits](#branching-and-commits)
- [Linux Commands](#linux-commands)
  - [Tmux](#tmux)
  
## Bash Scripting
### Cheatsheets and Tutorials
[Bash scripting cheatsheet](https://devhints.io/bash)

## Useful Git Commands
### Status and Logs
```
git ls-tree -r master --name-only
```
list all the files currently being tracked under the branch `master`

```
git log --graph
git log --graph --all
git log --graph --decorate --oneline
git log --graph --full-history --all --pretty=format:"%h%x09%d%x20%s"
```
Draw a text-based graphical representation of the commit history on the left hand side of the output. 

*ref:*
* https://git-scm.com/docs/git-log 
* https://stackoverflow.com/questions/1838873/visualizing-branch-topology-in-git)

### Branching and Commits
```
git checkout <branch_name> -- <paths>
```
update the working tree with files or directories from another branch, you can use the branch name pointer in the git checkout command (where `--` is used as an end-of-options marker).

*ref:* 
* http://nicolasgallagher.com/git-checkout-specific-files-from-another-branch/

#### Change Commits History
```
git reset --soft [<commit>]
``` 
can be used to squashing multiple commits into one (will re-write the commit history). 

```
git rebase <basebranch> <topicbranch>
```
checks out the topic branch for you and replays it onto the base branch

*ref:*
* https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified
* https://git-scm.com/book/en/v2/Git-Branching-Rebasing

## Linux Commands
### Tmux

*ref:*
* tmux cheatsheet: https://gist.github.com/MohamedAlaa/2961058
