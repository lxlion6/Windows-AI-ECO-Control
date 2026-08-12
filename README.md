#Windows AI ECO Control
Leistung Verbessern

Dieser KI Manager soll dein PC langlebiger machen als auch die Leistung verbessern. Im Alltag läuft dein PC auf ECO um Energie und Strom zu sparen und beim starten eines Spiels schaltet der selbstständig auf Performance und gibt dir die beste Leistung. Dieses Programm ist derzeitig in Testphase und Installation auf eigene Gefahr. Für Verbesserungsvorschläge bin ich jederzeit offen. Es gibt auch eine Version für Linux Cashy OS, diese Version ist derzeitig nur auf Anfrage erhältlich.





WINDOWS AI ECO CONTROL - WINDOWS 11 - VERSION 1.4.0
INSTALLATIONSANLEITUNG
============================================================

ZIEL
----
Diese Anleitung führt dich Schritt für Schritt durch die Installation.
Du brauchst keine Programmierkenntnisse.

WICHTIG
-------
- Unterstützt wird Windows 11.
- Python 3.11 oder neuer wird benötigt.
- Die lokale KI über Ollama ist optional.
- Automatische Eingriffe sind beim ersten Start ausgeschaltet.
- Schalte Windows-Sicherheitsfunktionen nicht einfach ab, wenn Windows eine Warnung zeigt.


SCHRITT 1 - ZIP-DATEI ENTPACKEN
--------------------------------
1. Klicke die ZIP-Datei mit der rechten Maustaste an.
2. Wähle "Alle extrahieren...".
3. Wähle einen normalen Ordner, zum Beispiel den Desktop oder Dokumente.
4. Öffne anschließend den entpackten Ordner.

Wichtig: setup.bat und run.bat nicht direkt aus der ZIP-Datei starten.


SCHRITT 2 - PYTHON PRÜFEN
--------------------------
1. Drücke Windows-Taste + R.
2. Tippe: cmd
3. Drücke Enter.
4. Gib ein:

   py --version

Wenn zum Beispiel "Python 3.11", "Python 3.12", "Python 3.13" oder neuer erscheint,
kannst du mit Schritt 4 weitermachen.

Wenn "py" nicht gefunden wird, folgt Schritt 3.


SCHRITT 3 - PYTHON INSTALLIEREN
--------------------------------
Windows 11 kann Python normal installieren.

Empfohlen:
1. Öffne die offizielle Python-Seite: https://www.python.org/downloads/windows/
2. Installiere eine aktuelle Python-Version ab 3.11.
3. Folge dem offiziellen Windows-Installer.
4. Schließe nach der Installation das alte CMD-Fenster.
5. Öffne CMD erneut und prüfe noch einmal:

   py --version

Alternative: Python kann auch über den Microsoft Store beziehungsweise
den aktuellen Python Install Manager bezogen werden.

Verwende keine unbekannten Download-Seiten.


SCHRITT 4 - WINDOWS AI ECO CONTROL EINRICHTEN
--------------------------------------
1. Öffne den entpackten Programmordner.
2. Doppelklicke auf setup.bat.
3. Ein schwarzes Fenster öffnet sich.
4. Warte, bis "Einrichtung abgeschlossen" erscheint.

setup.bat erstellt eine eigene Python-Umgebung nur für dieses Programm
und installiert die benötigten kostenlosen Python-Pakete.


SCHRITT 5 - PROGRAMM STARTEN
-----------------------------
1. Doppelklicke auf run.bat.
2. Die Oberfläche des Windows AI ECO Controls öffnet sich.
3. Kontrolliere zuerst CPU, RAM, GPU und Status.

Beim ersten Test empfehlen wir:
- Automatische Eingriffe: AUS
- Erst beobachten, ob die erkannten Werte plausibel sind.
- Danach gewünschte Eingriffsschwelle und maximale Aggressivität einstellen.
- Änderungen mit "Speichern" übernehmen.


OPTIONALE LOKALE KI - OLLAMA + QWEN3
-------------------------------------
Diese Installation ist NUR nötig, wenn du die Registerkarte "KI-Hilfe & Notfall"
vollständig benutzen möchtest.

Ollama läuft unter Windows als lokale Anwendung. Die KI-Verarbeitung findet lokal statt.

A) Ollama installieren
1. Öffne die offizielle Seite: https://ollama.com/download/windows
2. Lade den Windows-Installer herunter.
3. Installiere Ollama mit den normalen Vorgaben.
4. Öffne danach ein neues CMD- oder PowerShell-Fenster.
5. Prüfe:

   ollama --version

B) Qwen3 1.7B installieren
1. Gib in CMD oder PowerShell ein:

   ollama pull qwen3:1.7b

2. Warte, bis der Download vollständig abgeschlossen ist.
3. Starte anschließend den Windows AI ECO Control neu.

Ohne Ollama bleibt der normale System Manager funktionsfähig.
Die KI-Hilfe zeigt dann lediglich an, dass die lokale KI nicht erreichbar ist.


WAS BEDEUTEN DIE RAM-STUFEN?
-----------------------------
Du stellst bei jeder Stufe nur ein, AB WIE WENIG VERFÜGBAREM RAM sie beginnt.
Die eigentliche Eingriffsstärke ist intern sicher voreingestellt.

Stufe 1 = Frühwarnung / sehr leichter Eingriff
Stufe 2 = leichter Eingriff
Stufe 3 = hoher Eingriff
Stufe 4 = kritische Stufe / stärkster regulärer Eingriff

Zusätzlich kannst du global einstellen, ab welcher Stufe die Automatik überhaupt
handeln darf und welche maximale Aggressivität erlaubt ist.


NOTFALL-KI
-----------
Die Notfall-KI ist standardmäßig AUS.
Wenn du sie einschaltest, gilt:
1. Normale Regeln reagieren zuerst.
2. Ein kritischer Zustand muss zunächst anhalten.
3. Erst danach werden ausschließlich freigegebene Fachquellen gesucht.
4. Die lokale KI darf keine freien CMD-/PowerShell-Befehle ausführen.
5. Nur im Programm vorab definierte, reversible Aktionen sind möglich.
6. Automatische Notfall-Aktionen setzen zusätzlich aktivierte Automatik und
   maximale Aggressivität 4 voraus.


WENN ETWAS NICHT FUNKTIONIERT
------------------------------
1. Starte diagnose.bat oder klicke im Programm auf "Diagnose erstellen".
2. Die Logdateien liegen unter:

   %USERPROFILE%\Windows-AI-ECO-Control\logs

3. Schicke die Diagnose an den Entwickler.

Wenn Python nicht gefunden wird:
- CMD schließen und neu öffnen.
- py --version erneut prüfen.
- Bei Bedarf Python über die offizielle Python-Seite neu installieren.

Wenn die KI-Hilfe nicht funktioniert:
- Prüfe: ollama --version
- Prüfe: ollama list
- In der Liste sollte qwen3:1.7b erscheinen.


DEINSTALLATION
--------------
Im Programm unten "Programm deinstallieren" wählen.
Falls die Oberfläche nicht startet: uninstall.bat doppelklicken.
Weitere Details stehen in DEINSTALLATION.txt.

