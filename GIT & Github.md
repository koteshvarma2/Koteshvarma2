# 🚀 Git & GitHub Guide (Beginner → Advanced)

> A simple, beginner-friendly guide to learn Git and GitHub step by step.

---

# 📌 1. What is Git?

Git is a tool that helps you:

* Track changes in your code
* Go back to previous versions
* Work with others easily

👉 Think of Git like a **save history for your project**

---

# 🌍 2. What is GitHub?

GitHub is a website where you:

* Store your Git projects online
* Share code with others
* Collaborate on projects

---

# ⚙️ 3. Install & Setup Git

Download Git: https://git-scm.com

Set your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Check:

```bash
git config --list
```

---

# 📁 4. Create Your First Project

```bash
mkdir my-project
cd my-project
git init
```

👉 This creates a Git repository

---

# 🔄 5. Basic Workflow (Most Important)

```bash
git status
git add .
git commit -m "first commit"
```

Flow:

```
edit → add → commit
```

---

# 📜 6. View History

```bash
git log
git log --oneline
```

---

# 📂 7. Ignore Files

Create `.gitignore`

Example:

```
node_modules/
*.log
.env
```

---

# 🌿 8. Branching (Work Safely)

```bash
git branch
git checkout -b feature
```

Switch branch:

```bash
git checkout main
```

Merge:

```bash
git merge feature
```

---

# 🌍 9. Connect to GitHub

Create a repo on GitHub, then:

```bash
git remote add origin https://github.com/username/repo.git
git push -u origin main
```

---

# 📥 10. Get Code from GitHub

```bash
git clone https://github.com/username/repo.git
git pull origin main
```

---

# 🔧 11. Undo Mistakes

Unstage:

```bash
git restore --staged file.txt
```

Discard changes:

```bash
git restore file.txt
```

Undo commit safely:

```bash
git revert HEAD
```

---

# 🚀 12. Intermediate Commands

Stash:

```bash
git stash
git stash pop
```

Check changes:

```bash
git diff
```

---

# ⚡ 13. Advanced Git

Rebase:

```bash
git rebase main
```

Cherry-pick:

```bash
git cherry-pick <commit-hash>
```

Tag:

```bash
git tag v1.0
git push origin v1.0
```

---

# 🧠 14. Important Concepts

Git has 3 areas:

* Working Directory
* Staging Area
* Repository

Flow:

```
Working → Staging → Repository
```

---

# ⚔️ 15. Merge Conflicts

If conflict happens:

```
<<<<<<< HEAD
your code
=======
other code
>>>>>>> branch
```

👉 Fix manually → then:

```bash
git add .
git commit
```

---

# 🧩 16. Real Workflow (Industry Style)

```bash
git checkout -b feature-login
# work
git add .
git commit -m "add login"
git push origin feature-login
```

Then:

* Create Pull Request on GitHub
* Review
* Merge

---

# 🛡️ 17. Best Practices

* Commit small changes
* Write clear messages
* Pull before push
* Don’t use `--force` on shared branches

---

# 🧪 18. Practice (Try This)

```bash
git init
echo "hello" > file.txt
git add .
git commit -m "first commit"
git log --oneline
```

---

# 🎯 Final Tip

Git is not about files.

👉 It is about **tracking changes over time**

---

⭐ If this helped you, give this repo a star!
