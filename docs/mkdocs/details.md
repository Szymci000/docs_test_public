# Sekcje zwijane

Sekcje zwijane (details) pozwalają na tworzenie rozwijanych/zwijanych sekcji treści. Użytkownik może kliknąć, aby rozwinąć lub zwinąć sekcję. To przydatne do ukrywania szczegółów technicznych, dodatkowych informacji lub opcjonalnych treści.

## Użycie

Sekcje zwijane tworzy się używając składni HTML `<details>`:

````markdown
??? note "Tytuł sekcji"
    Treść sekcji zwijanej.
    Może zawierać wiele linii.
    Wszystkie linie muszą być wcięte o 4 spacje.
````

Dostępne typy:
- `note` - Notatka
- `tip` - Wskazówka
- `warning` - Ostrzeżenie
- `danger` - Niebezpieczeństwo
- `info` - Informacja
- `abstract` - Streszczenie
- `example` - Przykład
- `question` - Pytanie
- `success` - Sukces
- `failure` - Niepowodzenie
- `bug` - Błąd
- `quote` - Cytat

## Przykłady

### Podstawowa sekcja zwijana

??? note "Kliknij, aby rozwinąć"
    To jest treść sekcji zwijanej. Jest ukryta domyślnie i można ją rozwinąć klikając na tytuł.

### Sekcja z różnymi typami

??? tip "Wskazówka"
    To jest sekcja zwijana typu "tip". Użyj jej do wskazówek i pomocnych informacji.

??? warning "Ostrzeżenie"
    To jest sekcja zwijana typu "warning". Użyj jej do ostrzeżeń.

??? danger "Niebezpieczeństwo"
    To jest sekcja zwijana typu "danger". Użyj jej do ostrzeżeń o niebezpieczeństwie.

### Sekcja z kodem

??? example "Przykład kodu"
    ```python
    def example():
        print("To jest przykład w zwijanej sekcji")
        return True
    ```

### Sekcja z listą

??? note "Lista kroków"
    1. Pierwszy krok
    2. Drugi krok
    3. Trzeci krok
    4. Czwarty krok

### Sekcja z admonitions

??? tip "Sekcja z notatką"
    !!! note
        To jest admonition wewnątrz sekcji zwijanej.

### Sekcja bez tytułu

???
    To jest sekcja zwijana bez tytułu. Użyj jej, gdy tytuł nie jest potrzebny.

### Zagnieżdżone sekcje

??? note "Sekcja zewnętrzna"
    To jest zewnętrzna sekcja.
    
    ??? tip "Sekcja wewnętrzna"
        To jest wewnętrzna sekcja zwijana.

### Sekcja z tabelą

??? info "Dodatkowe informacje"
    | Kolumna 1 | Kolumna 2 |
    |-----------|-----------|
    | Wartość 1 | Wartość 2 |
    | Wartość 3 | Wartość 4 |

## Różnica między `???` a `!!!`

- `!!!` - Admonition zawsze widoczny
- `???` - Details zwijany domyślnie

## Wskazówki

- Używaj sekcji zwijanych do ukrywania szczegółów technicznych
- Sekcje zwijane są przydatne do opcjonalnych informacji
- Możesz zagnieżdżać sekcje zwijane
- Treść sekcji musi być wcięta o 4 spacje
- Sekcje zwijane mogą zawierać wszystkie elementy markdown

