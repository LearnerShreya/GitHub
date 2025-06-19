
# **Collaborating with Others, Branch Safety & GitHub Workflows**

---

## 1. Collaborating with Others (Forks, Pull Requests, Code Reviews)

### Forking a Repo

* Fork = Make **your own copy** of someone else’s GitHub repo.
* Use when you want to **contribute but don’t have edit access**.

### Cloning Your Fork

```bash
git clone https://github.com/your-username/repo-name.git
```

* Clones your forked repo to your local machine.

### Creating a New Branch

```bash
git checkout -b feature/your-feature-name
```

* Always create a new branch to make changes.

### Add, Commit & Push

```bash
git add .
git commit -m "Your message"
git push origin feature/your-feature-name
```

### Opening a Pull Request (PR)

* Go to your fork on GitHub
* Click **“Compare & Pull Request”**
* Add a title and description → Submit PR

Note: PR = You’re asking the original owner to merge your changes.

---

## 2. Working with Branches Safely

### Stashing Changes

```bash
git stash
```

* Temporarily saves your uncommitted work.

```bash
git stash apply
```

* Bring the stashed changes back.

---

### Rebasing (Advanced)

```bash
git rebase main
```

* Rewrites your branch to start from the latest `main`.
* Keeps history **clean and linear**.
* Use before pushing.

---

### Cherry-Picking a Commit

```bash
git cherry-pick <commit-hash>
```

* Apply a **single commit** from another branch to your current branch.

---

## 3. GitHub Workflows (GUI vs CLI, Issues, Actions)

### Git CLI vs GitHub GUI

| Action      | CLI                      | GitHub Website (GUI)     |
| ----------- | ------------------------ | ------------------------ |
| Clone repo  | `git clone <url>`        | "Code" → Copy link       |
| Make branch | `git checkout -b <name>` | "Branch → New" on web    |
| Make PR     | Push first, then web PR  | "Compare & pull request" |
| Issues      | Not available            | Use "Issues" tab         |

---

### Issues

* Report bugs, request features, or assign tasks.
* Helps teams organize work.

---

### GitHub Actions

* Automate testing, deployment, etc.
* Use `.yml` files inside `.github/workflows/`

Example: Auto-run tests when someone pushes code.

---

## Summary Table

| Concept      | Meaning (in Simple Words)                   |
| ------------ | ------------------------------------------- |
| Fork         | Your own copy of someone else's repo        |
| Clone        | Bring GitHub project to your laptop         |
| Branch       | A separate workspace to test changes        |
| Stash        | Temporarily save work                       |
| Rebase       | Make your changes look like they came later |
| Cherry-pick  | Pick one specific commit                    |
| Pull Request | Ask to merge your changes into main project |
| Issues       | To-do list or bug report                    |
| Actions      | GitHub robots to test or deploy your code   |

---
