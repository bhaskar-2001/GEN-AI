# Git Commands – Complete Reference 

This file contains commonly used Git commands with clear descriptions.
Useful for beginners, interviews, and real-world development.

---

## 1. Git Configuration

git config --global user.name "Your Name"  
Sets the global Git username.

git config --global user.email "you@email.com"  
Sets the global Git email.

git config --list  
Displays all Git configuration settings.

---

## 2. Repository Setup

git init  
Initializes a new Git repository.

git clone <repository_url>  
Clones a remote repository to local machine.

---

## 3. Status & Logs

git status  
Shows current working directory status.

git log  
Shows commit history.

git log --oneline  
Shows compact commit history.

git log --oneline --graph --all  
Shows commit history with branch graph.

git show <commit_id>  
Displays details of a specific commit.

---

## 4. Staging & Commit

git add <file>  
Stages a specific file.

git add .  
Stages all changes.

git commit -m "message"  
Creates a commit.

git commit --amend  
Edits the last commit.

---

## 5. Branching

git branch  
Lists local branches.

git branch -r  
Lists remote branches.

git branch <branch_name>  
Creates a new branch.

git checkout <branch_name>  
Switches to another branch.

git checkout -b <branch_name>  
Creates and switches to a new branch.

git branch -d <branch_name>  
Deletes a merged branch.

git branch -D <branch_name>  
Force deletes a branch.

---

## 6. Merging & Rebasing

git merge <branch_name>  
Merges a branch into current branch.

git merge --ff-only <branch_name>  
Fast-forward merge only.

git rebase <branch_name>  
Rebases current branch onto another branch.

git rebase -i HEAD~n  
Interactive rebase for last n commits.

git rebase --continue  
Continues rebase after resolving conflicts.

git rebase --abort  
Cancels rebase.

---

## 7. Remote Repository

git remote -v  
Shows remote URLs.

git remote add origin <url>  
Adds remote repository.

git push origin <branch>  
Pushes branch to remote.

git push -u origin <branch>  
Pushes and sets upstream.

git pull  
Fetches and merges from remote.

git fetch  
Fetches changes without merging.

git fetch --prune  
Removes deleted remote branch references.

git push origin --delete <branch>  
Deletes remote branch.

---

## 8. Undo & Reset

git restore <file>  
Discards file changes.

git restore --staged <file>  
Unstages a file.

git reset --soft HEAD~1  
Undo commit, keep changes staged.

git reset --mixed HEAD~1  
Undo commit, keep changes unstaged.

git reset --hard HEAD~1  
Deletes commit and changes completely.

---

## 9. Stash

git stash  
Saves uncommitted changes.

git stash list  
Lists all stashes.

git stash apply  
Applies last stash.

git stash drop  
Deletes a stash.

git stash clear  
Deletes all stashes.

---

## 10. Tags

git tag  
Lists tags.

git tag v1.0  
Creates a tag.

git push origin v1.0  
Pushes tag to remote.

---

## 11. Cleaning

git clean -n  
Shows files to be deleted.

git clean -f  
Deletes untracked files.

git clean -fd  
Deletes untracked files and directories.

---

## 12. Advanced / Recovery

git reflog  
Shows history of HEAD movements.

git cherry-pick <commit_id>  
Applies a specific commit.

git blame <file>  
Shows who modified each line.

---

## 13. Force Push (Use Carefully)

git push origin main --force  
Overwrites remote history.

---

## Best Practices

• Commit small logical changes  
• Use rebase for clean history  
• Avoid force push on shared branches  
• Delete merged branches regularly  

---