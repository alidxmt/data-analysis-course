# GitHub Setup & Push - Full A-Z Guide

This guide shows how to connect a new computer to GitHub, clone your repo, edit, and push changes. Everything from scratch.

---

## Step 0: Prerequisites

* Git installed. Check:

```bash
git --version
```

---

## Step 1: Configure Git Identity

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

---

## Step 2: Create GitHub Personal Access Token (PAT)

1. Go to [GitHub login](https://github.com/login) → login / create account.
2. Navigate: **Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token**
3. Name: `Laptop Git`
4. Expiration: `No expiration`
5. Scope: `repo`
6. Click **Generate token** → **copy the token now** (won’t show again)

---

## Step 3: Clone Your Repository

```bash
git clone https://github.com/YourUsername/YourRepo.git
cd YourRepo
```

* Git will ask:

```
Username for 'https://github.com': YourUsername
Password for 'https://github.com': <paste token here>
```

---

## Step 4: (Optional) Create a Branch

```bash
git checkout -b my-feature
```

---

## Step 5: Edit Files Locally

```bash
# Open file with your editor
nano file.txt
```

---

## Step 6: Stage & Commit Changes

```bash
git add .
git commit -m "Describe my changes"
```

---

## Step 7: Push Changes to GitHub

```bash
git push -u origin my-feature
```

* Username → GitHub username
* Password → your PAT

---

## Step 8: Save Credentials (Optional)

```bash
git config --global credential.helper store
```

* Future pushes won’t ask for username/token.

---

✅ Done — your computer is fully connected to GitHub, edits are pushed, first-time setup included.
