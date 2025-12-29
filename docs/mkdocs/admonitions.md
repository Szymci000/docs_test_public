# Admonitions

Admonitions to specjalne bloki służące do wyróżniania ważnych informacji, ostrzeżeń, wskazówek i innych typów treści. Są wizualnie wyróżnione i pomagają czytelnikom szybko zidentyfikować typ informacji.

## Użycie

Admonitions tworzy się używając składni z trzema dwukropkami i typem bloku:

````markdown
!!! note "Tytuł opcjonalny"
    Treść notatki. Może zawierać wiele linii.
    Wszystkie linie muszą być wcięte o 4 spacje.
````

Dostępne typy admonitions:
- `note` - Informacja ogólna
- `tip` - Wskazówka
- `warning` - Ostrzeżenie
- `danger` - Niebezpieczeństwo
- `info` - Informacja dodatkowa

## Przykłady

!!! note "Notatka"
    To jest przykład notatki. Użyj jej do przekazania ogólnych informacji.

!!! tip "Wskazówka"
    To jest przykład wskazówki. Użyj jej do podania pomocnych sugestii.

!!! warning "Ostrzeżenie"
    To jest przykład ostrzeżenia. Użyj go do zwrócenia uwagi na potencjalne problemy.

!!! danger "Niebezpieczeństwo"
    To jest przykład bloku niebezpieczeństwa. Użyj go do ostrzeżenia przed poważnymi konsekwencjami.

!!! info "Informacja"
    To jest przykład informacji dodatkowej. Użyj go do przekazania dodatkowych szczegółów.

## Admonitions bez tytułu

Możesz również używać admonitions bez tytułu:

````markdown
!!! note
    To jest notatka bez tytułu.
````

!!! note
    To jest notatka bez tytułu.

## Zagnieżdżone treści

Admonitions mogą zawierać zagnieżdżone elementy markdown:

````markdown
!!! tip "Wskazówka z listą"
    Oto lista w admonition:
    
    - Punkt pierwszy
    - Punkt drugi
    - Punkt trzeci
    
    I **pogrubiony tekst** również działa.
````

!!! tip "Wskazówka z listą"
    Oto lista w admonition:
    
    - Punkt pierwszy
    - Punkt drugi
    - Punkt trzeci
    
    I **pogrubiony tekst** również działa.

