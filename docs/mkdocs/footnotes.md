# Przypisy

Przypisy pozwalają na dodawanie dodatkowych informacji, źródeł lub komentarzy do tekstu bez zakłócania głównego przepływu treści. Po najechaniu na odnośnik przypisu wyświetla się tooltip z treścią.
:far_calendar_plus:
## Użycie

Przypisy tworzy się w dwóch krokach:

1. **Odnośnik w tekście** - użyj składni `[^etykieta]`
2. **Definicja przypisu** - na końcu dokumentu lub w dowolnym miejscu użyj `[^etykieta]: Treść przypisu`

````markdown
Tekst z przypisem[^1] i kolejnym przypisem[^custom-label].

[^1]: To jest pierwszy przypis.
[^custom-label]: To jest przypis z własną etykietą.
````

## Przykłady

### Podstawowe przypisy

Tekst z przypisem[^1] i kolejnym przypisem[^2].

[^1]: To jest pierwszy przypis z dodatkowymi informacjami.
[^2]: To jest drugi przypis z innymi szczegółami.

### Przypisy z własnymi etykietami

Możesz używać własnych etykiet dla przypisów[^custom] zamiast numerów[^another-custom].

[^custom]: To jest przypis z własną etykietą "custom".
[^another-custom]: To jest kolejny przypis z własną etykietą.

### Przypisy z formatowaniem

Tekst z przypisem zawierającym formatowanie[^formatted].

[^formatted]: To jest przypis z **pogrubionym tekstem**, *kursywą* i [linkiem](https://example.com).

### Przypisy z listami

Tekst z przypisem zawierającym listę[^list].

[^list]: To jest przypis z listą:
    - Punkt pierwszy
    - Punkt drugi
    - Punkt trzeci

### Przypisy z kodem

Tekst z przypisem zawierającym kod[^code].

[^code]: To jest przypis z przykładem kodu: `const x = 1;`

### Wiele przypisów w jednym miejscu

Tekst z wieloma przypisami[^first][^second][^third].

[^first]: Pierwszy przypis.
[^second]: Drugi przypis.
[^third]: Trzeci przypis.

### Przypisy wielokrotnego użycia

Możesz użyć tego samego przypisu wielokrotnie[^reuse] w różnych miejscach[^reuse].

[^reuse]: Ten przypis jest używany dwukrotnie.

## Tooltips

Po najechaniu myszką na odnośnik przypisu wyświetla się tooltip z treścią przypisu. To pozwala na szybki podgląd bez konieczności przewijania do końca dokumentu.

## Wskazówki

- Używaj przypisów do dodawania dodatkowych informacji bez zakłócania głównego tekstu
- Przypisy są automatycznie numerowane, jeśli nie używasz własnych etykiet
- Definicje przypisów mogą być umieszczone w dowolnym miejscu dokumentu
- Możesz używać tego samego przypisu wielokrotnie w różnych miejscach tekstu
- Przypisy mogą zawierać formatowanie markdown

