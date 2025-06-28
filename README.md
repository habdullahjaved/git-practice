# 📘 Git Practice – Beginner-Friendly Git Workflow

Welcome to the **Git Practice** repository!  
This guide walks you through the **complete Git workflow** using the command line, starting from initializing a new project to working with branches and merging features.

---

## 🚀 Getting Started

### Step 1: Create a New Local Project

```bash
mkdir git-practice
cd git-practice
git init
```

## Create some starter files in your editor or manually:

index.html
style.css
.gitignore
README.md

### Example .gitignore content:

gitignore
Copy
Edit
\*.zip
node_modules
.env
.DS_Store
✅ Step 3: Make Your First Commit
Stage and commit your files with a clear message:

## Commands

git add .
git commit -m "feat: initial project setup with HTML and CSS"

## Connect Your Local Repo to GitHub

Create an empty repo named git-practice on GitHub (without README or license).

### Then link your local repo to GitHub and push the initial commit:

git remote add origin https://github.com/habdullahjaved/git-practice.git
git branch -M main
git push -u origin main
Create a Feature Branch
Start working on a new feature in a separate branch:

git checkout -b feature/footer
This helps keep your work isolated and organized.

## Work on the Feature and Commit

Make your changes (for example, add a footer to your website).

Stage and commit with a meaningful message following the Conventional Commits format:

git add .
git commit -m "feat(footer): add footer section with basic styling"
Push your feature branch to GitHub:

git push origin feature/footer
Merge Your Feature Branch into Main
Switch back to main and update it:

git checkout main
git pull origin main
Merge the feature branch into main:

git pull origin feature/footer
Push the updated main branch back to GitHub:

git push origin main
Clean Up Your Branches
Once merged, remove the feature branch locally and remotely:

git branch -d feature/footer
git push origin --delete feature/footer
🎯 Quick Reference: Common Commands

# Initialize new repo and push initial commit

git init
git add .
git commit -m "feat: initial project setup"
git remote add origin https://github.com/yourusername/git-practice.git
git branch -M main
git push -u origin main

# Create a feature branch

git checkout -b feature/xyz
git add .
git commit -m "feat(xyz): add new feature"
git push origin feature/xyz

# Merge feature branch into main

git checkout main
git pull origin main
git pull origin feature/xyz
git push origin main

# Delete feature branch after merge

git branch -d feature/xyz
git push origin --delete feature/xyz
