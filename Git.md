
## Git Bash

- `ls (=dir)`		      List all files
- `clear(=clr)` 		    Clear console
- `cat <filename>`		Show file content
- `vim`			          Open VIM text editor

## Git Initial Settings

`git --version`						                          Checks Git version

`git config --global user.name <myUserNameForGit>`	Set global user name for the OS

`git config --global user.name`				              Shows global user name

`git config --global user.email <myEmailForGit>`	  Set global user email for the OS

`git config --global user.email`  			            Shows global user name

`git config --global --list`				                List all global user settings (name, email, pass etc.)

`git config --global init.defaultBranch <branchname>`	  Change default branch for all future new repos

`git branch -m <branchname>`				                    Renames current repo current branch

`git log`							                  Show History of commits

`git log --all  --oneline`				      History for all branches and on one line


## Create New Project and Add it to Git:

**create repo** --> **add & commit changes** *(staging area)* --> **push changes to repo**

## Working with repos

`git init`						                  Initialise current directory as empty Git Repo

`git init <project-name>`				        Init with name of repo (creates folder)

`git status`						                Current status of Git Repo (branch, files etc)


`git add filename/dirname`				      Add file/directory to staging area

`git add .`					                    Add all files

`git rm --cached filename/dirname`			Unstage changes (remove from staging area)

`git commit -m "commit message"`				Commit changes with message

`git push -u origin master`

`git push -u "url of repo" master`

## Create New BRANCH & Merging changes

`git branch`						                Show all local branches inside project

`git branch --all`					            Show all existing local + remote branches

`git branch <my-ne-branch-name>`				Create new branch

`git checkout <branch-name>`				    Checkout desired branch (switch to that branch)

`git checkout -b <new-branch-name>`			Create New Branch and switch to it

`git branch -d <branch-name>`				    Delete specified branch locally (then must be removed remote: git pull --prune)

`git pull --prune`					            Updates(delete) remote branche when said branch is deleted locally

`git push -u origin <new-branch-name>`	Push newly created branch to Remote repo/ -u: create new branch with name

`git push`						                Push changes to current branch if it is existing to Remote repo


**NB**: To merge you must be in target branch and specify the branch which is changes source:

`git merge <branch-name>`					  Merge changes from specified branch to current 

`git stash / git stash push`				Save changes in separate location, without adding them

`git stash list`						        Show all saved stashes

`git stash apply / pop`					    Apply stash changes(apply - don't remove from stash list, pop - remove)

`git stash clear`						        Clear all saves stash changes
