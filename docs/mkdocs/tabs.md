# Zakładki

Zakładki pozwalają na organizowanie treści w sekcjach, które użytkownik może przełączać. To przydatne narzędzie do prezentowania alternatywnych opcji, różnych wersji kodu lub kategoryzacji informacji.

## Użycie

Zakładki tworzy się używając składni z trzema dwukropkami i etykietą:

````markdown
=== "Tytuł pierwszej zakładki"
    Treść pierwszej zakładki.
    Może zawierać wiele linii.

=== "Tytuł drugiej zakładki"
    Treść drugiej zakładki.
    
    Może również zawierać:
    - Listy
    - **Formatowanie**
    - I inne elementy markdown
````

## Przykłady

### Podstawowe zakładki

=== "Opcja A"
    To jest treść pierwszej zakładki. Możesz umieścić tutaj dowolną treść.

=== "Opcja B"
    To jest treść drugiej zakładki. Każda zakładka może zawierać różną ilość treści.

=== "Opcja C"
    To jest treść trzeciej zakładki.

### Zakładki z kodem

=== "Python"
    ```python
    def hello():
        print("Hello from Python!")
    ```

=== "JavaScript"
    ```javascript
    function hello() {
        console.log("Hello from JavaScript!");
    }
    ```

=== "Java"
    ```java
    public void hello() {
        System.out.println("Hello from Java!");
    }
    ```

### Zakładki z listami

=== "Instalacja Windows"
    1. Pobierz instalator
    2. Uruchom plik .exe
    3. Postępuj zgodnie z instrukcjami

=== "Instalacja macOS"
    1. Pobierz plik .dmg
    2. Otwórz obraz dysku
    3. Przeciągnij aplikację do folderu Applications

=== "Instalacja Linux"
    ```bash
    sudo apt-get update
    sudo apt-get install package-name
    ```

### Zakładki z admonitions

=== "Informacja"
    !!! note
        To jest notatka w zakładce.

=== "Ostrzeżenie"
    !!! warning
        To jest ostrzeżenie w zakładce.

=== "Wskazówka"
    !!! tip
        To jest wskazówka w zakładce.

## Zagnieżdżone zakładki

Zakładki mogą być zagnieżdżone (choć nie jest to zalecane ze względu na UX):

=== "Zewnętrzna 1"
    === "Wewnętrzna A"
        Treść wewnętrznej zakładki A.
    
    === "Wewnętrzna B"
        Treść wewnętrznej zakładki B.

=== "Zewnętrzna 2"
    Treść zewnętrznej zakładki 2.

## Wskazówki

- Używaj zakładek do prezentowania alternatywnych opcji
- Unikaj zbyt wielu zakładek (3-5 to optymalna liczba)
- Każda zakładka powinna mieć jasny, opisowy tytuł
- Treść w zakładkach powinna być wcięta o 4 spacje

