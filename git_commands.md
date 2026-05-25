# Git & GitHub Quick Notes

## Create New Project

```bash
# Go to coding folder
cd "D:\Ashu\OneDrive\Desktop\The Directory\Coding"

# Create project
mkdir my-project

# Enter project
cd my-project

# Initialize Git
git init
```

---

# Basic Git Workflow

```bash
# Check status
git status

# Create file
notepad README.md

# Stage one file
git add README.md

# Stage everything
git add .

# Commit changes
git commit -m "Initial commit"

# View commits
git log --oneline
```

---

# Connect GitHub

```bash
# Add remote repository
git remote add origin https://github.com/USERNAME/my-project.git

# Verify remote
git remote -v

# Check branch
git branch
```

Push code:

```bash
# If branch is main
git push -u origin main

# If branch is master
git push -u origin master
```

After first push:

```bash
git push
```

---

# Daily Workflow

```bash
git status
git add .
git commit -m "message"
git push
```

---

# Branching

```bash
# Create branch
git branch feature-1

# Switch branch
git switch feature-1

# Old method
git checkout feature-1

# Show branches
git branch

# Switch back
git switch main
```

---

# Check Ahead / Behind

```bash
git status
```

Examples:

```bash
Your branch is ahead of 'origin/main' by 2 commits.
```

→ Push changes:

```bash
git push
```

---

```bash
Your branch is behind 'origin/main' by 1 commit.
```

→ Pull latest changes:

```bash
git pull
```

---

# See File Changes

```bash
# Show unstaged changes
git diff

# Show staged changes
git diff --staged
```

---

# Pull & Fetch

```bash
# Download + merge changes
git pull

# Download only
git fetch
```

---

# Clone Repository

```bash
git clone https://github.com/USERNAME/REPO.git
```

---

# Commit History

```bash
# Simple history
git log --oneline

# Graph history
git log --graph --oneline --all
```

---

# Undo Commits

```bash
# Undo last commit but keep files
git reset --soft HEAD~1

# Undo last commit completely
git reset --hard HEAD~1
```

---

# Go to Older Commit

```bash
# Temporary move
git checkout COMMIT_ID

# Return back
git switch main
```

---

# Reset to Older Commit

```bash
# Keep files staged
git reset --soft COMMIT_ID

# Keep files unstaged
git reset --mixed COMMIT_ID

# Delete newer commits completely
git reset --hard COMMIT_ID
```

---

# Restore Files

```bash
# Restore modified/deleted file
git restore filename.txt
```

---

# Delete Branches

```bash
# Delete local branch
git branch -d feature-1

# Force delete branch
git branch -D feature-1

# Delete GitHub branch
git push origin --delete feature-1
```

---

# Rename Branch

```bash
git branch -m new-name
```

---

# Stash (Temporary Save)

```bash
# Save unfinished work
git stash

# Restore work
git stash pop
```

---

# Useful Commands

```bash
# Show remotes
git remote -v

# Show commit details
git show COMMIT_ID

# Change last commit message
git commit --amend -m "New message"

# Remove file from Git only
git rm --cached filename.txt
```

---

# .gitignore Example

```bash
node_modules/
.env
dist/
```

---

# Remove Git Tracking

```bash
rmdir /s /q .git
```

---

# Most Important Commands

```bash
git init
git status
git add .
git commit -m "message"
git push
git pull
git branch
git switch branch-name
git log --oneline
git diff
```