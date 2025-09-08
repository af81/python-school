# 🧮 Variablen & Datentypen

## Wert einer Variable zuweisen

Ohne Variablen kommt kein Programm aus. Variablen dienen als **Datenspeicher** und werden während der Ausführung des Programms im Arbeitsspeicher (RAM) abgelegt. Hier ein Beispiel:

```python
number = 18
```

Links steht der Variablenname `number`. Diese Variable speicher den Wert `10`.

Ein zweites Beispiel:

```python
modul_name = "Applikationen entwerfen und implementieren"
```

Hier speichert die Variable `modul_name` den Wert `Applikationen entwerfen und implementieren`.

Ich kann auch **Werte an mehrere Variablen** auf einmal vergeben.

```python
a, b, c = 5, 3.2, "Hello"

print(a) # prints 5
print(b) # prints 3.2
print(c) # prints Hello
```

---

## Variablennamen

Beachte, dass Variablen mit einem **Kleinbuchstaben** beginnen, zusammengesetzte Begriffe mit einem `_` verbunden werden und keine Sonderzeichen enthalten dürfen.

<table>
    <tr>
      <th>✅ Erlaubt</th>
      <th>⛔️ Nicht erlaubt</th>
    </tr>
    <tr>
      <td>number</td>
      <td>Number</td>
    </tr>
    <tr>
      <td>h4acker</td>
      <td>8ung</td>
    </tr>
    <tr>
      <td>first_name</td>
      <td>first-name</td>
    </tr>
    <tr>
      <td>speed_in_percent</td>
      <td>speedin%</td>
    </tr>
</table>

---

## Datentypen

In Python ist es nicht nötig, den Variablen einen **festen Datentyp** zu zuzuweisen. Es wird automatisch erkannt, ob der gespeicherte Wert eine **Zahl** (Integer oder Float), eine **Zeichenkette** (String) oder ein **Wahrheitswert** (Boolean) ist.

Folgende **Datentypen** solltest du kennen:

<table>
    <tr>
      <th>Typ 🇩🇪</th>
      <th>Typ 🇬🇧</th>
      <th>Kurzschreibweise</th>
      <th>Beispiele</th>
    </tr>
    <tr>
      <td>Zeichenkette</td>
      <td>String</td>
      <td>str</td>
      <td>"Hallo", "abc123", "0.62", "Mein Name"</td>
    </tr>
    <tr>
      <td>Ganzzahlen</td>
      <td>Integer</td>
      <td>int</td>
      <td>-5, -3, 0, 8, 54</td>
    </tr>
    <tr>
      <td>Fliesskommazahlen</td>
      <td>Float</td>
      <td>float</td>
      <td>-1.25, -1.0, 0.0, 7.6543</td>
    </tr>
    <tr>
      <td>Wahrheitswerte</td>
      <td>Boolean</td>
      <td>bool</td>
      <td>True, False</td>
    </tr>
</table>

Um den Datentyp einer Variable herauszufinden, kannst du die **Funktion** `type` verwenden.

```python
name = "Naruto"
type(name) # <class 'str', also String

age = 16
type(age) # <class 'int', also Integer

hero = True
type(hero) # <class 'bool', also Boolean
```

> 🤓 Um lange Ganzzahlen wie z.B. 1000000 besser lesen zu können, kann man `_` verwenden. Z.B. 1_000_000. Der Wert ändert sich dadurch nicht.

---

## Konvertieren - Benutzereingabe mit input()

Es ist wichtig zu wissen, dass der **input()-Befehl** immer einen *Zeichenkette* (String) einliest. Selbst wenn die Eingabe eine *Ganzzahl* (Integer), z.B. 16, ist.

```python
# using input() to take user input
age = input("Wie alt bist du? [in Jahren]: ")

# print age
print("Dein Alter: ", age)

# investigate data type of age
print ("Datentyp der Variable age: ", type(age))
```

Damit wir mit der Variable *age* rechnen können, müssen wir sie zuerst in einen Zahlentyp wie Integer oder Float **konvertieren (umwandeln)**. Das machen wir mithilfe der **int()-** oder **float()-Funktion**.

```python
age = int(input("Wie alt bist du? [in Jahren]: "))
```

Hier wird der der Datentyp der Benutzereingabe von String zu Integer konvertiert.

---

## String-Operationen

Es gibt verschiedene Möglichkeiten Strings umzuformen, zu verkürzen und oder sie zusammenzusetzen.

### Index einer Zeichenkette

