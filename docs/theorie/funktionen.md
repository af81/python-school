# 🐍 Python Functions – Einführung

Eine **Funktion** ist ein Block von Code, der eine bestimmte Aufgabe erfüllt.
Funktionen helfen dabei, Programme in kleinere, **verständliche** und **wiederverwendbare** Einheiten zu unterteilen.

Beispiel:
Wenn wir ein Programm schreiben, das einen Kreis erstellt und färbt, können wir dafür zwei Funktionen erstellen:

1. Funktion zum Erstellen des Kreises
2. Funktion zum Färben des Kreises

---

## 1. Eine Funktion erstellen

```python
def greet():
    print('Hello World!')
```

Erläuterung:

- `def` → Schlüsselwort zum Definieren einer Funktion
- `greet()` → Funktionsname
- Alles, was eingerückt ist, gehört zum Funktionskörper

>Hinweis: Python verwendet Einrückungen, um Codeblöcke zu definieren.

---

## 2. Eine Funktion aufrufen

Das Definieren einer Funktion führt sie nicht automatisch aus.
Um die Funktion zu verwenden, muss sie aufgerufen werden:

```python
greet()
print('Outside function')
```

Ausgabe:

```bash
Hello World!
Outside function
```

Ablauf:

1. Die Kontrolle springt zur Funktion `greet()`.
2. Der Code innerhalb der Funktion wird ausgeführt.
3. Die Kontrolle kehrt zurück zum nächsten Befehl nach dem Funktionsaufruf.

---

## 3. Funktionsargumente

Argumente sind Eingabewerte, die an die Funktion übergeben werden:

```python
def greet(name):
    print("Hello", name)

greet("John")
greet("David")
```

Ausgabe:

```python
Hello John
Hello David
```

---

## 4. Funktion mit mehreren Parametern

```python
def add_numbers(num1, num2):
    sum = num1 + num2
    print("Sum:", sum)

add_numbers(5, 4)
```

Ausgabe:

```python
Sum: 9
```

---

## 5. Rückgabewert mit `return`

Mit `return` kann eine Funktion einen Wert zurückgeben:

```python
def find_square(num):
    result = num * num
    return result

square = find_square(3)
print("Square:", square)
```

Ausgabe:

```python
Square: 9
```

> Hinweis: Alles nach return wird nicht mehr ausgeführt, die Funktion endet sofort.

---

## 6. Platzhalter-Funktion mit `pass`

Manchmal möchte man Funktionen vorab definieren, ohne dass sie Code enthalten:

```python
def future_function():
    pass

future_function()  # keine Ausgabe, kein Fehler
```

---

## 7. Python-Bibliotheksfunktionen

Python enthält viele eingebaute Funktionen, die direkt genutzt werden können:

- `print()` → gibt Text aus
- `pow(x, y)` → x hoch y
- `sqrt(x)` → Quadratwurzel von x (aus dem Modul math)

Beispiel:

```python
import math

square_root = math.sqrt(4)
print("Square Root of 4 is", square_root)

power = pow(2, 3)
print("2 to the power 3 is", power)
```

Ausgabe:

```python
Square Root of 4 is 2.0
2 to the power 3 is 8
```

> Hinweis: Funktionen aus Modulen wie math müssen zuerst importiert werden.

---

## Zusammenfassung

| Konzept               | Erklärung                                           |
| --------------------- | --------------------------------------------------- |
| `def`                 | Definiert eine Funktion                             |
| Funktionsaufruf       | Führt den Code innerhalb der Funktion aus           |
| Parameter / Argumente | Übergabe von Eingabewerten an die Funktion          |
| `return`              | Rückgabe eines Wertes und Beenden der Funktion      |
| `pass`                | Platzhalter für leeren Funktionskörper              |
| Bibliotheksfunktionen | Vorgefertigte Funktionen aus Modulen (z. B. `math`) |


> Funktionen machen Programme übersichtlicher, wiederverwendbar und leichter wartbar.
