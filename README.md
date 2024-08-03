# Git Cheat Sheet


## Basic Commands
- **cd**: Change directory.
- **ls**: List files and directories.
- **ls -a**: List all files and directories, including hidden ones.
- **mkdir**: Create a new directory.

## Git Initialization and File Management
- **git init**: Initialize a new Git repository.
- **touch names.txt**: Create a new file named `names.txt`.

## Staging and Committing
- **git status**: View the status of your working directory and staging area.
- **git add names.txt**: Add `names.txt` to the staging area.
- **git add .**: Add all files to the staging area.
- **git commit -m "Added names.txt"**: Commit the staged files with a message.

## Unstaging and Resetting
- **git restore --staged names.txt**: Unstage `names.txt` after staging it.
- **git log**: View the history of commits.
- **git reset commit_Id**: Reset the current branch to a specific commit, deleting commits after it.

## Stashing
- **git stash**: Stash your changes to be able to work on something else without committing the current work.

## Remote Repositories
- **git remote add origin "your GitHub repo link"**: Link the local repository to a GitHub repository.

## Pushing Changes
- **git push origin master**: Push changes to the master branch on GitHub.

## Branching
- **git branch praneeth**: Create a new branch named `praneeth`.
- **git checkout praneeth**: Switch to the `praneeth` branch.
- **git checkout -b new_branch**: Create and switch to a new branch `new_branch` in one step.

## Viewing Branches
- **git branch**: List all local branches.
- **git branch -a**: List all branches, including remote branches.

## Deleting Branches
- **git branch -d branch_name**: Delete a local branch `branch_name`.
- **git push origin --delete branch_name**: Delete a remote branch `branch_name`.

## Contributing to a Repository
1. **Fork** the repository.
2. **Clone** the forked repository.
3. **Create a branch**.
4. **Make changes** and **push** to your branch.

## Pushing and Pulling
- **git push origin praneeth**: Push changes to the `praneeth` branch.
- **git remote add upstream "url"**: Add the original repository as an upstream remote.
- **git pull upstream main**: Pull new commits from the upstream repository.

## Pull Requests
1. **Push changes** to the forked repository.
2. **Open a pull request** from your forked repository.

## Squashing Commits
- **git rebase -i HEAD~n**: Squash the last `n` commits into a single commit. In the interactive rebase screen, replace `pick` with `squash` (or `s`) for the commits you want to squash.

## Handling Merge Conflicts
1. **git merge branch_name**: Attempt to merge `branch_name` into the current branch.
2. If a conflict occurs, Git will mark the conflicted areas in the files.
3. **Resolve the conflicts** manually in your text editor.
4. **git add resolved_file**: Add the resolved files to the staging area.
5. **git commit**: Commit the merge.

## Fetching Changes
- **git fetch**: Fetch updates from the remote without merging them. Useful to see what others have committed before merging.
- **git fetch origin**: Fetch updates from the origin remote.

## Rebasing
- **git rebase branch_name**: Rebase your current branch onto `branch_name`. This is often used to keep your feature branch up to date with the main branch.
- **git rebase --continue**: Continue the rebase process after resolving conflicts.
- **git rebase --abort**: Abort the rebase and return to the state before the rebase started.

## Viewing Changes
- **git diff**: Show changes between working directory and staging area.
- **git diff --staged**: Show changes between staging area and the last commit.

## Undoing Changes
- **git checkout -- file_name**: Discard changes in the working directory.
- **git reset HEAD file_name**: Unstage a file.

## Tagging
- **git tag tag_name**: Create a tag named `tag_name`.
- **git push origin tag_name**: Push a tag to the remote repository.

## Collaborating
- **git pull origin branch_name**: Fetch and merge changes from `branch_name` on the remote repository.

## Viewing Remote Repositories
- **git remote -v**: View all remote repositories and their URLs.

