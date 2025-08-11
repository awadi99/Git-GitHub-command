
1. Git Configuration Commands
These set up your identity, preferences, and defaults.

Command	Description
git config --global user.name "Your Name"	Sets your Git username (used for commits).
git config --global user.email "you@example.com"	Sets your email for commits.
git config --global core.editor "code --wait"	Sets default text editor (e.g., VS Code).
git config --list	Shows all Git configuration settings.

2. Starting a Repository
Create or clone a repo.

Command	Description
git init	Initializes a new Git repo in current folder.
git clone <url>	Clones an existing remote repo from GitHub.
git clone <url> <folder>	Clones repo into a specific folder.

3. Staging and Committing Changes
Control what changes go into Git history.

Command	Description
git status	Shows changed files and their state.
git add <file>	Stages a specific file.
git add .	Stages all changes in the directory.
git commit -m "message"	Commits staged changes with a message.
git commit -am "message"	Adds & commits only tracked files in one step.

4. Viewing History and Changes
Track what happened in the repo.

Command	Description
git log	Shows commit history.
git log --oneline	Shows compact commit history.
git diff	Shows unstaged changes.
git diff --staged	Shows staged changes.
git show <commit>	Shows details of a commit.

5. Branching
Work on different features or fixes.

Command	Description
git branch	Lists all branches.
git branch <name>	Creates a new branch.
git checkout <branch>	Switches to a branch.
git checkout -b <branch>	Creates & switches to a branch.
git branch -d <branch>	Deletes a branch.
git branch -D <branch>	Force deletes a branch.

6. Merging & Rebasing
Integrating work from different branches.

Command	Description
git merge <branch>	Merges a branch into the current branch.
git rebase <branch>	Re-applies commits from your branch on top of another.
git merge --abort	Cancels a merge in progress.
git rebase --abort	Cancels a rebase in progress.
git rebase --continue	Continues a paused rebase after resolving conflicts.

7. Remote Repositories
Connecting to GitHub.

Command	Description
git remote -v	Shows remote repos linked to local repo.
git remote add origin <url>	Adds a remote named origin.
git remote remove <name>	Removes a remote.
git push -u origin <branch>	Pushes branch to GitHub and sets tracking.
git fetch	Gets latest changes without merging.
git pull	Fetches and merges from remote.
git push	Pushes local commits to remote.

8. Undoing Changes
Fixing mistakes.

Command	Description
git restore <file>	Restores file to last committed version.
git restore --staged <file>	Unstages a file.
git reset <commit>	Moves branch pointer to a commit (keeps changes).
git reset --hard <commit>	Resets to a commit and deletes all changes.
git revert <commit>	Creates a new commit that undoes a commit.

9. Tags
Marking important commits.

Command	Description
git tag	Lists tags.
git tag <tagname>	Creates a tag.
git tag -a <tagname> -m "message"	Creates annotated tag with message.
git push origin <tagname>	Pushes a tag to remote.
git push origin --tags	Pushes all tags.

10. GitHub-Specific Commands
Integration & GitHub CLI.

Command	Description
gh auth login	Logs into GitHub CLI.
gh repo create	Creates a new GitHub repo.
gh repo clone <repo>	Clones a repo from GitHub.
gh issue list	Lists GitHub issues.
gh pr create	Creates a pull request.
gh pr merge	Merges a pull request.

11. Miscellaneous
Extra useful commands.

Command	Description
git stash	Temporarily saves uncommitted changes.
git stash pop	Restores stashed changes.
git clean -fd	Deletes untracked files/folders.
git reflog	Shows all branch history (including deleted commits).
