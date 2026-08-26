# Git & GitHub Grundlagen

## Lernziel
Am Ende dieser Lektion weisst du: was **Git** ist und wozu es dient, wie du Git installierst und konfigurierst, was der Unterschied zwischen einem **lokalen** und einem **Remote-Repository** ist, wie du **Commit, Push und Pull** mit aussagekräftigen **Commit-Messages** durchführst, und wie du einen Commit bei Bedarf rückgängig machst.

---

## 1. Einstieg

- Ohne Versionskontrolle **geht Arbeit schnell verloren**, wenn mehrere Personen gleichzeitig am selben Code arbeiten oder du selbst frühere Zwischenstände wiederherstellen möchtest.
- Git verhindert genau das Chaos von Dateinamen wie "Endgueltig_v2_FINAL_wirklich.docx", indem es jeden Stand deines Codes nachvollziehbar und wiederherstellbar speichert.
- Praktisch jedes professionelle Software-Team arbeitet mit Git – die Grundlagen aus dieser Lektion sind direkt im Lehrbetrieb und in späteren Projekten einsetzbar.

---

## 2. Grundlagen
- Git speichert **Schnappschüsse** (Commits) deines Codes über die Zeit – es überschreibt Dateien nicht einfach, sondern merkt sich jeden Zwischenstand.
- Ein **lokales Repository** liegt auf deinem eigenen Rechner. Ein **Remote-Repository** liegt auf einem Server, z.B. auf GitHub, und ist dort für dich (und ggf. andere) erreichbar.
- Die wichtigsten Befehle:

```bash
git init                        # neues Repository anlegen
git status                      # zeigt, was geändert/noch nicht versioniert ist
git add hello.py                # Änderung zum Commit vormerken
git add .                       # Alle Änderungen in einem Verzeichnis zum Commit vormerken
git commit -m "Erster Commit"   # Schnappschuss erstellen
git log --oneline               # Commit-Historie kompakt anzeigen
git push                        # lokale Commits zu GitHub hochladen
git pull                        # Änderungen von GitHub herunterladen
git clone <URL>                 # bestehendes Repository lokal kopieren
git reset --soft HEAD~1         # macht einen fehlerhaften Commit rückgängig
```

- Der Kreislauf, mit dem du in diesem Kurs meistens arbeiten wirst: **Ändern → Stagen (`git add`) → Committen (`git commit`) → Pushen (`git push`)**.
- Eine gute Commit-Message ist kurz und sagt präzise, was sich am Projekt ändert, z.B. `fix: Tippfehler in Begrüssung korrigiert`. Schlechte Beispiele wie `update` oder `changes` helfen dir (und anderen) später nicht weiter.

<iframe width="560" height="315" src="https://www.youtube.com/embed/a0_AcknhqDY?si=Iku3ypj3IoDGVeTB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## 3. Aufgaben

### 🦊 Git & Github komplett durchspielen

#### Schritt 1 – Git installieren
1. Öffne [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. Installiere Git mit **Standard-Einstellungen**.
3. Prüfen, ob Git funktioniert: `git --version`

![git download page](../img/git.png)

#### Schritt 2 – GitHub-Account erstellen
1. Öffne [https://github.com/](https://github.com/)
2. Klicke auf **Sign up**
3. Benutzername, E-Mail und Passwort wählen
4. E-Mail bestätigen

![github page](../img/github.png)


#### Schritt 3 – Git konfigurieren
Führe diese Befehle im Terminal aus (ersetze mit deinen Daten):
```bash
git config --global user.name "Vorname Nachname"
git config --global user.email "deine@email.ch"
```

Mit `git config --list` kannst du überprüfen, ob du Git richtig konfiguriert hast.

#### Schritt 4 – Python-Projekt anlegen
1. Erstelle einen neuen Ordner für dein Projekt, z.B. `mein-git-projekt`, und öffne ihn in VS Code.
2. Erstelle darin eine neue Datei `hello.py`.
3. Schreibe folgenden Code hinein:
```python
print("Hello Git!")
```
4. Speichere die Datei und führe sie einmal aus, um sicherzustellen, dass sie ohne Fehler läuft.


#### Schritt 5 – Verbindung testen
1. Erstelle ein neues öffentliches (public) Repository auf GitHub
2. Code lokal commiten und pushen:
```bash
git init
git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/deinusername/test-repo.git
git push -u origin main
```

Nach diesen Schritten ist dein Code sowohl lokal als auch auf GitHub sichtbar.

#### Schritt 6 – Status prüfen
Ändere in `hello.py` den ausgegebenen Text, z.B. zu `print("Hello Git! Ich lerne gerade Versionskontrolle.")`, und speichere die Datei. Prüfe danach, was Git von dieser Änderung mitbekommen hat:
```bash
git status
```
Du siehst, dass `hello.py` als **verändert** (modified) angezeigt wird – Git erkennt automatisch, welche Dateien sich seit dem letzten Commit verändert haben.

#### Schritt 7 – Zweiten Commit erstellen
Nimm die Änderung in den nächsten Commit auf:
```bash
git add hello.py
git commit -m "Begrüssungstext angepasst"
git push
```
Prüfe mit `git status`, dass keine offenen Änderungen mehr angezeigt werden.

#### Schritt 8 – Commit-Historie ansehen
Verschaffe dir einen Überblick über alle bisherigen Commits:
```bash
git log --oneline
```
Du solltest jetzt zwei Commits sehen: "First commit" und "Begrüssungstext angepasst". Vergleiche diese Liste mit der Commit-Historie auf GitHub (Reiter "Commits" in deinem Repository) – sie sollte identisch sein.

#### Schritt 9 – Commit rückgängig machen
Manchmal committet man zu früh oder aus Versehen etwas Falsches. Probiere das gefahrlos aus:
1. Ändere `hello.py` erneut, z.B. füge eine Zeile hinzu, die du eigentlich gar nicht behalten willst.
2. Committe sie trotzdem: `git add . && git commit -m "Testcommit, will ich eigentlich nicht"`
3. Mache den Commit rückgängig, ohne die Änderung selbst zu verlieren:
```bash
git reset --soft HEAD~1
```
4. Prüfe mit `git status` und `git log --oneline`: Der Commit ist aus der Historie verschwunden, deine Änderung in `hello.py` ist aber weiterhin vorhanden (jetzt wieder als "staged" markiert). Entscheide danach, ob du sie verwerfen (`git checkout -- hello.py`) oder sauber neu committen möchtest.

Nach diesen Schritten kennst du den kompletten Grundzyklus: Änderung machen → Status prüfen → committen → pushen → Historie ansehen → im Notfall einen Commit rückgängig machen.

---

## 4. Weiterführende Beispiele und Gedanken

- Überlege: Wie könnte Git helfen, wenn zwei Personen gleichzeitig am selben Projekt arbeiten, ohne sich gegenseitig Code zu überschreiben?
- Nächste Themen: Variablen und Datentypen. Vertiefende Git-Themen wie Branches und die Zusammenarbeit mehrerer Personen im selben Repository folgen später in einem anderen Modul.
- Zusätzlicher Gedanke: Praktisch jedes grössere Software-Team der Welt arbeitet mit demselben Grundprinzip, das du heute gelernt hast – die Werkzeuge (GitHub, GitLab, Bitbucket) unterscheiden sich, aber Commit/Push/Pull bleiben gleich.
