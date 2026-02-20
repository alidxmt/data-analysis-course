*Ali Zolfagharian*

# Python Data Analysis Environment Setup

This guide shows how to create a project folder, set up a Python virtual environment called `data`, install Git, and install common Python data analysis libraries.

---

## 1️⃣ Create a Project Folder and Initialize Git

> Replace the paths with your preferred project location.For windows "C:\Users\YourUsername\Documents\" and for mac "~/yourpath/" should be replaced.

**Windows (PowerShell or CMD):**

```powershell
mkdir C:\Users\YourUsername\Documents\DataAnalysis
cd C:\Users\YourUsername\ProjDocumentsects\DataAnalysis
# Install Git from https://git-scm.com/downloads if not installed
# Initialize Git repository
git init
```

**macOS / Linux (Terminal):**

```bash
mkdir -p ~/yourpath/DataAnalysis
cd ~/yourpath/DataProDataAnalysisject
# Install Git from https://git-scm.com/downloads if not installed
# Initialize Git repository
git init
```

---

## 2️⃣ Set Up Python Virtual Environment and Install Libraries

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

> This creates a folder `data` that contains an isolated Python environment.

### Activate the Environment and Install Libraries

```bash
# Windows PowerShell
cd data
.\Scripts\Activate.ps1

# Windows CMD
cd data
.\Scripts\activate.bat

# macOS / Linux
cd data
source bin/activate
```

```bash
# Once environment is active, install data analysis libraries
pip install --upgrade pip
pip install jupyter pandas numpy matplotlib seaborn plotly scikit-learn scipy statsmodels
pip install openpyxl xlrd sqlalchemy notebook ipywidgets
```

> Installs core Python data stack including plotting, data manipulation, notebooks, Excel/DB support, and statistical tools.

---

## 3️⃣ Start Jupyter Notebook

```bash
jupyter notebook
```

> Opens a browser interface to create and run notebooks interactively.
