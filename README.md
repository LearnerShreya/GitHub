# My Quick Git and GitHub Commands 

### Configuration
- **Set your Git username:**  
  `git config --global user.name "Your Name"`
- **Set your Git email:**  
  `git config --global user.email "youremail@example.com"`

---

### Creating a Repository
- **Initialize a new repository:**  
  `git init`
- **Clone an existing repository:**  
  `git clone <repository-URL>`

---

### Staging and Committing Changes
- **Check repository status:**  
  `git status`
- **Stage a file:**  
  `git add <file>`
- **Stage all changes:**  
  `git add .`
- **Commit changes:**  
  `git commit -m "Commit message"`
- **Push changes:**
  `git push`

---

### Branching
- **List all branches:**  
  `git branch`
- **Create a new branch:**  
  `git branch <branch-name>`
- **Switch to a branch:**  
  `git switch <branch-name>` (or `git checkout <branch-name>`)
- **Merge a branch:**  
  `git merge <branch-name>`

---

### Pushing and Pulling
- **Link local repo to remote repo:**  
  `git remote add origin <repository-URL>`
- **Push changes:**  
  `git push origin <branch-name>`
- **Pull changes:**  
  `git pull origin <branch-name>`

---

### Logs and History
- **View commit history:**  
  `git log`
- **View simplified commit history:**  
  `git log --oneline`
- **Compare changes:**  
  `git diff`

---

### Undoing Changes
- **Discard changes to a file:**  
  `git checkout -- <file>`
- **Unstage a file:**  
  `git reset <file>`
- **Reset to the last commit:**  
  `git reset --hard`

---

### Removing Files
- **Remove a file and stage the deletion:**  
  `git rm <file>`

---

### Tagging
- **Create a tag:**  
  `git tag <tag-name>`
- **Push a tag to remote repo:**  
  `git push origin <tag-name>`

---

### **Reinitializing a Git Repository**  
If you've removed the `.git` folder or want to reinitialize a Git repository:  
1. **Initialize a new Git repository:**  
   `git init`  
2. **Link to your GitHub repository:**  
   `git remote add origin <your-repo-URL>`  
3. **Stage all changes:**  
   `git add .`  
4. **Commit the changes:**  
   `git commit -m "Reinitialize repository"`  
5. **Push changes to the main branch:**  
   `git push -u origin main`  (This will also set the upstream branch for future pushes)  

