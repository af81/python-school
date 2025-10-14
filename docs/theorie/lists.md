# Listen & Tuples 📋

In Python ermöglichen es uns Listen, mehrere Werte in einer einzigen Variablen zu speichern.
Zum Beispiel: Wenn du das Alter aller Schüler einer Klasse speichern möchtest, kannst du das mit einer Liste tun.

Listen sind ähnlich wie Arrays in anderen Programmiersprachen – dynamische Arrays, die auch Elemente unterschiedlicher Datentypen speichern können.

---

## Eine Python-Liste erstellen

Wir erstellen eine Liste, indem wir die Elemente in eckige Klammern `[]` schreiben und durch Kommas trennen.

```python
# Eine Liste mit drei Elementen
ages = [19, 26, 29]
print(ages)
```

Ausgabe:

```python
[19, 26, 29]
```

Hier hat die Liste `ages` drei Elemente.

---

## Elemente verschiedener Typen in einer Liste

Python-Listen sind sehr flexibel – sie können auch Elemente verschiedener Datentypen enthalten:

```python
# Eine Liste mit Strings, Zahlen und einer weiteren Liste
student = ['Jack', 32, 'Informatik', [2, 4]]
print(student)
```

```python
# Eine leere Liste
empty_list = []
print(empty_list)
```

---

## Eigenschaften von Listen

In Python sind Listen:

- **Geordnet (Ordered)** – Die Reihenfolge der Elemente bleibt erhalten.
- **Veränderbar (Mutable)** – Elemente können nach der Erstellung geändert werden.
- **Duplikate erlaubt (Allow duplicates)** – Eine Liste kann doppelte Werte enthalten.

---

## Zugriff auf Listenelemente

Jedes Element in einer Liste hat einen Index, der bei 0 beginnt.

| Element | Index |
| ------- | ----- |
| Erstes  | 0     |
| Zweites | 1     |
| Drittes | 2     |

Beispiel:

```python
languages = ['Python', 'Swift', 'C++']

# Erstes Element
print('languages[0] =', languages[0])

# Drittes Element
print('languages[2] =', languages[2])
```

Ausgabe:

```python
languages[0] = Python
languages[2] = C++
```

---

## Negative Indizes

Listen unterstützen auch negative Indizes.
Das letzte Element hat den Index -1, das vorletzte -2 usw.

```python
languages = ['Python', 'Swift', 'C++']

# Letztes Element
print('languages[-1] =', languages[-1])

# Drittes Element von hinten
print('languages[-3] =', languages[-3])
```

Ausgabe:

```python
languages[-1] = C++
languages[-3] = Python
```

---

## Slicing (Teillisten)

Um einen Teil einer Liste zu erhalten, verwenden wir den Slicing-Operator :.

```python
my_list = ['p', 'r', 'o', 'g', 'r', 'a', 'm']
print("my_list =", my_list)

# Elemente von Index 2 bis 4 (5 ist ausgeschlossen)
print("my_list[2:5] =", my_list[2:5])

# Elemente von Index 2 bis -2
print("my_list[2:-2] =", my_list[2:-2])

# Elemente von Index 0 bis 2
print("my_list[0:3] =", my_list[0:3])
```

Ausgabe:

```python
my_list[2:5] = ['o', 'g', 'r']
my_list[2:-2] = ['o', 'g', 'r']
my_list[0:3] = ['p', 'r', 'o']
```

---

## Start- und Endindex weglassen

Wenn du den Startindex weglässt, beginnt das Slicing am Anfang der Liste.
Wenn du den Endindex weglässt, läuft es bis zum Ende.

```python
my_list = ['p', 'r', 'o', 'g', 'r', 'a', 'm']

# Ab Index 5 bis zum Ende
print("my_list[5:] =", my_list[5:])

# Vom Anfang bis Index -4
print("my_list[:-4] =", my_list[:-4])

# Beide weggelassen → komplette Liste
print("my_list[:] =", my_list[:])
```

Ausgabe:

```python
my_list[5:] = ['a', 'm']
my_list[:-4] = ['p', 'r', 'o']
my_list[:] = ['p', 'r', 'o', 'g', 'r', 'a', 'm']
```

> Hinweis: Wenn du auf einen Index zugreifst, der nicht existiert, löst Python einen IndexError aus.

---

## Elemente zu einer Liste hinzufügen

Listen sind veränderbar, d. h. du kannst sie nachträglich ändern.

Am Ende hinzufügen mit `append()`

```python
fruits = ['apple', 'banana', 'orange']
print('Originale Liste:', fruits)

fruits.append('cherry')
print('Aktualisierte Liste:', fruits)
```

Ausgabe:

```python
Originale Liste: ['apple', 'banana', 'orange']
Aktualisierte Liste: ['apple', 'banana', 'orange', 'cherry']
```

An bestimmter Position einfügen mit `insert()`

```python
fruits = ['apple', 'banana', 'orange']
print("Originale Liste:", fruits)

fruits.insert(2, 'cherry')
print("Aktualisierte Liste:", fruits)
```

Ausgabe:

```python
Originale Liste: ['apple', 'banana', 'orange']
Aktualisierte Liste: ['apple', 'banana', 'cherry', 'orange']
```

Elemente aus anderen Iterables hinzufügen mit `extend()`

```python
numbers = [1, 3, 5]
even_numbers = [2, 4, 6]

# Elemente von even_numbers an numbers anhängen
numbers.extend(even_numbers)
print('Aktualisierte Liste:', numbers)
```

Ausgabe:

```python
Aktualisierte Liste: [1, 3, 5, 2, 4, 6]
```

---

## Elemente ändern

