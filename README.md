# 🚀 Git & GitHub Workshop — ACM ENISo

Welcome to the **Git & GitHub Workshop** organized by **ACM ENISo**.

This workshop introduces the fundamentals of **Git**, **GitHub**, version control, branching, collaboration, and Pull Requests through a practical exercise.

---

## 🎯 Objectives

By the end of this workshop, you should be able to:

* Understand the basics of Git and GitHub
* Clone a GitHub repository
* Create and switch between branches
* Modify files locally
* Stage and commit changes
* Push a branch to GitHub
* Create a Pull Request
* Understand the basic Git collaboration workflow

---

## 🛠️ Prerequisites

Before starting, make sure you have:

* [Git](https://git-scm.com/) installed
* A [GitHub](https://github.com/) account
* A code editor such as VS Code
* Basic knowledge of the command line

Check your Git installation:

```bash
git --version
```

---

# 🧪 Workshop Exercise

The goal of this exercise is to simulate a real collaborative development workflow.

## 1️⃣ Clone the repository

Clone the workshop repository:

```bash
git clone git@github.com:acm-eniso-coders/workshop-git-github.git
```

Then enter the project directory:

```bash
cd workshop-git-github
```

---

## 2️⃣ Check the repository

Check the current branch:

```bash
git branch
```

Check the remote repository:

```bash
git remote -v
```

You should see the ACM ENISo repository as the remote.

---

## 3️⃣ Create your own branch

Do **not** work directly on `main`.

Create a branch using your name:

```bash
git checkout -b your-name
```

For example:

```bash
git checkout -b khaled
```

You can verify your branch with:

```bash
git branch
```

---

## 4️⃣ Modify the project

Open the file:

```text
hello.py
```

Modify it by adding your name.

For example:

```python
print("Hello from Khaled!")
```

You can make your own modification as long as the original functionality remains understandable.

---

## 5️⃣ Check your changes

Before committing, check which files have been modified:

```bash
git status
```

You can also inspect the changes:

```bash
git diff
```

---

## 6️⃣ Stage your changes

Add the modified file to the staging area:

```bash
git add hello.py
```

Or add all modified files:

```bash
git add .
```

---

## 7️⃣ Create a commit

Create a commit describing your changes:

```bash
git commit -m "Add my name to hello.py"
```

A good commit message should clearly describe what was changed.

---

## 8️⃣ Push your branch

Push your branch to GitHub:

```bash
git push -u origin your-name
```

For example:

```bash
git push -u origin khaled
```

The `-u` option sets the **upstream branch**, allowing you to use simply:

```bash
git push
```

and

```bash
git pull
```

for future operations on this branch.

---

# 🔀 9️⃣ Create a Pull Request

Once your branch has been pushed:

1. Go to the GitHub repository.
2. Open the **Pull Requests** section.
3. Click **New Pull Request**.
4. Select your branch as the source branch.
5. Select `main` as the destination branch.
6. Review your changes.
7. Give your Pull Request a clear title.
8. Create the Pull Request.

Your Pull Request should look like:

```text
your-name  ───────────────►  main
             Pull Request
```

---

# 🔄 Git Workflow

The workflow practiced during this workshop is:

```text
                    GitHub
                      │
                      │ clone
                      ▼
                 Local Repository
                      │
                      │
                 Create Branch
                      │
                      ▼
                  Edit Files
                      │
                      ▼
                 git add
                      │
                      ▼
                git commit
                      │
                      ▼
                  git push
                      │
                      ▼
               Your GitHub Branch
                      │
                      │ Pull Request
                      ▼
                     main
```

---

# 📚 Essential Git Commands

| Command                   | Description                            |
| ------------------------- | -------------------------------------- |
| `git clone <url>`         | Clone a remote repository              |
| `git status`              | Show the current repository state      |
| `git branch`              | List branches                          |
| `git checkout -b <name>`  | Create and switch to a new branch      |
| `git add .`               | Stage changes                          |
| `git commit -m "message"` | Create a commit                        |
| `git push`                | Upload commits to a remote repository  |
| `git pull`                | Download and integrate remote changes  |
| `git merge <branch>`      | Merge a branch                         |
| `git remote -v`           | Display configured remote repositories |

---

# ⚠️ Important Rules

### ❌ Don't work directly on `main`

Always create your own branch:

```bash
git checkout -b your-name
```

### ❌ Don't commit unnecessary files

Before committing, check:

```bash
git status
```

### ✅ Write meaningful commit messages

Good:

```bash
git commit -m "Add participant introduction"
```

Avoid:

```bash
git commit -m "update"
```

or:

```bash
git commit -m "aaa"
```

### ✅ Pull before starting new work

When working on a shared project, make sure your local repository is up to date before starting new work.

---

# 🏆 Challenge

After completing the basic exercise, try the following:

1. Create another file.
2. Commit the change.
3. Push it to your branch.
4. Observe how the Pull Request is automatically updated.
5. Inspect the commit history using:

```bash
git log --oneline
```

---

## 💡 Remember

The basic Git workflow is:

```text
Modify
   ↓
git add
   ↓
git commit
   ↓
git push
```

And when collaborating through GitHub:

```text
Clone
  ↓
Branch
  ↓
Modify
  ↓
Commit
  ↓
Push
  ↓
Pull Request
  ↓
Review
  ↓
Merge
```

---

## 👥 Organized by

**ACM ENISo**

📍 École Nationale d'Ingénieurs de Sousse — Tunisia
