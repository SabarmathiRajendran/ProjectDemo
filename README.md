# 1. Git Basics

To set up your Git configuration for GitHub on your local machine, you need to configure your user name and email. This ensures your commits are properly attributed to your GitHub account.

**Command to Set Git Configuration:**
- Set your Git username: `git config --global user.name "Your GitHub Username"`
- Set your Git email: `git config --global user.email "your-email@example.com"`
- Verify the configuration: `git config --global --list`

The --global flag sets the configuration for all repositories on your local machine. To configure it for a specific repository, run the command without --global inside that repository.

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

- To stage all files: `git add .`

## 2.2 git commit
Records changes to the repository.
- Command: `git commit -m "<message>"`
- Example: `git commit -m "Initial commit"`

Commits the staged changes with the message "Initial commit".

**To commit and stage changes in one command:**

- Command: git commit -am "<message>"
- Example: git commit -am "Updated index.html"

Stages and commits all modified files with the message "Updated index.html".

# 3. Branching
## 3.1 git branch
**Lists Branches**
- Command: git branch
- Example: git branch

Lists all branches in the repository.

**Create a Branch**
- Command: git branch <branch-name>
- Example: git branch feature-branch

Creates a new branch named feature-branch.

**Delete a Branch**
- Command: git branch -d <branch-name>
- Example: git branch -d feature-branch

Deletes the feature-branch.

## 3.2 git checkout
**Creates a new branch and switches to it.**
- Command: git checkout -b <new-branch>
- Example: git checkout -b feature-branch

Creates and switches to feature-branch.

**Switches to an existing branch.**

- Command: git checkout <branch>
- Example: git checkout main

Switches to main.

- To create and switch to a new branch: `git checkout -b new-branch`

# 4. Pushing and Pulling Changes
## 4.1 git push
Uploads local repository content to a remote repository.
- Command: `git push <remote> <branch>`
- Example: `git push origin main`

Pushes the main branch to the origin remote.

## 4.2 git pull

**Pull Request**
A request to merge changes from one branch (e.g., feature-branch) into another (e.g., main).

Commonly used in collaborative projects for:

- Reviewing code before merging.
- Discussing changes with team members.
- Tracking progress and issues.

**Prerequisites**
Ensure changes are committed and pushed to a remote branch.
Example: git push origin feature-branch

**Creating a Pull Request on GitHub**
- Go to the Repository: Open your GitHub repository in a browser.
- Navigate to Pull Requests: Click the Pull Requests tab.
- Create New Pull Request:
    - Click New Pull Request.
    - Select:
        - Base branch: The branch you want to merge changes into (e.g., main).
        - Compare branch: The branch with your changes (e.g., feature-branch).
- Review Changes: GitHub displays a comparison of the changes between branches.
- Add Details:
    - Enter a descriptive title and summary of the changes.
    - Optionally, link issues (e.g., Closes #123) or tag reviewers.
- Submit the Pull Request:
- Click Create Pull Request.

# 5. Viewing History
## 5.1 git log
Displays the commit history.
- Command: `git log`
- Example: `git log --oneline`

Shows a condensed log of commits.

## 5.2 git diff
Displays changes between the working directory and the staging area.

- Command: git diff
- Example: git diff

Shows modifications not yet staged for commit.

## 5.2 git diff HEAD
Displays changes between the working directory and the latest commit.

- Command: git diff HEAD
- Example: git diff HEAD

Shows all changes made since the last commit.