Als erstes ist es aber wichtig, dass wir verstehen, wie eine Zeichenkette aufgebaut ist. Schaue dir dazu die **Position der Buchstaben** im String `HACKER` an.

![](../img/hacker.png)

In der Informatik beginnen wir stets **bei 0** mit zählen. Der String `HACKER`besteht aus 6 Zeichen, wobei das `H` die Position 0 und das `R` die Position 5 hat. Im Englischen verwendet man statt Position den Begriff **Index.**

### Substrings

Einzelne Zeichen oder Substrings kannst du mithilfe eckiger Klammern `[]` und dem Index auslesen.

```python
text = "HACKER"

text[3] # K
```

Du kannst auch mehre Zeichen aus einem String ausschneiden (*slicing*), indem du den *3* und den **Endindex** angibts.

> ⚠️ Achtung: Der Endindex ist nicht mehr im Slice enthalten.

Um `ACK`aus dem String `HACKER`auszuschneiden, gibt man also den Index von `A`und `E`(eins mehr als K) an und setzt einen **Doppelpunkt** dazwischen.

```python
text = "HACKER"

text[1:4] # ACK
```

### Zeilenumbruch

Einen **Zeilumbruch** erzeugst du mit `\n`. Das steht für *new Line*.

```python
text = "Erste Zeile.\nZweite Zeile."

print[text]

# Output:
# Erste Zeile.
# Zweite Zeile.
```

### Anführungszeichen innerhalb eines Strings

Willst du innerhalb eines Strings **Anführungszeichen** nutzen, ohne einen Fehler zu erzeugen, brauchst du das Markierungszeichen `\"`.

```python
text = "Der \"FCL\" ist mein Lieblingsclub."    # Der "FCL" ist mein Lieblingsclub.
```

### Länge eines Strings

Um die Länge eines Strings zu ermitteln, brauchst du die Funktion `len()`.

```python
text = "Gorilla"
len(text)   # 6
```

Um den Index des Buchstabens `r` in Gorilla zu ermitteln, nimmst du die Funktion `.index()`.

```python
text = "Gorilla"
print(text.index("r"))  # 2
```

### Strings zusammensetzen

Um Strings zusammenzusetzen, kann man sie mit `+` addieren.

```python
print("Hello" + " World" + "!")     # Hello World!
```

Man kann auch String-Variablen zusammensetzen.

```python
text1 = "Hello"
text2 = "World!"

print(text1 + " " + text2)     # Hello World!
```

Um Variablen aller Typen in einem String einzubinden, schreibt man ein `f` vor den String und setzt die Variable in geschweifte Klammern `{}`.

```python
name = "Kim"
language = "Python"

print(f"My name is {name} and I am learning {language}.")

# My name is Kim and I am learning Python.
```

### Gross- und Kleinbuchstaben

Um Strings komplett in **Gross- oder Kleinbuchstaben** zu transformieren, stehen die Funktionen `upper()` und `lower()` zur Verfügung.

```python
name = "Ringo"

print(name.upper())     # RINGO
print(name.lower())     # ringo
```

### Weitere String-Funktionen

Weitere String-Funktionen kannst du in der offiziellen Python-Dokumentation nachlesen:

[https://docs.python.org/3/library/string.html](https://docs.python.org/3/library/string.html)

---

## Coding-Aufgaben "Variablen"

Lösen in Block 1 die **Aufgaben 1, 2 und 3**.

<!-- Erstelle ein Projekt und Repo ([Anleitung](aufgaben/python-repo.md)) mit dem Namen **VarTasks**.

### 1. Einfache Ein- und Ausgabe

1. Schreibe ein Programm, das deinen Namen einliest und ihn mit einer Begrüssung ausgibt.
    - Beispiel: „Hallo Anna! Schön, dass du da bist.“

---

### 2. Variablen & Datentypen

1. Deklariere drei Variablen: eine ganze Zahl, eine Kommazahl und einen Text. Lasse dir jeweils den Datentyp mit `type()` ausgeben.

2. **Wissensfrage:** Was ist der Unterschied zwischen `=` und `==`?

---

### 3. String-Operationen

1. Schreibe ein Programm, das deinen Namen in Grossbuchstaben, Kleinbuchstaben und umgedreht ausgibt.
   Beispiel: `Anna` → `ANNA`, `anna`, `annA`.

2. Lasse den Benutzer zwei weitere Wörter eingeben und verbinde sie zu einem neuen Wort. -->
