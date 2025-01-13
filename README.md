# 1. Git Basics
## 1.1 git init
Initializes a new Git repository in the current directory.
- Command: `git init`
- Example:
    - `mkdir my_project`
    - `cd my_project`
    - `git init`

Creates a new Git repository in my_project.

## 1.2 git clone
Clones an existing repository from a remote source to your local machine.
- Command: `git clone <repository-url>`
- Example: `git clone https://github.com/username/repo.git`
Clones the repository from the given URL.

## 1.3 git status
Shows the status of your working directory and staging area.
- Command: `git status`
- Example: `git status`
Displays untracked, modified, and staged files.

# 2. Staging and Committing Changes

## 2.1 git add
Stages changes for the next commit.
- Command: `git add <file>`
- Example: `git add index.html`
Stages index.html for committing.
To stage all files: `git add .`

## 2.2 git commit
Records changes to the repository.
- Command: `git commit -m "<message>"`
- Example: `git commit -m "Initial commit"`
Commits the staged changes with the message "Initial commit".

# 3. Branching
## 3.1 git branch
Lists, creates, or deletes branches.
- Command: `git branch`
- Example: `git branch`
Lists all branches.
To create a new branch: `git branch feature-branch`
To delete a branch: `git branch -d feature-branch`

## 3.2 git checkout
Switches between branches or restores files.
- Command: `git checkout <branch>`
- Example: `git checkout feature-branch`
Switches to feature-branch.
To create and switch to a new branch: `git checkout -b new-branch`

# 4. Pushing and Pulling Changes
## 4.1 git push
Uploads local repository content to a remote repository.
- Command: `git push <remote> <branch>`
- Example: `git push origin main`
Pushes the main branch to the origin remote.

## 4.2 git pull
Fetches changes from a remote repository and merges them into the current branch.
- Command: `git pull <remote> <branch>`
- Example: `git pull origin main`
Pulls changes from the main branch of the origin remote.

# 5. Viewing History
## 5.1 git log
Displays the commit history.
- Command: `git log`
- Example: `git log --oneline`
Shows a condensed log of commits.

## 5.2 git diff
Shows the differences between files.
- Command: `git diff`
- Example: `git diff HEAD~1 HEAD`
Compares the most recent commit with the previous one.
