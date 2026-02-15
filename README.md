# ML Project – Git & GitHub Workflow Demonstration

This repository demonstrates a structured Git workflow for a Python-based machine learning project.  

---

# Submission

```Google Doc Link```

[Google Doc Link ](https://docs.google.com/document/d/1-3h-mPqbebu9Z5HO8Q3aksl7SpeAN_dzulbx1E7xPjA/edit?usp=sharing)

---

# 📌 Project Overview

This project contains:

- `train.py` – Model training script  
- `predict.py` – Inference/prediction logic  
- `utils.py` – Shared helper functions  
- `config.py` – Configuration file  
- `README.md` – Documentation  

The objective is to demonstrate proper Git usage across multiple development scenarios.

---

# Stage 1 – Repository Setup (Foundation)

### Goal:
Initialize a Git repository from scratch and prepare project structure.

### Commands Executed

```bash
cd ~
mkdir ml-project
cd ml-project
git init
touch train.py predict.py utils.py README.md
git status
```

### Outcome

- Git repository initialized
- Project file structure created
- Working directory verified using `git status`

---

# Stage 2 – Version Control Workflow (Application)

### Scenario:
New code added to:
- `train.py`
- `utils.py`

Only these files should be staged and committed.

---

## 1. Stage Specific Files

```bash
git add train.py utils.py
```

✔ Demonstrates selective staging

---

## 2. Commit Changes

```bash
git commit -m "Add training script and utilities"
```

✔ Clear, meaningful commit message

---

## 3. Ensure Branch is `main`

```bash
git branch -M main
```

✔ Standard modern branch naming

---

## 4. Connect to Remote Repository

```bash
git remote add origin https://github.com/yourusername/ml-project.git
```

✔ Links local repo to GitHub

---

## 5. Push to GitHub

```bash
git push -u origin main
```

✔ Sets upstream tracking branch

---

# Stage 3 – Collaborative Workflow (Synthesis)

### Scenario:

Remote (GitHub):
- Updated `predict.py`
- Updated `README.md`

Local:
- Modified `utils.py`
- Created `config.py`
- Changes are uncommitted

---

## Step 1 – Retrieve Teammate Changes

```bash
git pull origin main
```

✔ Synchronizes local repository with remote  
✔ Prevents diverging history

---

## Step 2 – Stage Local Changes

```bash
git add utils.py config.py
```

✔ Stages modified and new files

---

## Step 3 – Commit Local Work

```bash
git commit -m "Update utils and add config file"
```

✔ Logical, descriptive commit

---

## Step 4 – Push to Remote

```bash
git push origin main
```

✔ Publishes work for collaboration

---

# Potential Issues & Resolution Strategies

### Uncommitted Changes Prevent Pull

```bash
git stash
git pull origin main
git stash pop
```

✔ Temporarily stores local changes  
✔ Applies them after syncing  

---

### Remote Changes Ahead of Local

```bash
git pull --rebase origin main
```

✔ Maintains clean linear commit history  

---

### Best Practices for Collaboration

- Pull before pushing
- Use meaningful commit messages
- Stage only relevant files
- Keep branches synchronized
- Avoid force pushing to shared branches

---

# Final Project Structure

```
ml-project/
│
├── train.py
├── predict.py
├── utils.py
├── config.py
└── README.md
```
---

# Screenshots 

## Initial Repository Setup

![Initial repository setup](https://github.com/user-attachments/assets/a15fbdaf-5ed1-49f1-a024-fa57fc15510e)

---

## Status

![Status](https://github.com/user-attachments/assets/d447ea07-757d-4844-8d98-fe12c1fb9773)

---

## Selective Staging and Push

![Selective staging and push](https://github.com/user-attachments/assets/12bb9138-3e19-414d-b622-a91b38ee4df4)

---

## Pull Operation

![Pull operation](https://github.com/user-attachments/assets/6a768093-b807-4ab4-a7bd-decb8599a21f)

---

## Potential Collaboration Issues

![Potential issues](https://github.com/user-attachments/assets/c3f2b37e-7fec-4337-9cf9-f13c5374e6fb)

---

## Handling Such Issues

![Handling issues](https://github.com/user-attachments/assets/df3b690f-0c1b-4b98-b75c-37e3ad294543)



---

