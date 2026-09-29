# Git & GitHub – Basic Commands

## 1. Initialize Git Repository

Use the following command to initialize Git:

```bash
git init
```

---

## 2. Check Git Status

Check the current status of your Git repository:

```bash
git status
```

---

## 3. Add All Files

Add all files to the Git staging area:

```bash
git add .
```

---

## 4. Check Staged Files

Check which files are ready to be committed:

```bash
git status
```

---

## 5. Commit Changes

Create a commit with a meaningful message:

```bash
git commit -m "Add Python programming basics"
```

---

## 6. Rename Branch to Main

Rename the default branch to `main`:

```bash
git branch -M main
```

---

## 7. Connect Local Repository to GitHub

Add your GitHub repository as the remote repository:

```bash
git remote add origin https://github.com/Ziaullah/Into_to_python.git
```

---

## 8. Verify GitHub Remote

Check whether your local repository is connected to GitHub:

```bash
git remote -v
```

Expected output:

```text
origin  https://github.com/Ziaullah/Into_to_python.git (fetch)
origin  https://github.com/Ziaullah/Into_to_python.git (push)
```

---

## 9. Push Code to GitHub

Push your local `main` branch to GitHub:

```bash
git push -u origin main
```

---

# Complete Command Sequence

For a new Git repository, the complete sequence is:

```bash
git init
git status
git add .
git status
git commit -m "Add Python programming basics"
git branch -M main
git remote add origin https://github.com/Ziaullah/Into_to_python.git
git remote -v
git push -u origin main
```

---

# For Future Changes

Once your repository is already connected to GitHub, you **do not need** to run:

```bash
git init
git branch -M main
git remote add origin ...
```

Instead, use:

```bash
git status
git add .
git status
git commit -m "Update Python concepts"
git push
```

---

# Simple Git Workflow

```text
Create / Modify Code
        ↓
   git status
        ↓
     git add .
        ↓
git commit -m "Your message"
        ↓
      git push
        ↓
      GitHub
```

---

# Important Notes

### `git add .`

Adds all new and modified files to the staging area.

### `git commit`

Saves your changes in your local Git history.

### `git push`

Uploads your committed changes to GitHub.

### `git pull`

Downloads the latest changes from GitHub.

### `git status`

Shows the current status of your files.

---

# Example Workflow

Suppose you create a new Python file:

```text
Python_Concepts/
├── 01_What_is_programming.py
├── 02_Python_Uses.py
└── 03_Python_Syntax.py
```

Run:

```bash
git status
git add .
git commit -m "Add Python uses and syntax"
git push
```

Your changes will then appear on GitHub.
