# Django-Template (Minimal)

A short, clean README to get this Django template running with a local virtual environment.

## Quick setup

1. Clone the repo
```bash
git clone <repo-url>
cd <project-folder>
```

2. Create a virtual environment in the project root (same folder as manage.py)
```bash
python -m venv venv
```

3. Activate the venv
- Windows (PowerShell):
```powershell
venv\Scripts\Activate
```
- macOS / Linux:
```bash
source venv/bin/activate
```

4. Install dependencies (if present)
```bash
pip install -r requirements.txt
# or at minimum:
pip install django
```

5. Run the dev server
```bash
python manage.py runserver
```

## PyCharm note
Cloning the repo does not auto-create or select a virtual environment in PyCharm. After creating the `venv` above, set it as the project interpreter:
Preferences / Settings → Project → Python Interpreter → Add → Existing environment → select `venv/bin/python` (or `venv\Scripts\python.exe` on Windows).

## Tips
- Never commit the `venv/` folder. Add `venv/` to `.gitignore`.
- Re-run `pip install -r requirements.txt` when dependencies change.
