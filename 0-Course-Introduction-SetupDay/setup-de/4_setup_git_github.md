# GitHub Einrichtung & Push - Vollständige Anleitung

Diese Anleitung zeigt, wie man einen neuen Computer mit GitHub verbindet, ein Repository klont, Dateien bearbeitet und Änderungen pusht. Alles von Grund auf.

---

## Schritt 0: Voraussetzungen

* Git installiert. Überprüfen:

```bash
git --version
```

---

## Schritt 1: Git-Identität konfigurieren

```bash
git config --global user.name "Ihr Name"
git config --global user.email "ihre_email@example.com"
```

---

## Schritt 2: GitHub Personal Access Token (PAT) erstellen

1. Gehe zu [GitHub Login](https://github.com/login) → anmelden / Konto erstellen.
2. Navigiere: **Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token**
3. Name: `Laptop Git`
4. Ablauf: `No expiration`
5. Berechtigungen: `repo`
6. Klicke **Generate token** → **Token jetzt kopieren** (wird danach nicht mehr angezeigt)

---

## Schritt 3: Repository klonen

```bash
git clone https://github.com/IhrBenutzername/IhrRepo.git
cd IhrRepo
```

* Git fragt:

```
Username for 'https://github.com': IhrBenutzername
Password for 'https://github.com': <PAT hier einfügen>
```

---

## Schritt 4: Dateien lokal bearbeiten

```bash
# Datei mit Editor öffnen
nano datei.txt
```

---

## Schritt 5: Änderungen zum Commit vorbereiten & committen

```bash
git add .
git commit -m "Änderungen beschreiben"
```

---

## Schritt 6: Änderungen zu GitHub pushen

```bash
git push -u origin main
```

* Benutzername → GitHub Benutzername
* Passwort → Ihr PAT

---

## Schritt 7: Anmeldedaten speichern (optional)

```bash
git config --global credential.helper store
```

* Zukünftige Pushes fragen nicht erneut nach Benutzername/Token.

---

✅ Fertig — Ihr Computer ist vollständig mit GitHub verbunden, Änderungen wurden gepusht.
