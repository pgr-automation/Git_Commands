# Git_Commands

Below is a list of commonly used Git commands with explanations and examples:
### 1. Configuration Commands
git config

Used to set user details or other configurations.

    Command:

    git config --global user.name "Your Name"
    git config --global user.email "youremail@example.com"

    Description: Sets your username and email for all repositories. Use --local instead of --global to set it for a specific repository.

### 2. Initialize a Repository
git init

Starts a new Git repository.

    Command:

    git init

    Description: Initializes a new Git repository in the current folder.

### 3. Clone a Repository
git clone

Copies an existing repository to your local machine.

    Command:

    git clone https://github.com/user/repo.git

    Description: Downloads the project and its commit history.

### 4. Check Status
git status

Shows the working directory and staging area status.

    Command:

    git status

    Description: Displays untracked files, changes to be committed, etc.


### 5. Add Changes
git add

Stages changes to be committed.

    Command:

    git add file.txt        # Add a specific file
    git add .               # Add all changes in the current directory

    Description: Prepares changes for the next commit.


### 6. Commit Changes
git commit

Records changes to the repository.

    Command:

    git commit -m "Add feature X"

    Description: Saves changes along with a descriptive message.


### 7. View Log
git log

Shows the commit history.

    Command:

    git log
    git log --oneline       # One-line summary of each commit

    Description: Displays commit details (hash, author, date, and message).


### 8. Create a New Branch
git branch

Lists, creates, or deletes branches.

    Command:

    git branch              # List branches
    git branch new-feature  # Create a new branch

    Description: Manages branches in the repository.


### 9. Switch Branch
git checkout

Switches to another branch.

    Command:

    git checkout new-feature

    Description: Moves to the specified branch. Use git switch in newer Git versions.


### 10. Merge Branch
git merge

Combines changes from another branch into the current branch.

    Command:

    git merge new-feature

    Description: Integrates changes from new-feature into the current branch.


### 11. Push Changes
git push

Uploads changes to a remote repository.

    Command:

    git push origin main    # Push changes to the main branch

    Description: Sends committed changes to the remote repository.


### 12. Pull Changes
git pull

Fetches and merges changes from the remote repository.

    Command:

    git pull origin main

    Description: Updates your local branch with changes from the remote.


### 13. Fetch Changes
git fetch

Downloads changes but does not merge them.

    Command:

    git fetch origin

    Description: Updates your local tracking branches.


### 14. Discard Changes
git checkout or git restore

Reverts changes in the working directory.

    Command:

    git restore file.txt    # Undo changes to a file (newer Git versions)
    git checkout file.txt   # Undo changes to a file (older versions)

    Description: Discards local changes in the specified file.


### 15. Remove Files
git rm

Removes files from the working directory and stages the removal.

    Command:

    git rm file.txt

    Description: Deletes a file and prepares it for the next commit.


### 16. Stash Changes
git stash

Temporarily saves changes.

    Command:

    git stash
    git stash pop           # Apply the last stashed changes

    Description: Saves uncommitted changes for later use.


### 17. Tagging
git tag

Creates a tag for a specific commit.

    Command:

    git tag v1.0
    git tag -a v1.0 -m "Version 1.0"

    Description: Marks a point in the repository's history.


### 18. View Remote
git remote

Manages remote repositories.

    Command:

    git remote -v           # View remotes
    git remote add origin https://github.com/user/repo.git

    Description: Links or lists remote repositories.


### 19. Revert a Commit
git revert

Creates a new commit to undo changes.

    Command:

    git revert <commit-hash>

    Description: Reverts changes from the specified commit.


### 20. Reset Changes
git reset

Undoes commits or unstages files.

    Command:

    git reset --soft HEAD~1  # Keep changes
    git reset --hard HEAD~1  # Discard changes

    Description: Resets the current branch to a specific state.


### 21. Show Changes
git diff

Shows differences between changes.

    Command:

    git diff                # Changes not staged
    git diff --staged       # Changes staged for commit

    Description: Compares file changes.


### 22. Delete a Branch
git branch -d

Deletes a branch.

    Command:

    git branch -d new-feature

    Description: Removes the specified branch.


### 23. Cherry Pick
git cherry-pick

Applies a specific commit to the current branch.

    Command:

    git cherry-pick <commit-hash>

    Description: Adds changes from a single commit.


### 24. Squash Commits
git rebase

Combines multiple commits into one.

    Command:

git rebase -i HEAD~3

Description: Allows interactive editing of the last three commits.

---
#Git Tag Commands

## How to Remove All Git Tags

Follow the steps below to remove all Git tags from both your local and remote repository.

---

### 1. Remove All Local Tags

Run the following command to delete all tags locally:

```bash
git tag -l | xargs git tag -d
```

### 2. 
