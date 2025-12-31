# MkDocs Documentation Site

This is a MkDocs documentation site using the Material theme.

## Prerequisites

- **Python 3.7 or higher** - [Download Python](https://www.python.org/downloads/)
- **pip** (usually comes with Python)

Verify your Python installation:
```bash
python --version
# or
python3 --version
```

## Getting Started

### Windows

#### 1. Navigate to the project directory
```powershell
cd docs_test_public
```

#### 2. Create a virtual environment
```powershell
python -m venv venv
```

#### 3. Activate the virtual environment

**PowerShell:**
```powershell
.\venv\Scripts\Activate.ps1
```

If you get an execution policy error, run this first:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

**Command Prompt (cmd):**
```cmd
venv\Scripts\activate.bat
```

You should see `(venv)` in your prompt when activated.

#### 4. Install dependencies
```powershell
pip install -r requirements.txt
```

#### 5. Start the development server
```powershell
mkdocs serve
```

The site will be available at `http://127.0.0.1:8000`

---

### macOS

#### 1. Navigate to the project directory
```bash
cd docs_test_public
```

#### 2. Create a virtual environment
```bash
python3 -m venv venv
```

#### 3. Activate the virtual environment
```bash
source venv/bin/activate
```

You should see `(venv)` in your prompt when activated.

#### 4. Install dependencies
```bash
pip install -r requirements.txt
```

#### 5. Start the development server
```bash
mkdocs serve
```

The site will be available at `http://127.0.0.1:8000`

---

## Common Commands

### Development

**Start the development server:**
```bash
mkdocs serve
```

**Start on a custom address/port:**
```bash
mkdocs serve -a 127.0.0.1:8080
```

**Build static site (without serving):**
```bash
mkdocs build
```

**Build to a custom directory:**
```bash
mkdocs build -d site_output
```

### Virtual Environment

**Activate (Windows PowerShell):**
```powershell
.\venv\Scripts\Activate.ps1
```

**Activate (Windows CMD):**
```cmd
venv\Scripts\activate.bat
```

**Activate (macOS/Linux):**
```bash
source venv/bin/activate
```

**Deactivate:**
```bash
deactivate
```

### Other Useful Commands

**Check MkDocs version:**
```bash
mkdocs --version
```

**List available MkDocs commands:**
```bash
mkdocs --help
```

**Validate configuration:**
```bash
mkdocs build --strict
```

---

## Project Structure

```
docs_test_public/
├── docs/              # Documentation source files
│   ├── index.md       # Homepage
│   └── ...
├── mkdocs.yml         # MkDocs configuration
├── requirements.txt   # Python dependencies
└── README.md          # This file
```

---

## Features

This site uses:
- **Material for MkDocs** - Modern documentation theme
- **PyMdown Extensions** - Enhanced markdown features
- Various markdown extensions for:
  - Admonitions (callouts)
  - Code highlighting
  - Emoji support
  - Mermaid diagrams
  - Tabs
  - Task lists
  - And more...

---

## Troubleshooting

### Windows PowerShell Execution Policy Error

If you see: `cannot be loaded because running scripts is disabled on this system`

**Solution:**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### Port Already in Use

If port 8000 is already in use, use a different port:
```bash
mkdocs serve -a 127.0.0.1:8080
```

### Module Not Found Errors

Make sure you've:
1. Activated your virtual environment (see `(venv)` in prompt)
2. Installed dependencies: `pip install -r requirements.txt`

### Python Not Found

- Windows: Make sure Python is added to PATH during installation
- macOS: You may need to use `python3` instead of `python`
- Verify installation: `python --version` or `python3 --version`

### Virtual Environment Issues

If you encounter issues with the virtual environment:
1. Delete the `venv` folder
2. Recreate it: `python -m venv venv` (or `python3 -m venv venv` on macOS)
3. Activate and reinstall: `pip install -r requirements.txt`

---

## Next Steps

- Edit files in the `docs/` directory
- The development server auto-reloads on file changes
- Check `mkdocs.yml` for configuration options
- Visit [MkDocs documentation](https://www.mkdocs.org/) for more information

---

## Stopping the Server

Press `Ctrl+C` in the terminal where `mkdocs serve` is running.

