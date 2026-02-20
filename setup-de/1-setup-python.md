*Ali Zolfagharian – GBZ*
# 🐍 Python Installations- & PATH-Anleitung

Installation und PATH-Konfiguration für Windows, macOS und Linux. Bitte folge den Anweisungen entsprechend deinem Betriebssystem.

---

## 🛠️ 1. Installationsanleitung

### 🪟 Windows

1. **Download:** Besuche [python.org](https://www.python.org/downloads/windows/) und lade den **Windows Installer (64-bit)** herunter.
2. **Installer ausführen:** Öffne die `.exe`-Datei.
3. **✨ WICHTIG:** Aktiviere das Kästchen **"Add Python 3.x to PATH"** unten im Installer.
4. **Installieren:** Klicke auf **Install Now**.
5. **Überprüfen:** Öffne die Eingabeaufforderung und tippe: `python --version`

---

### 🍎 macOS

1. **Methode A (Installer):** Lade den macOS 64-bit universal2 Installer von [python.org](https://www.python.org/downloads/macos/) herunter und führe die `.pkg`-Datei aus.
2. **Methode B (Homebrew):** Wenn Homebrew installiert ist, führe aus: `brew install python`
3. **Überprüfen:** Öffne das Terminal und tippe: `python3 --version`

---

### 🐧 Linux (Ubuntu/Debian)

1. **Aktualisieren:** Öffne das Terminal und führe aus: `sudo apt update`
2. **Installieren:** Führe aus: `sudo apt install python3`
3. **Überprüfen:** Tippe: `python3 --version`

---

## 🔍 2. Fehlerbehebung: Hinzufügen zu PATH

Wenn der Befehl `python` oder `python3` nicht erkannt wird, folge diesen Schritten, um ihn manuell zu den Umgebungsvariablen deines Systems hinzuzufügen.

### **Windows (Manueller PATH)**

1. Suche im Startmenü nach **"Systemumgebungsvariablen bearbeiten"**.
2. Klicke auf **Umgebungsvariablen** (unten rechts).
3. Unter **Systemvariablen** finde **Path** und klicke auf **Bearbeiten**.
4. Klicke auf **Neu** und füge deinen Python-Installationsordner hinzu (z. B. `C:\Python312\`).
5. Klicke erneut auf **Neu** und füge den Scripts-Ordner hinzu (z. B. `C:\Python312\Scripts\`).
6. Klicke auf **OK** und starte alle offenen Terminals neu.

### **macOS / Linux (Manueller PATH)**

1. Öffne dein Shell-Profil in einem Texteditor:

   ```bash
   nano ~/.zshrc  # (Nutze ~/.bashrc bei älteren Linux/Mac-Versionen)
   ```
