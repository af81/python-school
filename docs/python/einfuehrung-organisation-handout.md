# Einführung & Organisation

*Kontext: Berufsschule (Informatik-Grundkurs) · Dauer: 90 Min*

## Lernziel
Am Ende dieser Lektion weisst du: wie dieses Modul aufgebaut ist, wie du deine Entwicklungsumgebung (VS Code + Python) einrichtest, wie du einen GitHub-Account und dein erstes Repository anlegst – und du hast dein erstes eigenes Python-Programm ausgeführt.

## 1. Einstieg
*Warum ist das wichtig?*

- Software begegnet dir jeden Tag: in Apps auf deinem Handy, in Games, in Kassensystemen im Laden. Jemand hat all das programmiert.
- Diskussion: "KI kann doch schon programmieren – wieso lernen wir das dann noch?" Sammelt in der Gruppe Pro- und Contra-Argumente.
- Wichtige Gegenargumente, die du kennen solltest: KI-generierter Code muss verstanden, geprüft und bei Fehlern korrigiert werden können – ohne eigenes Grundwissen kannst du das nicht beurteilen. Ohne Grundlagen kannst du weder gute Prompts schreiben noch erkennen, ob ein KI-Vorschlag stimmt. Die Lehrabschlussprüfung verlangt Code-Verständnis ohne KI-Hilfe.
- Am Ende dieses Semesters kannst du selbst ein kleines Programm mit eigener Logik schreiben – und damit auch KI-generierten Code kompetent beurteilen.

## 2. Grundlagen
*Um was geht es? Was musst du wissen?*

- Das Modul besteht aus vier Bausteinen: theoretische Grundlagen, praktisches Programmieren, Arbeiten mit Git und GitHub, sowie mehrere kleinere Prüfungen über das Semester verteilt.
- Ein Programm ist wie ein Rezept: eine Anleitung, die der Computer Schritt für Schritt abarbeitet. VS Code ist der Editor, in dem du diese Anleitung schreibst; Python ist die Sprache, in der du sie formulierst.
- GitHub ist die Plattform, auf der du deinen Code sicherst, später mit anderen zusammenarbeitest und dir ein kleines Portfolio aufbaust.

```python
print("Hello World")
```
Das ist bereits ein vollständiges Python-Programm: Es gibt den Text "Hello World" aus.

## 3. Anwendung
*Wie funktioniert es? Schritt für Schritt am Beispiel*

- Schritt 1: Python installieren (Download von python.org, Installation starten, Haken bei "Add to PATH" setzen).
- Schritt 2: Visual Studio Code installieren und die Python-Erweiterung über den Extensions-Marktplatz hinzufügen.
- Schritt 3: Eine neue Datei `hello.py` anlegen, den Code oben eintippen und über den "Run"-Button ausführen.

```python
# hello.py
print("Hello World")
# Ausgabe im Terminal: Hello World
```

## 4. Üben
*Aufgaben zum Vertiefen*

**Aufgabe: Entwicklungsumgebung einrichten**
Installiere Python und Visual Studio Code auf deinem Gerät und richte die Python-Erweiterung ein, sodass du Code ausführen kannst.

- **Basic:** Folge der Schritt-für-Schritt-Anleitung in Kapitel 3 exakt. Bei Problemen: Lehrperson beiziehen.
- **Intermediate:** Führe zusätzlich im Terminal `python --version` aus und kontrolliere, dass eine aktuelle Version angezeigt wird.
- **Advanced:** Installiere zusätzlich eine Erweiterung oder ein Theme deiner Wahl in VS Code und notiere kurz, warum du diese gewählt hast.

*Kontrollgrösse:* Die Ausführung von `hello.py` zeigt "Hello World" im Terminal.

**Aufgabe: GitHub-Account & erstes Repository**
Erstelle einen GitHub-Account (falls noch nicht vorhanden) und lege ein erstes Repository für den Kurs an.

- **Basic:** Erstelle den Account und lege ein Repository mit dem Namen "python-kurs-[Nachname]" an.
- **Intermediate:** Ergänze zusätzlich ein Profilbild und eine kurze Profilbeschreibung.
- **Advanced:** Versieh dein Repository mit einer README-Datei, die kurz beschreibt, was darin im Verlauf des Semesters entstehen wird.

*Kontrollgrösse:* Ein sichtbares Repository mit korrektem Namen ist in deinem GitHub-Profil vorhanden.

## 5. Lösungen

**Entwicklungsumgebung:**

- Basic/Intermediate: Nach korrekter Installation zeigt `python --version` z.B. `Python 3.12.x` an, und `hello.py` gibt beim Ausführen "Hello World" aus.
- Advanced: Es gibt keine "falsche" Wahl bei Theme/Erweiterung – wichtig ist eine nachvollziehbare Begründung (z.B. bessere Lesbarkeit, dunkles Design für die Augen).

**GitHub-Account & Repository:**

- Basic: Repository "python-kurs-[Nachname]" ist im eigenen Profil sichtbar und öffentlich oder privat (je nach Vorgabe) erreichbar.
- Intermediate: Profilbild und Beschreibung sind im GitHub-Profil sichtbar.
- Advanced: Beispiel für eine passende README: "In diesem Repository sammle ich meine Python-Übungen aus dem Informatik-Grundkurs."

## 6. Weiterführende Beispiele und Gedanken
*Transfer*

- Überlege: Wo in deinem eigenen Alltag oder Lehrbetrieb könnte ein kleines selbst geschriebenes Programm bereits jetzt nützlich sein?
- Nächste Lektion: Was passiert eigentlich, wenn du auf "Run" drückst – Compiler versus Interpreter.
- Zusätzlicher Gedanke: Viele grosse Open-Source-Projekte, die du vielleicht schon nutzt (z.B. Spiele-Engines, Programmiersprachen selbst), werden öffentlich auf GitHub entwickelt – dein erstes Repository heute ist technisch derselbe Mechanismus im Kleinen.
- Auch wenn du später im Berufsleben KI-Tools zum Programmieren nutzt: Je besser du die Grundlagen beherrschst, desto gezielter kannst du diese Tools einsetzen und desto sicherer erkennst du, wenn ein KI-Vorschlag fehlerhaft ist.
