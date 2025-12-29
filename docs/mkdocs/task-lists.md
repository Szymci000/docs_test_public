# Listy zadań

Listy zadań (task lists) to specjalny typ listy z checkboxami, które można zaznaczać. Są przydatne do tworzenia list kontrolnych, checklistów i śledzenia postępów.

## Użycie

Listy zadań tworzy się używając składni podobnej do zwykłych list, ale z checkboxami:

````markdown
- [ ] Niezaznaczone zadanie
- [x] Zaznaczone zadanie
- [ ] Kolejne niezaznaczone zadanie
````

## Przykłady

### Podstawowa lista zadań

- [ ] Pierwsze zadanie do wykonania
- [x] Zadanie już ukończone
- [ ] Trzecie zadanie do wykonania
- [x] Czwarte zadanie ukończone

### Lista zadań z podpunktami

- [ ] Główne zadanie
    - [ ] Podzadanie 1
    - [x] Podzadanie 2
    - [ ] Podzadanie 3
- [x] Kolejne główne zadanie

### Lista zadań z formatowaniem

- [ ] Zadanie z **pogrubionym tekstem**
- [x] Zadanie z *kursywą*
- [ ] Zadanie z `kodem inline`
- [x] Zadanie z [linkiem](https://example.com)

### Lista kontrolna przed wdrożeniem

- [ ] Przegląd kodu
- [ ] Testy jednostkowe
- [ ] Testy integracyjne
- [ ] Aktualizacja dokumentacji
- [ ] Deploy na środowisko testowe
- [ ] Testy na środowisku testowym
- [ ] Deploy na produkcję

### Lista zadań z numeracją

1. [ ] Pierwsze zadanie
2. [x] Drugie zadanie
3. [ ] Trzecie zadanie

### Lista zadań z admonitions

- [ ] Zadanie z notatką
    !!! note
        Pamiętaj o sprawdzeniu tego przed kontynuacją.

- [x] Zadanie z ostrzeżeniem
    !!! warning
        To zadanie wymaga szczególnej uwagi.

## Wskazówki

- Używaj list zadań do śledzenia postępów w projektach
- Zaznaczaj zadania jako ukończone używając `[x]`
- Możesz łączyć listy zadań z innymi elementami markdown
- Listy zadań są interaktywne - użytkownicy mogą je zaznaczać w przeglądarce

