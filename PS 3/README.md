# Git Repository Setup and Basic Commands

This guide walks you through the process of creating a local Git repository, committing your files, and pushing your project to GitHub.

---

## 🧩 Step 1: Initialize a Local Git Repository

Open your terminal inside your project folder and run:

```bash
git init
```

## 🗃️ Step 2: Add Your Project Files

If you haven’t created a file yet, make one:

```
echo "# My Project" > README.md
```

Then add all files to the staging area:
```
git add .
```
Use git add . to add all files, or specify a single file (e.g. git add index.html).

## 💬 Step 3: Commit Your Changes

Create your first commit:
```
git commit -m "Initial commit"
```
The -m flag lets you include a message describing the changes you made.

## 🌐 Step 4: Create a GitHub Repository

Go to GitHub → New Repository

1. Enter a name for your repository (e.g., my-project)
2. Choose Public or Private
3. Click Create repository

## 🔗 Step 5: Connect Local Repo to GitHub

Copy your repository URL from GitHub.
Then, connect it to your local repository using one of these commands:

For HTTPS:
```
git remote add origin https://github.com/username/my-project.git
```
For SSH:
```
git remote add origin git@github.com:username/my-project.git
```

Verify the remote:
```
git remote -v
```

## ⬆️ Step 6: Push Code to GitHub

If this is your first push:
```
git branch -M main
git push -u origin main
```

Afterward, just use:
```
git push
```
The -u flag sets your GitHub repo as the default remote branch, so future pushes can be done with just git push.

# 🧭 Optional Useful Commands
| Command           | Description                              |
| ----------------- | ---------------------------------------- |
| `git status`      | Shows which files are staged or modified |
| `git log`         | Displays commit history                  |
| `git pull`        | Fetches and merges updates from GitHub   |
| `git clone <URL>` | Copies an existing repo to your computer |

