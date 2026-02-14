
<h1 align="center">🚀 Git Quick Reference Cheat Sheet</h1>
<p align="center">
A practical Git reference for daily development workflow.
</p>

---

# 📌 1) Basic Workflow

## ➜ Add Files
```bash
git add file1 file2
git add *.extension
git add .
````

## ➜ Check Status

```bash
git status
```

## ➜ Commit Changes

```bash
git commit -m "Your commit message"
```

## ➜ Push To Remote

```bash
git push origin main
```

---

# 📌 2) Pull Changes

```bash
git pull origin main
```

---

# 📌 3) Branching

## ➜ Show Branches

```bash
git branch
```

## ➜ Create & Switch To New Branch

```bash
git checkout -b branch-name
```

## ➜ Switch Branch

```bash
git checkout branch-name
```

## ➜ Rename Branch

```bash
git branch -m new-name
```

## ➜ Delete Branch

```bash
git branch -d branch-name
```

## ➜ Merge Branch Into Current

```bash
git merge branch-name
```

---

# 📌 4) Stash (Temporary Save)

## ➜ Save Changes

```bash
git stash
```

## ➜ Save With Description

```bash
git stash save "description"
```

## ➜ List Stashes

```bash
git stash list
```

## ➜ Apply Without Delete

```bash
git stash apply stash@{0}
```

## ➜ Apply & Remove

```bash
git stash pop
```

## ➜ Create Branch From Stash

```bash
git stash branch new-branch stash@{0}
```

## ➜ Delete Specific Stash

```bash
git stash drop stash@{0}
```

## ➜ Clear All Stash

```bash
git stash clear
```

---

# 📌 5) Git Config

## ➜ Show Config

```bash
git config --list
```

## ➜ Show Email

```bash
git config --global user.email
```

## ➜ Change Email

```bash
git config --global user.email "your@email.com"
```

## ➜ Edit Config

```bash
git config --global --edit
```

---

# 📌 6) SSH Key (GitHub)

## ➜ Generate Key

```bash
ssh-keygen -t rsa -b 4096 -C "your@email.com"
```

## ➜ Copy Public Key (Mac/Linux)

```bash
cat ~/.ssh/id_rsa.pub
```

## ➜ Copy Public Key (Windows)

```bash
cat C:\Users\YourUser\.ssh\id_rsa.pub
```

## ➜ Test Connection

```bash
ssh -T git@github.com
```

---

# 📌 7) Create Repository From Existing Project

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:username/repo.git
git push -u origin main
```

---

# 📌 8) Restore & Clean

## ➜ Unstage File

```bash
git restore --staged file-name
```

## ➜ Preview Clean

```bash
git clean -n
```

## ➜ Force Clean

```bash
git clean -f
```

---

# 📌 9) Reset

## ➜ Show Log

```bash
git log
```

## ➜ Hard Reset

```bash
git reset --hard commit-hash
```

## ➜ Force Push (Use Carefully)

```bash
git push origin main --force
```

---

# 📌 10) Tags

## ➜ Show Tags

```bash
git tag
```

## ➜ Create Lightweight Tag

```bash
git tag v1.0
```

## ➜ Create Annotated Tag

```bash
git tag -a v1.0 -m "Release version 1.0"
```

## ➜ Push Tag

```bash
git push origin v1.0
```

## ➜ Delete Tag

```bash
git tag -d v1.0
```

## ➜ Delete Remote Tag

```bash
git push origin --delete v1.0
```

---

# 📌 11) Aliases (Shortcuts)

## ➜ Create Alias

```bash
git config --global alias.st status
git config --global alias.br branch
git config --global alias.cm "commit -m"
```

## ➜ Use Alias

```bash
git st
git br
git cm "message"
```

---

# 📌 12) .gitignore Example

```
*.log
node_modules/
.env
```

---

## 💡 Pro Tip

Use meaningful commit messages and follow a clean branching strategy:

* feature/
* bugfix/
* hotfix/

---

<p align="center">
Made with ❤️ for developers
</p>
```
