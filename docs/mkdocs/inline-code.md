# Kod inline

Kod inline pozwala na wyświetlanie krótkich fragmentów kodu w tekście z podświetlaniem składni. To przydatne do odwoływania się do zmiennych, funkcji, komend lub krótkich fragmentów kodu w kontekście zdania.

## Użycie

Kod inline tworzy się używając backticków (odwrotnych apostrofów):

````markdown
Użyj komendy `npm install` aby zainstalować pakiety.

Zmienna `const x = 1` jest zdefiniowana jako stała.
````

## Przykłady

### Podstawowy kod inline

Użyj komendy `npm install` aby zainstalować pakiety.

Zmienna `const x = 1` jest zdefiniowana jako stała.

### Kod inline w kontekście

Funkcja `calculateSum()` zwraca sumę dwóch liczb.

Aby uruchomić serwer, użyj komendy `python manage.py runserver`.

### Kod inline z różnymi językami

W JavaScript użyj `const` do deklaracji stałych.

W Python użyj `def` do definiowania funkcji.

W HTML użyj `<div>` do tworzenia kontenerów.

### Kod inline w listach

- Uruchom `npm start` aby rozpocząć serwer deweloperski
- Użyj `git commit -m "message"` aby utworzyć commit
- Wykonaj `docker build` aby zbudować obraz

### Kod inline w admonitions

!!! tip "Wskazówka"
    Użyj `console.log()` aby wyświetlić wartości w konsoli.

!!! warning "Ostrzeżenie"
    Komenda `rm -rf` jest niebezpieczna - usuwa pliki bez możliwości przywrócenia.

### Kod inline z formatowaniem

Możesz używać **pogrubienia** z `kodem inline` w tym samym zdaniu.

Możesz również używać *kursywy* z `kodem inline`.

### Kod inline w tabelach

| Komenda | Opis |
|---------|------|
| `npm install` | Instalacja pakietów |
| `npm start` | Uruchomienie serwera |
| `npm test` | Uruchomienie testów |
| `npm build` | Budowanie aplikacji |

### Kod inline z zmiennymi

Zmienna `userName` przechowuje nazwę użytkownika.

Funkcja `getUserData()` zwraca dane użytkownika.

### Kod inline z ścieżkami

Plik znajduje się w `src/components/Button.js`.

Katalog `node_modules` zawiera zainstalowane pakiety.

### Kod inline z komendami systemowymi

W systemie Windows użyj `dir` aby wyświetlić zawartość katalogu.

W systemie Linux użyj `ls` aby wyświetlić zawartość katalogu.

### Kod inline z parametrami

Funkcja `fetch(url, options)` przyjmuje dwa parametry.

Komenda `git commit -m "message"` używa flagi `-m` do podania wiadomości.

## Różnica między kodem inline a blokami kodu

- **Kod inline** (`backtick`) - krótkie fragmenty w tekście
- **Bloki kodu** (```) - dłuższe fragmenty z podświetlaniem składni

## Wskazówki

- Używaj kodu inline do krótkich fragmentów kodu w tekście
- Kod inline nie ma podświetlania składni, ale jest czytelny
- Używaj backticków do oznaczania komend, zmiennych, funkcji
- Kod inline jest automatycznie formatowany z monospace fontem
- Nie używaj kodu inline do długich fragmentów - użyj bloków kodu zamiast tego

