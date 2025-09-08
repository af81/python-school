# 🧮 Rechnen

## Grundrechenarten

Die vier mathematischen Grundrechenarten **Addition** (+), **Substraktion** (-), **Multiplikation** (*) und **Division** (/) sind auch in Python möglich.

```python
print(5 + 8)        # 13

print(5 - 3)        # 2

print (3 + 2.0)     # 5.0   Wenn ein Element in einer Rechnung ein Float ist, wird das Ergebnis auch immer ein Float

print(5 * 80)       # 400

print (6 / 2)       # 3.0   Bei / kommt immer ein Float raus

print (6 / 4)       # 1.5

print (6 // 4)      # 1     Das ist die sogenannte Integer-Division, bei der die Nachkommastellen einfach weggelassen werden
```

---

## Runden

Um Float-Zahlen zu runden, braucht man die Funktion `round(x, y)`. Für **x** setzt man die zu rundende Zahl ein, für **y** die Anzahl Nachkommastellen.

```python
number = 3.5 / 1.2   # 2.916666666666667

round(number, 2)     # 2.91     number wird auf 2 Nachkommastellen gerundet
```

## Inkrementieren und Dekrementieren

Wenn du den Werte einer Variable um 1 erhöhen bzw. verringern möchtest, bezeichnet man das als **Inkrementieren bzw. Dekrementieren**.

```python
number = 18

number += 1     # 19    number wird um den Wert 1 erhöht
number -= 1     # 17    number wird um den Wert 1 verringert
```

Man kann den Wert statt um 1 auch um einen **beliebigen Wert** erhöhen bzw. verringern.

```python
number = 18

number += 2     # 20    number wird um den Wert 2 erhöht
number -= 8     # 10    number wird um den Wert 8 verringert
```

## Potenzieren

Beim Potenzieren wird eine Zahl n-mal mit sich selbst multipliziert.

```python
print(2 ** 5)     # 32  Entspricht 2`5. Hier wird also 2 * 2 * 2 * 2 * 2 gerechnet
```

## Integer-Division und Modulo

Wenn das Ergebnis einer Divison keine Gannzahl ergibt (z.B. 1.5), dann können wir mit der **Integer-Divison** dafür sorgen, dass das Ergebnis eine Ganzzahl ausgibt und die Stellen nach dem Komman wegschneidet (nicht runden).

```python
print (6 / 4)       # 1.5

print (6 // 4)      # 1     Integer-Division. Die Nachkommastelle wird weggelassen
```

Interessieren wir uns bei einer Division für den **Rest**, dann verwenden wir den **Modulo-Operator** `%`.

```python
print (9 % 3)       # 0     9 / 3 = 3, Rest 0

print (9 % 2)       # 1     9 / 2 = 4, Rest 1

print (5 % 9)       # 5     5 / 9 = 0, Rest 5
```

---

## Coding-Aufgaben "Rechnen"

Löse in Block 1 die **Aufgaben 4, 5 und 6**.

<!-- ### 1. Grundrechenarten

1. Lasse den Benutzer zwei Zahlen eingeben und gib die Ergebnisse für Addition, Subtraktion, Multiplikation und Division aus. Runde die Ergebnisse auf 2 Stellen nach dem Komma.

3. **Wissensfrage:** Was ist der Unterschied zwischen `/` und `//` in Python?

---

## 2. Inkrementieren & Dekrementieren

1. Lege eine Variable `x = 5` an. Erhöhe sie um 1, gib das Ergebnis aus. Erniedrige sie dann um 2 und gib das Ergebnis erneut aus.

---

## 3. Potenzieren, Division & Modulo

1. Ein Protein-Schokoriegel kostet 3.20 Franken. Wie viele Riegel kannst du mit 20 Franken kaufen? Wie viel Geld bleibt übrig? -->
