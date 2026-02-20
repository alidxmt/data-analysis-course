*Ali Zolfagharian*

# Python Data Analysis Umgebung einrichten

Dieser Leitfaden zeigt, wie man einen Projektordner erstellt, eine Python-virtuelle Umgebung namens `data` einrichtet, Git installiert und gängige Python-Bibliotheken für Datenanalyse installiert.

---

## 1️⃣ Projektordner erstellen und Git initialisieren

> Ersetze die Pfade durch den gewünschten Projektort. Für Windows `C:\Users\DeinBenutzername\Documents\` und für mac `~/deinpfad/`.

**Windows (PowerShell oder CMD):**

```powershell
mkdir C:\Users\DeinBenutzername\Documents\DataAnalysis
cd C:\Users\DeinBenutzername\Documents\DataAnalysis
# Installiere Git von https://git-scm.com/downloads, falls noch nicht installiert
# Git-Repository initialisieren
git init
```

**macOS / Linux (Terminal):**

```bash
mkdir -p ~/deinpfad/DataAnalysis
cd ~/deinpfad/DataAnalysis
# Installiere Git von https://git-scm.com/downloads, falls noch nicht installiert
# Git-Repository initialisieren
git init
```

---

## 2️⃣ Python-virtuelle Umgebung einrichten und Bibliotheken installieren

### Python-Version prüfen

```bash
python --version
# oder
python3 --version
```

> Muss Python ≥ 3.7 sein

### Virtuelle Umgebung erstellen

```bash
# Windows
python -m venv data

# macOS / Linux
python3 -m venv data
```

> Erstellt einen Ordner `data`, der eine isolierte Python-Umgebung enthält.

### Umgebung aktivieren und Bibliotheken installieren

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
# Sobald die Umgebung aktiv ist, installiere die Datenanalyse-Bibliotheken
pip install --upgrade pip
pip install jupyter pandas numpy matplotlib seaborn plotly scikit-learn scipy statsmodels
pip install openpyxl xlrd sqlalchemy notebook ipywidgets
```

> Installiert den Kernstapel für Python-Datenanalyse einschließlich Visualisierung, Datenmanipulation, Notebooks, Excel/DB-Unterstützung und statistischer Werkzeuge.

---

## 3️⃣ Jupyter Notebook starten

```bash
jupyter notebook
```

> Öffnet eine Browseroberfläche, um Notebooks interaktiv zu erstellen und a
