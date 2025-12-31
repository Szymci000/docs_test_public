# MkDocs Documentation Site

To jest strona dokumentacji MkDocs używająca motywu Material.

## Wymagania

- **Python 3.7 lub nowszy** - [Pobierz Python](https://www.python.org/downloads/)
- **pip** (zwykle dołączony do Python)

Sprawdź instalację Python:
```bash
python --version
# lub
python3 --version
```

## Rozpoczęcie pracy

### Windows

#### 1. Przejdź do katalogu projektu
```powershell
cd docs_test_public
```

#### 2. Utwórz virtual environment
```powershell
python -m venv venv
```

#### 3. Aktywuj virtual environment

**PowerShell:**
```powershell
.\venv\Scripts\Activate.ps1
```

Jeśli pojawi się błąd execution policy, najpierw uruchom:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

**Command Prompt (cmd):**
```cmd
venv\Scripts\activate.bat
```

Po aktywacji powinieneś zobaczyć `(venv)` w swoim promptcie.

#### 4. Zainstaluj zależności
```powershell
pip install -r requirements.txt
```

#### 5. Uruchom development server
```powershell
mkdocs serve
```

Strona będzie dostępna pod adresem `http://127.0.0.1:8000`

---

### macOS

#### 1. Przejdź do katalogu projektu
```bash
cd docs_test_public
```

#### 2. Utwórz virtual environment
```bash
python3 -m venv venv
```

#### 3. Aktywuj virtual environment
```bash
source venv/bin/activate
```

Po aktywacji powinieneś zobaczyć `(venv)` w swoim promptcie.

#### 4. Zainstaluj zależności
```bash
pip install -r requirements.txt
```

#### 5. Uruchom development server
```bash
mkdocs serve
```

Strona będzie dostępna pod adresem `http://127.0.0.1:8000`

---

## Najczęściej używane komendy

### Development

**Uruchom development server:**
```bash
mkdocs serve
```

**Uruchom na niestandardowym adresie/porcie:**
```bash
mkdocs serve -a 127.0.0.1:8080
```

**Zbuduj statyczną stronę (bez serwowania):**
```bash
mkdocs build
```

**Zbuduj do niestandardowego katalogu:**
```bash
mkdocs build -d site_output
```

### Virtual Environment

**Aktywuj (Windows PowerShell):**
```powershell
.\venv\Scripts\Activate.ps1
```

**Aktywuj (Windows CMD):**
```cmd
venv\Scripts\activate.bat
```

**Aktywuj (macOS/Linux):**
```bash
source venv/bin/activate
```

**Deaktywuj:**
```bash
deactivate
```

### Inne przydatne komendy

**Sprawdź wersję MkDocs:**
```bash
mkdocs --version
```

**Wyświetl dostępne komendy MkDocs:**
```bash
mkdocs --help
```

**Zweryfikuj konfigurację:**
```bash
mkdocs build --strict
```

---

## Struktura projektu

```
docs_test_public/
├── docs/              # Pliki źródłowe dokumentacji
│   ├── index.md       # Strona główna
│   └── ...
├── mkdocs.yml         # Konfiguracja MkDocs
├── requirements.txt   # Zależności Python
└── README.md          # Ten plik
```

---

## Funkcje

Ta strona używa:
- **Material for MkDocs** - Nowoczesny motyw dokumentacji
- **PyMdown Extensions** - Rozszerzone funkcje markdown
- Różne rozszerzenia markdown dla:
  - Admonitions (callouts)
  - Code highlighting
  - Emoji support
  - Mermaid diagrams
  - Tabs
  - Task lists
  - I więcej...

---

## Rozwiązywanie problemów

### Błąd Execution Policy w Windows PowerShell

Jeśli widzisz: `cannot be loaded because running scripts is disabled on this system`

**Rozwiązanie:**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### Port już zajęty

Jeśli port 8000 jest już zajęty, użyj innego portu:
```bash
mkdocs serve -a 127.0.0.1:8080
```

### Błędy Module Not Found

Upewnij się, że:
1. Aktywowałeś virtual environment (zobacz `(venv)` w promptcie)
2. Zainstalowałeś zależności: `pip install -r requirements.txt`

### Python nie znaleziony

- Windows: Upewnij się, że Python został dodany do PATH podczas instalacji
- macOS: Możesz potrzebować użyć `python3` zamiast `python`
- Zweryfikuj instalację: `python --version` lub `python3 --version`

### Problemy z Virtual Environment

Jeśli napotkasz problemy z virtual environment:
1. Usuń folder `venv`
2. Utwórz go ponownie: `python -m venv venv` (lub `python3 -m venv venv` na macOS)
3. Aktywuj i zainstaluj ponownie: `pip install -r requirements.txt`

---

## Następne kroki

- Edytuj pliki w katalogu `docs/`
- Development server automatycznie przeładowuje się przy zmianach plików
- Sprawdź `mkdocs.yml` dla opcji konfiguracji
- Odwiedź [dokumentację MkDocs](https://www.mkdocs.org/) po więcej informacji

---

## Zatrzymywanie serwera

Naciśnij `Ctrl+C` w terminalu, w którym działa `mkdocs serve`.

