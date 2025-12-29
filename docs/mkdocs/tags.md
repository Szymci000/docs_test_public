# Tagi


Tagi pozwalają na kategoryzowanie i filtrowanie treści w dokumentacji. Używając tagów, możesz grupować powiązane strony i umożliwić użytkownikom szybkie znajdowanie treści na określone tematy.

## Użycie

Tagi są definiowane w frontmatter każdej strony:

````markdown
---
title: "Tytuł strony"
tags:
  - "Tag1"
  - "Tag2"
---
````

Tagi można również automatycznie dodawać do wszystkich stron w katalogu używając pliku `meta.yml`:

````yaml
tags:
  - "Tag1"
  - "Tag2"
````

## Przykłady

### Tagi w frontmatter

Każda strona może mieć własne tagi zdefiniowane w frontmatter:

```yaml
---
title: "Przykładowa strona"
tags:
  - "Dokumentacja"
  - "MkDocs"
  - "Przewodnik"
---
```

### Automatyczne tagi z meta.yml

Plik `meta.yml` w katalogu automatycznie dodaje tagi do wszystkich stron w tym katalogu:

```yaml
tags:
  - "MkDocs"
  - "Dokumentacja"
```

### Filtrowanie po tagach

Używając składni HTML comment z `material/tags` możesz wyświetlić tylko strony z określonym tagiem. 

Składnia wygląda następująco (użyj tego w swoim pliku markdown):


&lt;!-- material/tags { include: ["MkDocs"] } --&gt;


**Przykład:** W pliku `index.md` możesz użyć:

&lt;!-- material/tags { include: ["Panel ENP"] } --&gt;

To wyświetli wszystkie strony z tagiem "Panel ENP" na tej stronie.

**Uwaga:** W powyższych przykładach użyto HTML entities (`&lt;` i `&gt;`) aby pokazać składnię bez przetwarzania. W rzeczywistym użyciu wpisz normalne znaki `<` i `>`.

### Wiele tagów

Strona może mieć wiele tagów:

```yaml
---
tags:
  - "Panel ENP"
  - "CMS"
  - "Przewodnik"
---
```

### Tagi w kategoriach

Różne kategorie mogą mieć różne tagi:

- **Panel ENP** - tag: "Panel ENP"
- **Synerise** - tag: "Synerise"
- **Działania** - tag: "Działania"
- **VPS** - tag: "VPS"
- **MkDocs** - tag: "MkDocs"

## Funkcje tagów

- **Kategoryzacja** - grupowanie powiązanych stron
- **Filtrowanie** - wyświetlanie tylko stron z określonym tagiem
- **Nawigacja** - łatwe znajdowanie treści na określone tematy
- **Automatyzacja** - automatyczne dodawanie tagów przez meta.yml

## Wskazówki

- Używaj spójnych nazw tagów w całej dokumentacji
- Tagi powinny być opisowe i znaczące
- Możesz używać meta.yml do automatycznego dodawania tagów do wszystkich stron w katalogu
- Tagi są przydatne do tworzenia indeksów tematycznych
- Używaj tagów do grupowania powiązanych treści

