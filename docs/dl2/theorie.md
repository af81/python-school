# Theorie

## Wie funktioniert ein Computerprogramm?

Ein **Computerprogramm** ist eine Reihe von Anweisungen, die einem Computer sagen, was er tun soll.
Diese Anweisungen werden in einer **Programmiersprache** geschrieben (z. B. Python, Java oder C++).

Ablauf in Kurzform:
1. **Eingabe**: Der Benutzer oder ein anderes System liefert Daten.
2. **Verarbeitung**: Das Programm führt Schritt für Schritt die Anweisungen aus (Berechnungen, Vergleiche, Logik).
3. **Ausgabe**: Die Ergebnisse werden dargestellt, gespeichert oder an andere Systeme weitergegeben.

👉 Ein Programm funktioniert also wie ein Rezept: Es beschreibt präzise, welche Schritte in welcher Reihenfolge auszuführen sind, damit ein gewünschtes Ergebnis entsteht.

Hier ein kleines Beispiel in **Python**, das zeigt, wie ein Programm Eingaben verarbeitet und eine Ausgabe erzeugt:

```python
# 1. Eingabe: Benutzer gibt seinen Namen ein
name = input("Wie heisst du? ")

# 2. Verarbeitung: Text zusammensetzen
begrüssung = "Hallo, " + name + "! Schön, dich zu sehen."

# 3. Ausgabe: Ergebnis anzeigen
print(begrüssung)

```

## Compiler vs. Interpreter

Ein **Compiler** und ein **Interpreter** sind Programme, die Quellcode (den der Programmierer schreibt) in etwas übersetzen, das der Computer verstehen und ausführen kann.
Der Unterschied liegt vor allem in **wann** und **wie** die Übersetzung passiert.

| Merkmal              | Compiler                                                                 | Interpreter                                                               |
|-----------------------|--------------------------------------------------------------------------|---------------------------------------------------------------------------|
| **Arbeitsweise**      | Übersetzt den gesamten Quellcode auf einmal in Maschinencode (eine ausführbare Datei). | Liest und führt den Quellcode Schritt für Schritt direkt aus.             |
| **Geschwindigkeit**   | Ausführung ist meist schneller, da der Code vorher komplett übersetzt wurde. | Langsamer, da die Übersetzung während der Laufzeit passiert.              |
| **Fehlererkennung**   | Meldet Fehler erst nach der vollständigen Übersetzung.                   | Meldet Fehler sofort beim Ausführen der fehlerhaften Stelle.              |
| **Beispiele**         | C, C++ (meist kompiliert)                                                | Python, JavaScript (meist interpretiert)                                  |
| **Ausgabe**           | Erstellt eine separate, ausführbare Datei (.exe, .out etc.).             | Führt den Code direkt aus, ohne eine zusätzliche Datei zu erzeugen.       |

👉 Zusammengefasst:
- **Compiler** = „Übersetzer im Voraus“ (macht ein fertiges Programm).
- **Interpreter** = „Übersetzer in Echtzeit“ (führt direkt aus).
