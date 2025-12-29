# Bloki kodu

Bloki kodu pozwalają na wyświetlanie kodu źródłowego z podświetlaniem składni, numeracją linii i dodatkowymi funkcjami jak kopiowanie czy adnotacje.

## Użycie

Podstawowy blok kodu z podświetlaniem składni:

````markdown
```python
def hello_world():
    print("Hello, World!")
    return True
```
````

## Przykłady

### Podstawowy blok kodu

```python
def hello_world():
    print("Hello, World!")
    return True
```

### Blok kodu z numeracją linii

````markdown
```python linenums="1"
def calculate_sum(a, b):
    result = a + b
    return result
```
````

```python linenums="1"
def calculate_sum(a, b):
    result = a + b
    return result
```

### Blok kodu z wyróżnionymi liniami

````markdown
```python hl_lines="2 4"
def process_data(data):
    cleaned = data.strip()  # Wyróżniona linia
    if cleaned:
        return cleaned.upper()  # Wyróżniona linia
    return None
```
````

```python hl_lines="2 4"
def process_data(data):
    cleaned = data.strip()  # Wyróżniona linia
    if cleaned:
        return cleaned.upper()  # Wyróżniona linia
    return None
```

### Blok kodu z adnotacjami

````markdown
```python
def example():
    x = 1  # (1)
    y = 2  # (2)
    return x + y  # (3)
```

1.  Pierwsza zmienna
2.  Druga zmienna
3.  Zwracana suma
````

```python
def example():
    x = 1  # (1)
    y = 2  # (2)
    return x + y  # (3)
```

1.  Pierwsza zmienna
2.  Druga zmienna
3.  Zwracana suma

### Różne języki programowania

````markdown
```javascript
const greeting = "Hello";
console.log(greeting);
```

```html
<div class="container">
    <p>Hello World</p>
</div>
```

```css
.container {
    padding: 20px;
    margin: 0 auto;
}
```
````

```javascript
const greeting = "Hello";
console.log(greeting);
```

```html
<div class="container">
    <p>Hello World</p>
</div>
```

```css
.container {
    padding: 20px;
    margin: 0 auto;
}
```

## Funkcje bloków kodu

- **Podświetlanie składni** - automatyczne rozpoznawanie języka
- **Numeracja linii** - opcjonalna numeracja dla łatwiejszego odniesienia
- **Kopiowanie** - przycisk do kopiowania kodu
- **Adnotacje** - możliwość dodania komentarzy do konkretnych linii
- **Wyróżnianie linii** - podświetlanie wybranych linii

