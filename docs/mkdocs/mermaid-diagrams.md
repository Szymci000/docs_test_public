# Diagramy Mermaid

Mermaid to narzędzie do tworzenia diagramów i wykresów używając prostego tekstu. System dokumentacji wspiera diagramy Mermaid, które są automatycznie renderowane.

## Użycie

Diagramy Mermaid tworzy się używając bloku kodu z etykietą `mermaid`:

````markdown
```mermaid
graph TD
    A[Start] --> B{Decyzja}
    B -->|Tak| C[Akcja 1]
    B -->|Nie| D[Akcja 2]
    C --> E[Koniec]
    D --> E
```
````

## Przykłady

### Diagram przepływu (Flowchart)

```mermaid
graph TD
    A[Start] --> B{Decyzja}
    B -->|Tak| C[Akcja 1]
    B -->|Nie| D[Akcja 2]
    C --> E[Koniec]
    D --> E
```

### Diagram sekwencji (Sequence)

```mermaid
sequenceDiagram
    participant U as Użytkownik
    participant S as Serwer
    participant D as Baza danych
    
    U->>S: Żądanie logowania
    S->>D: Sprawdź dane
    D-->>S: Zwróć wynik
    S-->>U: Odpowiedź
```

### Diagram stanów (State)

```mermaid
stateDiagram-v2
    [*] --> Nowy
    Nowy --> W_trakcie: Rozpocznij
    W_trakcie --> Zakończony: Ukończ
    W_trakcie --> Anulowany: Anuluj
    Zakończony --> [*]
    Anulowany --> [*]
```

### Diagram klas (Class)

```mermaid
classDiagram
    class Użytkownik {
        +String imię
        +String email
        +loguj()
        +wyloguj()
    }
    class Zamówienie {
        +int id
        +Date data
        +utwórz()
        +anuluj()
    }
    Użytkownik "1" --> "*" Zamówienie
```

### Diagram Gantta (Gantt)

```mermaid
gantt
    title Harmonogram projektu
    dateFormat YYYY-MM-DD
    section Faza 1
    Zadanie 1 :a1, 2024-01-01, 30d
    Zadanie 2 :a2, after a1, 20d
    section Faza 2
    Zadanie 3 :a3, 2024-02-01, 25d
    Zadanie 4 :a4, after a3, 15d
```

### Diagram ER (Entity Relationship)

```mermaid
erDiagram
    UŻYTKOWNIK ||--o{ ZAMÓWIENIE : składa
    ZAMÓWIENIE ||--|{ POZYCJA : zawiera
    PRODUKT ||--o{ POZYCJA : jest_w
    
    UŻYTKOWNIK {
        int id
        string imię
        string email
    }
    ZAMÓWIENIE {
        int id
        date data
        float suma
    }
    PRODUKT {
        int id
        string nazwa
        float cena
    }
```

### Diagram pie chart (Pie)

```mermaid
pie title Rozkład czasu pracy
    "Kodowanie" : 40
    "Testy" : 25
    "Dokumentacja" : 20
    "Spotkania" : 15
```

### Diagram git graph (Git)

```mermaid
gitgraph
    commit id: "Initial"
    branch develop
    checkout develop
    commit id: "Feature A"
    commit id: "Feature B"
    checkout main
    merge develop
    commit id: "Release"
```

### Diagram użytkownika (User Journey)

```mermaid
journey
    title Proces zakupu
    section Przeglądanie
      Przeglądanie produktów: 5: Użytkownik
      Dodanie do koszyka: 4: Użytkownik
    section Zakup
      Logowanie: 3: Użytkownik
      Płatność: 5: Użytkownik
    section Dostawa
      Oczekiwanie: 2: Użytkownik
      Otrzymanie: 5: Użytkownik
```

## Typy diagramów

- **Flowchart** - diagramy przepływu
- **Sequence** - diagramy sekwencji
- **State** - diagramy stanów
- **Class** - diagramy klas
- **Gantt** - harmonogramy
- **ER** - diagramy relacji encji
- **Pie** - wykresy kołowe
- **Git** - wykresy git
- **Journey** - podróże użytkownika

## Wskazówki

- Diagramy Mermaid są renderowane automatycznie
- Możesz używać różnych typów diagramów w jednym dokumencie
- Diagramy są interaktywne i można je powiększać
- Składnia Mermaid jest prosta i czytelna
- Diagramy są przydatne do wizualizacji procesów i struktur

