# Git Cheatsheet 

This cheat sheet covers the most essential and frequently used Git commands for version control and collaboration.

## Git Basics

* `git init`: Initialize a new Git repository in the current directory.
* `git clone <repository URL>`: Create a local copy of a remote repository.
* `git status`: Check the status of your files (changes, additions, deletions).
* `git add <filename>`: Stage a file for the next commit.
* `git add .`: Stage all changed files.
* `git commit -m "Your commit message"`: Commit staged changes with a message.
* `git log`: View the commit history.
* `git log --oneline`: View a condensed commit history.

## Branching and Merging

* `git branch`: List all branches.
* `git branch <branchname>`: Create a new branch.
* `git checkout <branchname>`: Switch to a different branch.
* `git checkout -b <branchname>`: Create and switch to a new branch.
* `git merge <branchname>`: Merge a specified branch into the current branch.
* `git branch -d <branchname>`: Delete a branch.

## Remote Repositories

* `git remote -v`: List remote repositories.
* `git remote add <name> <url>`: Add a remote repository with a name.
* `git fetch <remote>`: Fetch changes from a remote repository.
* `git pull <remote> <branch>`: Fetch and merge changes from a remote repository.
* `git push <remote> <branch>`: Push your changes to a remote repository.
* `git push --set-upstream <remote> <branch>`: Push changes and set the default remote for the branch.

## Undoing Changes

* `git reset <filename>`: Unstage a file (remove from the staging area).
* `git checkout -- <filename>`: Discard changes in a file.
* `git revert <commit hash>`: Create a new commit that undoes the changes of a previous commit.
* `git reset --hard HEAD~1`: Undo the last commit, discard changes.

## Stashing

* `git stash`: Temporarily save uncommitted changes.
* `git stash list`: List stashed changesets.
* `git stash apply`: Apply the latest stash.
* `git stash pop`: Apply and remove the latest stash.
* `git stash drop`: Discard the latest stash.

## Inspecting Changes

* `git diff`: Show changes between working directory and staging area.
* `git diff --staged`: Show changes between staging area and the last commit.
* `git show <commit hash>`: Show details of a specific commit.

## Additional Tips

* `.gitignore`: Create a file to specify files and patterns to exclude from version control.
* `git config`: Configure user settings (name, email, editor, etc.).
* `git help <command>`: Get help on a specific Git command.
* `git alias`: Create shortcuts for frequently used commands (e.g., `git co` for `git checkout`).

## Workflows

* **Feature Branch Workflow:** A common way to isolate features and collaborate.
* **Gitflow Workflow:** More structured workflow for larger projects.

## Example: Pushing a New Branch

1. `git checkout -b new-feature`
2. *Make your changes and save files.*
3. `git add .`
4. `git commit -m "Add new feature"`
5. `git push --set-upstream origin new-feature` 
