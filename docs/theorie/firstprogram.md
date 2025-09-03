# 🐍 Erstes Python-Programm schreiben

## 📂 Projektordner und Datei anlegen

Für jedes Programm (bzw. Programmierprojekt) brauchen wir eine **saubere Ordnerstruktur**, die alle wichtigen Dateien (Files) enthält. Die beiden folgenden Varianten zeigen dir, wie man einen Projektordner anlegt.

### **Variante 1:** Über Explorer (Mac: Finder) und VS Code

1. Erstelle an einem Ort deiner Wahl einen **Projektordner** "HelloWorld".
2. Öffne in **VS Code** den Ordner "HelloWorld"
3. Klicke im VS Code Explorer auf **New File** und nenne dieses *hello.py*

### **Variante 2:** Über das Terminal

1. Navigiere über das Terminal zu einem Ort deiner Wahl und erstelle einen **Projektordner** mit `mkdir HelloWorld`
2. Wechsle in diesen Ordner mit `cd HelloWorld`
3. Erstelle darin ein File **hello.py** mit `touch hello.py`
4. Öffne in **VS Code** den Ordner "HelloWorld"

> ⚠️ Es ist wichtig, dass du den Projektordner öffenst und dieser die oberste Ebene im VS Code Explorer bildet. Ansonsten funktioniert das Ausführen der Programme unter Umständen nicht.

---

## 🧑🏼‍💻 HelloWorld - Erster Code

Wir schreiben nun als erstes das übliche *Hello World*-Programm. Dieses hilft Anfängern die grundlegende **Syntax** (Grammatik) einer Programmiersprache zu verstehen.

Klicke in VS Code auf *hello.py* und schreibe folgende Codezeile:

```python
print("Hello World!")
```

Der **Print-Befehl** in Python gibt den Text in der Klammer (*Hello World!*) aus. Text (strings) müssen in Anführungszeichen gesetzt werden.

Starte nun dein Programm mit `python hello.py`(Mac: `python3 hello.py`). Der Output sollte so aussehen:

```bash
Hello World!
```

---

## 💭 Kommentare

Kommentare sind nützlich, um den Code zu **beschreiben** und zu **strukturieren**. Das hilft uns (und anderen) die Übersicht zu behalten und den Zweck eines Code-Blocks zu verstehen.

Das ist besonders wichtig, um...

- unseren Code auch in Zukunft noch zu verstehen
- mit anderen gemeinsam am gleichen Code zu arbeiten
- um Fehler im Code zu finden (debuggen)

> 🤓 Kommentare werden beim Ausführen des Programms übrigens komplett ignoriert.


### Einzeilige Kommentare

Wir brauchen `#`, um einen einzeiligen Kommentar zu schreiben.

```python
# print hello world
print("Hello World!")
```

Wir können einen Kommentar auch rechts neben den Code setzen.

```python
print(18)   # print a number
```

### Mehrzeilige Kommentare

Python hat keine spezielle Methode für mehrzeilige Kommentare wie etwas C#, PHP oder Java.

Wir können aber denselben Effekt erzielen, indem wir vor jeder Zeile `#` nutzen.

```python
# My first program
# written in python!
# It prints the string Hello World
print("Hello World!")
```
