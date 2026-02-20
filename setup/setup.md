# 🐍 Python Installation & PATH Guide

This guide covers installation and PATH configuration for Windows, macOS, and Linux.

---

## 🛠️ 1. Installation Instructions

### 🪟 Windows
1. **Download:** Visit [python.org](https://www.python.org/downloads/windows/) and download the **Windows installer (64-bit)**.
2. **Run Installer:** Open the `.exe` file.
3. **✨ IMPORTANT:** Check the box **"Add Python 3.x to PATH"** at the bottom of the installer.
4. **Install:** Click **Install Now**.
5. **Verify:** Open Command Prompt and type: `python --version`
---
### 🍎 macOS
1. **Method A (Installer):** Download the macOS 64-bit universal2 installer from [python.org](https://www.python.org/downloads/macos/) and run the `.pkg`.
2. **Method B (Homebrew):** If you have Homebrew, run: `brew install python`
3. **Verify:** Open Terminal and type: `python3 --version`
---
### 🐧 Linux (Ubuntu/Debian)
1. **Update:** Open terminal and run: `sudo apt update`
2. **Install:** Run: `sudo apt install python3`
3. **Verify:** Type: `python3 --version`

---

## 🔍 2. Troubleshooting: Adding to PATH

If the command `python` or `python3` is not recognized, follow these steps to manually add it to your system's environment variables.

### **Windows (Manual PATH)**
1. Search for **"Edit the system environment variables"** in the Start menu.
2. Click **Environment Variables** (bottom right).
3. Under **System variables**, find **Path** and click **Edit**.
4. Click **New** and add your Python installation folder (e.g., `C:\Python312\`).
5. Click **New** again and add the Scripts folder (e.g., `C:\Python312\Scripts\`).
6. Click **OK** and restart any open terminals.

### **macOS / Linux (Manual PATH)**
1. Open your shell profile in a text editor:
   ```bash
   nano ~/.zshrc  # (Use ~/.bashrc if on older Linux/Mac)