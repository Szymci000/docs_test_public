
Ten dokument opisuje, jak pracować z Git i GitHub w projekcie dokumentacji,
gdzie:
- źródła znajdują się na gałęzi `main`,
- publikacja działa przez CI/CD na gałąź `gh-pages`,
- zmiany przechodzą przez proces **review** przed publikacją.

## 1. Kiedy używać `git init`

Użyj `git init` TYLKO wtedy, gdy **tworzysz nowe repozytorium od zera lokalnie**.

```
mkdir dokumentacja
cd dokumentacja
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/uzytkownik/nazwa-repo.git
git push -u origin main
```

Jeśli repozytorium już istnieje na GitHubie, zaczynasz od:
```
git clone https://github.com/uzytkownik/nazwa-repo.git
```

## 2. Codzienny workflow (z review)

### 2.1. Zaciągnięcie najnowszych zmian
```
git pull
```

### 2.2. Utworzenie nowej gałęzi dla zmian
```
git checkout -b feature/nazwa-zmiany
```

### 2.3. Podgląd lokalny MkDocs
```
mkdocs serve
# http://127.0.0.1:8000
```

### 2.4. Commit
```
git add .
git commit -m "Opis zmian"
```

### 2.5. Push gałęzi
```
git push -u origin feature/nazwa-zmiany
```

### 2.6. Pull Request + review
- Pull Request z `feature/...` → `main`
- review
- merge po akceptacji
- CI/CD publikuje na GitHub Pages

## 3. Poprawki po review
```
git checkout feature/nazwa-zmiany
git pull
git add .
git commit -m "poprawki po review"
git push
```

## 4. Konflikty – rozwiązanie
```
git checkout main
git pull
git checkout feature/nazwa-zmiany
git merge main
```

Rozwiąż ręcznie w plikach, usuń znaczniki konfliktu, potem:
```
git add .
git commit -m "fix: konflikty"
git push
```

## 5. Komendy skrót

| Cel | Komenda |
|------|----------|
| clone | git clone <adres> |
| init | git init |
| pobranie zmian | git pull |
| commit | git commit -m "opis" |
| push | git push |
| nowa gałąź | git checkout -b feature/... |
| merge z main | git merge main |

## 6. Przepływ końcowy

1. git pull
2. git checkout -b feature/...
3. mkdocs serve (opcjonalnie)
4. git add .
5. git commit -m "..."
6. git push -u origin feature/...
7. PR → review → merge
8. deploy na GitHub Pages

