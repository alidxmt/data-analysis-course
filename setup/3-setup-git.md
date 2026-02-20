# Python Data Analysis Environment Setup

This guide shows how to create a project folder, set up a Python virtual environment called `data`, install Git, and install common Python data analysis libraries.

---

## 1️⃣ Create a Project Folder and Initialize Git

**Windows (PowerShell or CMD):**
```powershell
mkdir C:\Users\YourUsername\Projects\DataProject
cd C:\Users\YourUsername\Projects\DataProject
# Install Git from https://git-scm.com/downloads if not installed
# Initialize Git repository
git init
```

**macOS / Linux (Terminal):**
```bash
mkdir -p ~/Projects/DataProject
cd ~/Projects/DataProject
# Install Git from https://git-scm.com/downloads if not installed
# Initialize Git repository
git init
```

> Replace the paths with your preferred project location.

---

## 2️⃣ Set Up Python Virtual Environment

### Check Python Version
```bash
python --version
# or
python3 --version
```
> Must be Python ≥ 3.7

### Create the Virtual Environment
```bash
# Windows
python -m venv data

# macOS / Linux
python3 -m venv data
```

> This creates a folder `data` that contains an isolated Python enviro