```python
colors = ['Red', 'Black', 'Green']
print('Originale Liste:', colors)

# Erstes Element ändern
colors[0] = 'Purple'

# Drittes Element ändern
colors[2] = 'Blue'

print('Aktualisierte Liste:', colors)
```


Ausgabe:

```python
Originale Liste: ['Red', 'Black', 'Green']
Aktualisierte Liste: ['Purple', 'Black', 'Blue']
```

---

## Elemente entfernen

Nach Wert löschen mit `remove()`

```python
numbers = [2, 4, 7, 9]
numbers.remove(4)
print(numbers)
```

Ausgabe:

```python
[2, 7, 9]
```

Nach Index oder Bereich löschen mit `del`

```python
names = ['John', 'Eva', 'Laura', 'Nick', 'Jack']

# Element an Index 1 löschen
del names[1]
print(names)

# Elemente von Index 1 bis 2 löschen
del names[1:3]
print(names)

# Ganze Liste löschen
del names
```

Ausgabe:

```python
['John', 'Laura', 'Nick', 'Jack']
['John', 'Jack']
NameError: name 'names' is not defined
```

---

## Länge einer Liste

Mit der Funktion `len()` kannst du die Anzahl der Elemente ermitteln:

```python
cars = ['BMW', 'Mercedes', 'Tesla']
print('Gesamtanzahl:', len(cars))
```

Ausgabe:

```python
Gesamtanzahl: 3
```

---

## Durch eine Liste iterieren

```python
fruits = ['apple', 'banana', 'orange']

for fruit in fruits:
    print(fruit)
```

Ausgabe:

```python
apple
banana
orange
```

---

## Wichtige Methoden von Python-Listen

| Methode     | Beschreibung                                                |
| ----------- | ----------------------------------------------------------- |
| `append()`  | Fügt ein Element am Ende hinzu                              |
| `extend()`  | Hängt mehrere Elemente (aus z. B. einer anderen Liste) an   |
| `insert()`  | Fügt ein Element an einer bestimmten Position ein           |
| `remove()`  | Entfernt das erste Vorkommen eines Werts                    |
| `pop()`     | Gibt ein Element zurück und entfernt es anhand seines Index |
| `clear()`   | Löscht alle Elemente aus der Liste                          |
| `index()`   | Gibt den Index des ersten Vorkommens eines Werts zurück     |
| `count()`   | Zählt, wie oft ein bestimmtes Element vorkommt              |
| `sort()`    | Sortiert die Liste auf- oder absteigend                     |
| `reverse()` | Kehrt die Reihenfolge der Elemente um                       |
| `copy()`    | Erstellt eine flache Kopie der Liste                        |

---

## Weiterführende Themen

- list() – Konvertiert andere Datentypen in eine Liste
- List Comprehension – Eine kompakte Art, Listen zu erstellen
- enumerate() – Fügt beim Iterieren einen Zähler hinzu

---

## Unterschied zu Tuples

Neben **Listen** gibt es in Python auch **Tuples** (auf Deutsch: *Tupel*).
Sie ähneln Listen sehr stark, haben aber einen wichtigen Unterschied:

> 🔒 **Tuples sind unveränderlich (immutable)** — einmal erstellt, können ihre Elemente **nicht geändert, hinzugefügt oder entfernt** werden.

---

## Erstellung eines Tuples

Ein Tuple wird mit **runden Klammern `()`** erstellt:

```python
# Ein Tuple mit drei Elementen
numbers = (10, 20, 30)
print(numbers)
```

Ausgabe:

```python
(10, 20, 30)
```

Ein Tuple kann – genau wie eine Liste – auch verschiedene Datentypen enthalten:

```python
student = ('Lisa', 23, 'Biologie', [1.3, 1.7])
print(student)
```

---

## Zugriff auf Tuple-Elemente

Der Zugriff funktioniert genauso wie bei Listen über den Index:

```python
languages = ('Python', 'Java', 'C++')

print(languages[0])   # Erstes Element
print(languages[-1])  # Letztes Element
```

Ausgabe:

```python
Python
C++
```

---

## Länge eines Tuples

Auch hier kannst du mit `len()` die Anzahl der Elemente bestimmen:

```python
animals = ('Hund', 'Katze', 'Vogel')
print(len(animals))
```

Ausgabe:

```python
3
```

---

## Versuch, ein Tuple zu ändern

Tuples sind unveränderlich – jede Änderung führt zu einem **Fehler**:

```python
colors = ('Rot', 'Grün', 'Blau')
colors[0] = 'Gelb'   # ❌ Fehler!
```

Ausgabe:

```python
TypeError: 'tuple' object does not support item assignment
```

---

## Warum Tuples verwenden?

Tuples sind nützlich, wenn du feste Daten speichern möchtest, die sich nicht ändern sollen, z. B.:

- Wochentage
- Koordinaten (x, y)
- Konstanten-Werte

Beispiel:

```python
days = ('Montag', 'Dienstag', 'Mittwoch', 'Donnerstag', 'Freitag')
```

---

## Vergleich: Liste vs. Tuple

| Eigenschaft           | Liste (`list`)         | Tuple (`tuple`) |
| --------------------- | ---------------------- | --------------- |
| Klammern              | `[]`                   | `()`            |
| Veränderbar           | ✅ Ja                   | ❌ Nein          |
| Geschwindigkeit       | Etwas langsamer        | Etwas schneller |
| Typisch verwendet für | Daten, die sich ändern | Feste Daten     |


💡 Merke:
- Wenn du Daten speichern willst, die sich nicht ändern dürfen, verwende ein **Tuple**.
- Wenn du Daten bearbeiten, hinzufügen oder löschen möchtest, verwende eine **Liste**.
