# Python-Schulung – Teil 1

Kursunterlagen als Jupyter-Notebooks:

- [`grundlagen/`](grundlagen/) – Einführung in Python, Variablen/Funktionen, objektorientierte Programmierung
- [`jupiter_animation/`](jupiter_animation/) – animierte Jupiter-Monde-Simulation als OOP-Anwendungsbeispiel

## Installation (Windows 11)

### 1. Python installieren

Auf KPT-Notebooks lässt sich Software nur über das **Unternehmensportal** (Company Portal) installieren – direkte Downloads von python.org funktionieren nicht.

1. Start-Menü öffnen, **"Company Portal"** (bzw. "Unternehmensportal") suchen und öffnen
2. Nach **"Python"** suchen und installieren

Prüfen, ob es geklappt hat (PowerShell oder Eingabeaufforderung öffnen):

```powershell
python --version
```

### 2. VS Code installieren

Ebenfalls über die **Company Portal**-App: nach **"Visual Studio Code"** suchen und installieren.

### 3. VS Code Extensions installieren

In VS Code auf das Extensions-Symbol (linke Seitenleiste) klicken und installieren:

- **Python** (von Microsoft)
- **Jupyter** (von Microsoft)

### 4. Repository herunterladen

Entweder mit Git:

```powershell
git clone https://github.com/grafmi/kpt_python_schulung_part1.git
cd kpt_python_schulung_part1
```

Oder ohne Git: Auf GitHub oben rechts auf **"Code" → "Download ZIP"** klicken und den Ordner entpacken.

### 5. Virtuelle Umgebung erstellen und Pakete installieren

Im Projektordner (in VS Code über **Terminal → New Terminal**, oder in PowerShell):

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

**Falls die Aktivierung mit einem Fehler zur "execution policy" abbricht**, einmalig folgenden Befehl ausführen und danach die Aktivierung wiederholen:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

Falls das auf dem KPT-Notebook von der IT gesperrt ist: Stattdessen die **Eingabeaufforderung (cmd)** statt PowerShell verwenden und dort aktivieren:

```cmd
.venv\Scripts\activate.bat
```

### 6. Notebook öffnen

1. In VS Code den Ordner `kpt_python_schulung_part1` öffnen (**File → Open Folder...**)
2. Ein Notebook öffnen, z. B. `grundlagen/01_einfuehrung.ipynb`
3. Oben rechts auf **"Select Kernel"** klicken → **"Python Environments"** → das eben erstellte `.venv` auswählen
4. Zellen mit `Shift + Enter` ausführen

Fertig – ihr könnt jetzt mit `grundlagen/01_einfuehrung.ipynb` starten.
