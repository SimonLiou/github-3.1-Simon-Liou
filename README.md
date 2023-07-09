# Simon Liou
## _My Basic Github Project_

Welcome to my page

## Basic Github commands

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

## Annex
 ***See Git download instructions for windows here:**
  > https://kinsta.com/knowledgebase/install-git/
 
 To configure and connect to git repository:
```
  $ git config --global user.name "[name]"      
  ^"Sets the name you want attached to your commit transactions"
  $ git config --global user.email "[email address]"
  ^"Sets the email you want attached to your commit transactions"
  $ git config --global color.ui auto
  ^"Enables helpful colorization of command line output"
  ```

> Do note that if you follow the instructions for downloads below, cd into the folder in Desktop same name as Repo in Git. try `git init`,`git add .` and `git commit -m "push"`, and then `git push`, by the last step the program should ask you for credentials (which is to be done once). If it did not happen. Connect from HTTPS or SSH shown in Annex. Instructions are yet to be tested by myself and is still a work in progress. 
  
  
  ***Creating SSH Keys when credentials manager in downloaded Git is not working**
  
  - go to github.com > settings > SSH & GPG Keys > New SSH Key > Add SSH Key
  - remove existing folder 
  - git clone <SSH URL>
  - git push https://<PERSONALACCESSTOKEN>@github.com/<YOUR git username>/<your repo name>.git

### Resource
- Dillinger
- https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet
- https://training.github.com/
- [GitHub Flow Cheatsheet] https://enterprise.github.com/downloads/en/github-flow-cheatsheet.pdf
- Work based on -cloud-3.1-introduction-to-git-i/assignment.md

**To read:**
-  [Git Flow] https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
- [GitHub Flow] https://docs.github.com/en/get-started/quickstart/github-flow
- [Trunk based development] https://cloud.google.com/architecture/devops/devops-tech-trunk-based-development
- [GitFlow vs GitHubFlow] https://www.geeksforgeeks.org/git-flow-vs-github-flow/ (Optional Read)
