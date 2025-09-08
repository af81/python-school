# ⚙️ Operatoren

## Vergleichsoperatoren

Mit **Vergleichsoperatoren** könnne wir Werte miteinander vergleichen. Das Ergebnis eines Vergleichs ist ein Wahrheitswert vom Datentyp `bool`, als entweder `True`oder `False`.

<table>
    <tr>
      <th>Operator</th>
      <th>Bedeutung</th>
    </tr>
    <tr>
      <td>a < b</td>
      <td>a kleiner als b</td>
    </tr>
    <tr>
      <td>a <= b</td>
      <td>a kleiner oder gleich b</td>
    </tr>
    <tr>
      <td>a == b</td>
      <td>a gleich b</td>
    </tr>
    <tr>
      <td>a != b</td>
      <td>a ungleich b</td>
    </tr>
    <tr>
      <td>a >= b</td>
      <td>a grösser gleich b</td>
    </tr>
    <tr>
      <td>a > b</td>
      <td>a grösser als b</td>
    </tr>
</table>

Hier ein paar Beispiele:

```python
7.6 > 1             # True, weil 7.6 grösser als 1 ist

34 >= 34            # True, weil 34 grösser oder gleich 34 ist

5 == 7              # False, weil 5 nicht gleich 7 ist

50 != 78            # True, weil 50 ungleich 78 ist

0.5 < 0.3           # False, weil 0.5 nicht kleiner als 0.3 ist
```

Man kann auch **Strings** miteinander vergleichen.

```python
"Password123" == "Password321"  # False, weil die beiden Strings nicht gleich sind

"Juliana" != "Julianna"         # True, weil die beiden Strings ungleich sind
```

---

## Logische Operatoren

Mit **logischen Operatoren** kann man Wahrheitswerte verknüpfen und vergleichen.

### AND

Werden zwei Wahrheitswerte a und b mit einem `and`verküpft, dann ist das Ergebnis genau dann `True`, wenn a UND b beide `True` sind. Ist a oder b (oder beide) `FALSE` ist auch die Verknüpfung `FALSE`.

```python
8 > 5 and 4 != 2        # True, da beide Aussagen (8 > 5 und 4 != 2) True sind

8 > 5 and 4 = 2         # False, da eine Aussage (8 > 5) zwar True, aber die andere (4 = 2) False ist

8 < 5 and 4 = 2          # False, da beide Aussagen (8 < 5 und 4 = 2) False sind
```

### OR

Werden zwei Wahrheitswerte a und b mit einem `or`verküpft, dann ist das Ergebnis `True`, wenn a ODER b (oder beide) `True` sind. Sind beide `FALSE` ist auch die Verknüpfung `FALSE`.

```python
8 > 5 or 4 != 2         # True, da beide Aussagen (8 > 5 und 4 != 2) True sind

8 > 5 or 4 = 2          # True, da mindestens eine Aussage (8 > 5) True ist

8 < 5 or 4 = 2          # False, da beide Aussagen (8 < 5 und 4 = 2) False sind
```

### XOR

Werden zwei Wahrheitswerte a und b mit einem `^`(xor) verküpft, dann ist das Ergebnis `True`, wenn ENTWEDER a ODER b `True` sind, ABER NICHT BEIDE. Sind beide `FALSE` ist auch die Verknüpfung weiterhin `FALSE`.

```python
8 > 5 ^ 4 = 2          # True, da mindestens ein Element (8 > 5) True ist

8 < 5 ^ 4 = 2          # False, da beide Elemente (8 < 5) und (4 = 2) False sind

8 > 5 ^ 4 != 2         # False, da beide Elemente (8 < 5) und (4 = 2) True sind
```

### NOT

Beim Operator `NOT` wird ausnahmsweise nur der Wahrheitswert einer Aussage beurteilt. Und zwar wird hier überprüft, ob die Aussage insgesamt `FALSE` ist.

```python
3 == 3                 # True, da 3 gleich 3 ist

"John" == "John"       # True, da die beiden Strings übereinstimmen

not 3 == 3             # False, da 3 gleich 3 ist, aber negiert wird

not "John" == "Pam"    # True, da John ungleich Pam ist, und dies korrekterweise negiert wird
```

---

## Coding-Aufgaben "Operatoren"

Löse in Block 1 die **Aufgaben 7, 8 und 9**.
