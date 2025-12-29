# Podświetlanie tekstu

Funkcja podświetlania tekstu pozwala na wyróżnianie fragmentów tekstu, podobnie jak markerem. To przydatne do zwracania uwagi na ważne informacje lub fragmenty kodu.

## Użycie

Tekst podświetla się używając podwójnego znaku równości `==`:

````markdown
To jest ==podświetlony tekst== w zdaniu.
````

## Przykłady

### Podstawowe podświetlanie

To jest ==podświetlony tekst== w zdaniu.

### Podświetlanie w kontekście

W tym zdaniu ==ważne słowa== są podświetlone, aby zwrócić uwagę czytelnika.

### Podświetlanie z innym formatowaniem

Możesz łączyć podświetlanie z **pogrubieniem** i ==podświetleniem== razem.

Możesz również używać ==*podświetlenia z kursywą*==.

### Podświetlanie w listach

- Pierwszy punkt z ==ważnym fragmentem==
- Drugi punkt bez podświetlenia
- Trzeci punkt z ==innym podświetleniem==

### Podświetlanie w tabelach

| Kolumna 1 | Kolumna 2 |
|-----------|-----------|
| Normalny tekst | ==Podświetlony tekst== |
| Kolejny tekst | ==Inny podświetlony tekst== |

### Podświetlanie w kodzie inline

Możesz używać `==podświetlenia==` obok `kodu inline`, ale podświetlanie nie działa wewnątrz bloków kodu.

### Podświetlanie w admonitions

!!! note "Notatka z podświetleniem"
    To jest ==ważna informacja== w notatce.

!!! warning "Ostrzeżenie z podświetleniem"
    ==Uwaga!== To jest ostrzeżenie z podświetlonym fragmentem.

## Wskazówki

- Używaj podświetlenia oszczędnie - zbyt dużo podświetlonych fragmentów może rozpraszać
- Podświetlanie działa dobrze w połączeniu z innym formatowaniem
- Nie używaj podświetlenia wewnątrz bloków kodu - użyj komentarzy zamiast tego
- Podświetlanie jest szczególnie przydatne do wyróżniania kluczowych informacji w długich tekstach

