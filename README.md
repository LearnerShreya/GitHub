

# **My Quick Git & GitHub Commands**

> *A beautifully structured, beginner-to-advanced Git reference for everyday development.*

---

## Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

*Sets your global Git identity — used for all repos on your system.*

---

## Creating a Repository

```bash
git init
```

*Start a new Git repo in the current folder.*

```bash
git clone <repository-URL>
```

*Download (clone) a project from GitHub or any Git server.*

---

## Staging and Committing Changes

```bash
git status
```

*Check current status — what’s changed, what’s staged, which branch you’re on.*

```bash
git add <file>
git add .
```

*Stage individual files or all changes.*

```bash
git commit -m "Your message"
```

*Record changes to the repository with a message.*

```bash
git push
```

*Push committed changes to the remote repo (if set).*

---

## Git Branching – Essential Commands

### List all branches

```bash
git branch
```

*Shows all local branches. Current one marked with `*`.*

---

### Create a new branch

```bash
git branch <branch-name>
```

*Creates a new branch but stays on the current one.*

---

### Switch to a branch

Modern (recommended):

```bash
git switch <branch-name>
```

Classic:

```bash
git checkout <branch-name>
```

*Switch to an existing branch.*

---

### Create and switch to a new branch

Modern (recommended):

```bash
git switch -c <branch-name>
```

Classic:

```bash
git checkout -b <branch-name>
```

*Creates a new branch and switches to it immediately.*

---

### Merge a branch into current branch

```bash
git merge <branch-name>
```

*Merges the given branch into your current one.*

*Ensure changes are committed/stashed before merging to avoid conflicts.*

---

## Pushing and Pulling

```bash
git remote add origin <repository-URL>
```

*Link local repo to remote (only once).*

```bash
git push origin <branch-name>
git pull origin <branch-name>
```

*Send or fetch changes from the remote branch.*

---

## Logs and History

```bash
git log
```

*Shows full commit history.*

```bash
git log --oneline
```

*Compact one-liner log view.*

```bash
git diff
```

*See what's changed but not yet staged.*

---

## Undoing Changes

```bash
git checkout -- <file>
```

*Revert a file to last committed version.*

```bash
git reset <file>
```

*Unstage a file (keeps changes).*

```bash
git reset --hard
```

*Remove all changes — BE CAREFUL: this erases uncommitted work.*

---

## Removing Files

```bash
git rm <file>
```

*Delete a file and stage the deletion for commit.*

---

## Tagging Versions

```bash
git tag <tag-name>
```

*Create a tag (like a bookmark or version label).*

```bash
git push origin <tag-name>
```

*Push tag to the remote repository.*

---

## Reinitializing a Git Repository

```bash
git init
git remote add origin <your-repo-URL>
git add .
git commit -m "Reinitialize repository"
git push -u origin main
```

*Use if `.git/` was deleted or you're resetting the repo.*

*`-u` links your local `main` with remote `origin/main` for future pushes.*

---
