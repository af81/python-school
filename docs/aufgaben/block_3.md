# 📒 Block 3 - Übungen

## 1. Eine einfache Liste erstellen

Erstelle eine Liste `fruits` mit den Elementen `"Apfel"`, `"Banane"` und `"Orange"`.
Gib die Liste auf dem Bildschirm aus.

---

## 2. Verschiedene Datentypen

Erstelle eine Liste `student`, die folgende Informationen enthält:

- Name: `"Max"`
- Alter: `21`
- Studienfach: `"Informatik"`
- Eine weitere Liste mit den Noten `[1.7, 2.0, 1.3]`

Gib die gesamte Liste aus.

---

## 3. Elemente abrufen

Gegeben ist die Liste:

```python
languages = ['Python', 'Java', 'C++', 'Swift']
```

1. Gib das erste und das letzte Element aus.
2. Gib das zweite Element von hinten aus.

---

## 4. Slicing

Gegeben ist:

```python
letters = ['p', 'r', 'o', 'g', 'r', 'a', 'm']
```

1. Gib nur die Buchstaben von Index 2 bis 5 aus.
2. Gib alle Buchstaben außer die letzten drei aus.
3. Gib mit Slicing die gesamte Liste aus.

---

## 5. Elemente hinzufügen

Erstelle eine Liste `animals = ['Hund', 'Katze']`.

1. Füge "Maus" am Ende hinzu.
2. Füge "Vogel" an Index 1 ein.
3. Gib die aktualisierte Liste aus.

---

## 6. Listen erweitern

Gegeben sind:

```python
numbers = [1, 2, 3]
even = [4, 6, 8]
```

Füge alle Elemente von even an numbers an (Tipp: extend()).

Erwartete Ausgabe:

```python
[1, 2, 3, 4, 6, 8]
```

---

## 7. Elemente ändern

Gegeben ist:

```python
colors = ['Rot', 'Grün', 'Blau']
```

1. Ändere das erste Element zu "Gelb".
2. Ändere das letzte Element zu "Violett".
3. Gib die neue Liste aus.

---

## 8. Elemente entfernen

Gegeben ist:

```python
numbers = [2, 4, 6, 8, 10]
```

1. Entferne die Zahl 6 mit remove().
2. Entferne das erste Element mit del.
3. Gib die Liste nach jedem Schritt aus.

---

## 9. Länge einer Liste

Gegeben ist:

```python
cities = ['Berlin', 'Paris', 'Rom', 'Madrid', 'Oslo']
```

1. Gib mit len() die Anzahl der Städte aus.
2. Füge "Wien" hinzu und gib die neue Länge aus.

---

## 10. Schleifen mit Listen

Erstelle eine Liste `names = ['Anna', 'Ben', 'Clara']`
und gib jedes Element in einer `for`-Schleife mit dem Zusatz `"ist anwesend"` aus.

Beispielausgabe:

```python
Anna ist anwesend
Ben ist anwesend
Clara ist anwesend
```

---

## 11. Kombination von Listenoperationen

1. Erstelle eine leere Liste `numbers`.
2. Füge mit `append()` die Zahlen 1 bis 5 hinzu.
3. Ersetze das dritte Element durch die Zahl `99`.
4. Entferne das erste Element.
5. Gib die fertige Liste aus.

---

## 12. Lieblingsfilme 🎬🍿

Erstelle eine Liste mit den Lieblingsfilmen deiner Freunde.

1. Sortiere sie alphabetisch.
2. Gib nur die ersten drei Filme aus.
3. Gib danach die gesamte Liste rückwärts aus.

---

## 13. Die Inventarliste des Abenteurers 🤠👑

**Geschichte**: Du bist ein Abenteurer, der eine Höhle voller Schätze durchsucht hat. Du möchtest eine Liste der gefundenen Gegenstände führen, um sicherzustellen, dass nichts verloren geht.

**Aufgabe**:

- Schreibe ein Programm, das eine Liste erstellt, um die Namen der Gegenstände zu speichern.
- Lasse den Benutzer 5 Gegenstände eingeben, die er gefunden hat.
- Zeige danach die Liste der Gegenstände an.
- Füge eine Funktion hinzu, die nach einem Gegenstand sucht (der Benutzer gibt den Namen ein) und mitteilt, ob der Gegenstand in der Liste vorhanden ist oder nicht.

**Erweiterung**:

- Ermögliche es dem Benutzer, einen Gegenstand aus der Liste zu entfernen.
- Sortiere die Liste alphabetisch und zeige sie neu an.

---

## 14. Das Punktesystem der Zaubererakademie 🧙🏼‍♀️🪄

**Geschichte**: Du bist ein Lehrer an einer Zaubererakademie. Deine Schüler haben eine Prüfung in Magie abgelegt, und du möchtest die Punkte der Schüler analysieren.

**Aufgabe**:

Erstelle eine Liste, um die Punkte von 10 Schülern zu speichern (die Punkte können vom Benutzer eingegeben werden oder zufällig generiert werden).

Zeige folgende Informationen an:

-Die höchsten und niedrigsten Punkte.
- Den Durchschnitt aller Punkte.
- Die Anzahl der Schüler, die den Test bestanden haben (z.B. Punkte >= 50).

**Erweiterung**:

- Füge die Möglichkeit hinzu, die Punkte eines bestimmten Schülers zu aktualisieren.
- Sortiere die Punkte der Schüler in absteigender Reihenfolge und zeige die Liste an.

---

## 15. Die Bestandsverwaltung eines Lagerhauses 🏭📦

**Geschichte**: Du bist für die Bestandsverwaltung eines grossen Lagerhauses verantwortlich. Das Lagerhaus hat drei Bereiche, und jeder Bereich enthält fünf verschiedene Artikeltypen. Dein Ziel ist es, den Bestand aller Artikel effizient zu verwalten.

**Aufgabe**:

- Erstelle eine zweidimensionale Liste, um die Bestände der Artikel zu speichern.
- Die Zeilen repräsentieren die Bereiche im Lagerhaus.
- Die Spalten repräsentieren die Artikeltypen in jedem Bereich.
- Initialisiere das Array mit zufälligen Bestandswerten (zwischen 0 und 100).
- Zeige den gesamten Bestand in tabellarischer Form an.
- Ermögliche es dem Benutzer, den Bestand eines spezifischen Artikels in einem bestimmten Bereich zu aktualisieren.
- Berechne die Gesamtanzahl aller Artikel im Lagerhaus.

**Erweiterung**:

- Füge eine Funktion hinzu, um den Bestand eines gesamten Bereichs zurückzusetzen (z. B. nach einer Inventur).
- Ermittle den Bereich mit den meisten Artikeln.
