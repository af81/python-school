# 📒 Block 4 - Übungen

## 1. Begrüssung 🤚🏻

Schreibe eine Funktion `begruessung(name)`, die einen **String-Parameter** `name` entgegennimmt und eine Begrüssungsnachricht ausgibt.
Die Funktion soll **keinen Rückgabewert** liefern (`None`).

- Wenn der Name `"Max"` übergeben wird, soll ausgegeben werden: `Hallo Max! Schön, dass du da bist.`
- Bei jedem anderen Namen soll ausgegeben werden: `Hallo [Name]! Willkommen im Programm.`

---

## 2. Flächenberechnung 📐

Schreibe eine Funktion `berechne_flaeche(breite, hoehe)`, die zwei Fliesskomma-Parameter (float) entgegennimmt und den Flächeninhalt eines Rechtecks berechnet.

Die Funktion soll den Flächenwert zurückgeben.

Beispiel-Aufruf:

```python
flaeche = berechne_flaeche(5.0, 3.2)
print(f"Die Fläche beträgt: {flaeche}")
```

---

## 3. Römische Ziffern 🏛️

Schreibe ein Programm, das den Benutzer zur Eingabe einer einzigen römischen Ziffer auffordert (I, V, X, L, C, D, M).
Erstelle eine Funktion roemisch_zu_dezimal(ziffer), die den Dezimalwert der Ziffer zurückgibt:

| Römisch | Dezimal |
| ------- | ------- |
| I       | 1       |
| V       | 5       |
| X       | 10      |
| L       | 50      |
| C       | 100     |
| D       | 500     |
| M       | 1000    |
