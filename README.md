# KI---Windows--Manager
Leistung Verbessern

Dieser KI Manager soll dein PC langlebiger machen als auch die Leistung verbessern. Im Alltag läuft dein PC auf ECO um Energie und Strom zu sparen und beim starten eines Spiels schaltet der selbstständig auf Performance und gibt dir die beste Leistung. Dieses Programm ist derzeitig in Testphase und Installation auf eigene Gefahr. Für Verbesserungsvorschläge bin ich jederzeit offen. Es gibt auch eine Version für Linux Cashy OS, diese Version ist derzeitig nur auf Anfrage erhältlich.






KI SYSTEM MANAGER - WINDOWS 11 - VERSION 1.1
INSTALLATIONSANLEITUNG FUER TESTER
=====================================

ZIEL DIESER ANLEITUNG
---------------------
Diese Anleitung fuehrt dich Schritt fuer Schritt durch die Installation.
Du brauchst keine besonderen Computerkenntnisse. Fuehre die Schritte bitte
in der angegebenen Reihenfolge aus.

WICHTIG VOR DEM START
---------------------
Der KI System Manager ist eine Testversion fuer Windows 11.
Beim ersten Start sind automatische Eingriffe AUS. Das Programm beobachtet
zunaechst nur den Systemzustand. Du entscheidest spaeter selbst, ob und ab
welcher Belastungsstufe das Programm eingreifen darf.

VORAUSSETZUNGEN
---------------
Du benoetigst:

1. Einen PC mit Windows 11.
2. Eine Internetverbindung fuer die einmalige Einrichtung.
3. Python 3.11 oder neuer.
4. Den entpackten Ordner "KI-System-Manager-Windows-v1".

Keine Sorge: Falls Python noch nicht installiert ist, wird die Installation
unten Schritt fuer Schritt erklaert.


SCHRITT 1 - ZIP-DATEI ENTPACKEN
--------------------------------
1. Suche die heruntergeladene ZIP-Datei.
2. Klicke mit der rechten Maustaste auf die ZIP-Datei.
3. Waehle "Alle extrahieren...".
4. Waehle einen Ordner, den du leicht wiederfindest, zum Beispiel den Desktop.
5. Klicke auf "Extrahieren".

Wichtig:
Starte setup.bat NICHT direkt aus der ZIP-Datei. Der komplette Ordner muss
vorher entpackt sein.


SCHRITT 2 - PYTHON PRUEFEN
---------------------------
Python ist bei Windows 11 nicht automatisch als vollstaendige
Programmierumgebung vorinstalliert. Fuer den KI System Manager wird
Python 3.11 oder neuer benoetigt.

So pruefst du, ob Python bereits vorhanden ist:

1. Druecke die Windows-Taste.
2. Schreibe: cmd
3. Oeffne die "Eingabeaufforderung".
4. Gib folgenden Befehl ein:

   py --version

5. Druecke die Eingabetaste.

Wenn zum Beispiel "Python 3.11", "Python 3.12", "Python 3.13" oder eine
neuere Version angezeigt wird, ist alles in Ordnung.

Dann kannst du das schwarze Fenster schliessen und mit SCHRITT 4 fortfahren.

Wenn "py" nicht gefunden wird oder keine passende Python-Version vorhanden
ist, fuehre SCHRITT 3 aus.


SCHRITT 3 - PYTHON UNTER WINDOWS 11 INSTALLIEREN
-------------------------------------------------
EMPFOHLENE EINFACHE METHODE: MICROSOFT STORE

1. Druecke die Windows-Taste.
2. Oeffne den "Microsoft Store".
3. Suche nach:

   Python Install Manager

4. Achte darauf, dass es sich um den Python Install Manager der
   Python Software Foundation handelt.
5. Klicke auf "Installieren".
6. Warte, bis die Installation abgeschlossen ist.
7. Schliesse den Microsoft Store.

Jetzt muss noch die eigentliche Python-Laufzeit bereitgestellt werden:

8. Druecke die Windows-Taste.
9. Schreibe: cmd
10. Oeffne die "Eingabeaufforderung".
11. Gib ein:

    python

12. Druecke die Eingabetaste.

Wenn noch keine Python-Laufzeit vorhanden ist, kann der aktuelle Python
Install Manager automatisch die aktuelle stabile Python-Version bereitstellen.
Dies kann einen Moment dauern und benoetigt eine Internetverbindung.

13. Wenn Python gestartet wurde, erkennst du dies unter anderem an einer
    Versionsanzeige und dem Zeichen:

    >>>

14. Gib danach ein:

    exit()

15. Druecke die Eingabetaste.

16. Pruefe nun die installierte Version mit:

    py --version

Es muss mindestens Python 3.11 angezeigt werden.
Eine hoehere stabile Version ist ebenfalls geeignet.

ALTERNATIVE: INSTALLATION UEBER PYTHON.ORG

Falls du den Microsoft Store nicht verwenden moechtest:

1. Oeffne im Browser die offizielle Python-Webseite:

   https://www.python.org/downloads/

2. Lade dort den offiziellen Python Install Manager fuer Windows herunter.
3. Oeffne die heruntergeladene Installationsdatei.
4. Waehle "Install" beziehungsweise "Installieren".
5. Warte, bis die Installation abgeschlossen ist.
6. Oeffne danach die Eingabeaufforderung und gib ein:

   python

7. Pruefe anschliessend mit:

   py --version

   ob mindestens Python 3.11 vorhanden ist.

HINWEIS ZU "PATH"
------------------
Bei aktuellen Versionen des offiziellen Python Install Managers stehen die
Befehle "python" und "py" normalerweise direkt unter Windows zur Verfuegung.
Wenn Windows waehrend der Einrichtung anbietet, Python-Verzeichnisse zum
PATH hinzuzufuegen, darf diese Option aktiviert werden. Fuer den KI System
Manager ist vor allem wichtig, dass der Befehl "py" funktioniert.

Wenn "py" trotz Installation nicht gefunden wird, starte Windows einmal neu
und pruefe danach erneut mit:

   py --version


SCHRITT 4 - EINRICHTUNG DES KI SYSTEM MANAGERS STARTEN
-------------------------------------------------------
1. Oeffne den entpackten Ordner "KI-System-Manager-Windows-v1".
2. Doppelklicke auf die Datei "setup.bat".
3. Es oeffnet sich ein schwarzes Fenster.
4. setup.bat prueft zuerst automatisch:
   - ob Python vorhanden ist,
   - ob Python mindestens Version 3.11 ist.
5. Anschliessend erstellt die Einrichtung eine eigene Python-Umgebung nur
   fuer den KI System Manager.
6. Danach werden die benoetigten Programmbibliotheken installiert.
7. Schliesse das Fenster waehrend der Einrichtung NICHT.
8. Warte, bis folgende Meldung erscheint:

   "Einrichtung abgeschlossen. Danach run.bat starten."

9. Druecke danach eine Taste. Das Fenster schliesst sich.

Die Einrichtung muss normalerweise nur EINMAL durchgefuehrt werden.


SCHRITT 5 - PROGRAMM STARTEN
-----------------------------
1. Bleibe im Ordner "KI-System-Manager-Windows-v1".
2. Doppelklicke auf "run.bat".
3. Der KI System Manager wird gestartet.

Beim ersten Start:
- Automatische Eingriffe sind AUS.
- Das Programm darf dein System zunaechst nur beobachten und bewerten.
- Du kannst die Eingriffsschwelle und maximale Aggressivitaet selbst einstellen.


SCHRITT 6 - SICHERER ERSTER TEST
---------------------------------
Fuer den ersten Test empfehlen wir:

- Automatische Eingriffe: AUS
- Eingriff ab Belastungsstufe: 3 - Hohe Belastung
- Maximale Aggressivitaet: 2 - Ausgeglichen

Beobachte zuerst einige Minuten die angezeigten Werte fuer CPU, RAM,
Datentraeger und Prozesse.

Erst wenn die Anzeige nachvollziehbar funktioniert, kannst du die
automatischen Eingriffe einschalten.

Auch bei hoher Aggressivitaet beendet Version 1.1 keine Prozesse automatisch.
Die aktive Vordergrund-App wird von automatischen Eingriffen ausgenommen.
Kritische Windows-Prozesse sind zusaetzlich geschuetzt.


WENN WINDOWS EINE SICHERHEITSABFRAGE ZEIGT
-------------------------------------------
Bei BAT-Dateien kann Windows eine Sicherheitswarnung anzeigen.
Pruefe immer, ob du wirklich die Datei aus dem entpackten
KI-System-Manager-Ordner gestartet hast.

Wenn Windows die Ausfuehrung vollstaendig blockiert oder du unsicher bist,
beende den Vorgang und melde die genaue Meldung an den Entwickler.
Deaktiviere keine Windows-Sicherheitsfunktionen nur fuer die Installation.


WENN DIE INSTALLATION NICHT FUNKTIONIERT
-----------------------------------------
Fall A - Meldung "Python wurde nicht gefunden"

1. Installiere den offiziellen Python Install Manager wie in SCHRITT 3.
2. Oeffne danach die Eingabeaufforderung.
3. Gib ein:

   py --version

4. Wenn mindestens Python 3.11 angezeigt wird, starte setup.bat erneut.
5. Wird "py" weiterhin nicht gefunden, starte Windows neu und pruefe erneut.

Fall B - Meldung "Python 3.11 oder neuer wird benoetigt"

Auf dem PC ist Python vorhanden, aber die gefundene Version ist zu alt.
Installiere ueber den Python Install Manager eine aktuelle stabile Version
und starte danach setup.bat erneut.

Fall C - setup.bat meldet "Einrichtung fehlgeschlagen"

1. Fotografiere oder notiere die Fehlermeldung im schwarzen Fenster.
2. Starte danach "diagnose.bat".
3. Die Diagnose-Dateien werden unter folgendem Ordner gespeichert:

   %USERPROFILE%\KI-System-Manager-Windows\logs

4. Sende die Fehlermeldung und die Diagnose-Datei an den Entwickler.

Fall D - run.bat meldet "Bitte zuerst setup.bat starten"

Die Einrichtung wurde noch nicht abgeschlossen.
Starte zuerst setup.bat und danach erneut run.bat.


PROGRAMM SPAETER WIEDER STARTEN
--------------------------------
Nach erfolgreicher Einrichtung musst du setup.bat nicht jedes Mal ausfuehren.
Zum normalen Start reicht:

1. Programmordner oeffnen.
2. run.bat doppelklicken.


DEINSTALLATION
--------------
Der KI System Manager kann spaeter wieder entfernt werden.

Moeglichkeit 1 - direkt im Programm:
1. KI System Manager starten.
2. Auf "Programm deinstallieren" klicken.
3. Sicherheitshinweis lesen.
4. Deinstallation bestaetigen.

Moeglichkeit 2 - falls das Programm nicht startet:
1. Programmordner oeffnen.
2. uninstall.bat doppelklicken.
3. Rueckfrage bestaetigen.

Eine ausfuehrliche Anleitung befindet sich auch in "DEINSTALLATION.txt".

Die Deinstallation entfernt NICHT Python, Windows oder andere Programme.
Python kann auf dem PC bleiben und von anderen Programmen verwendet werden.


KURZFASSUNG
-----------
1. ZIP-Datei entpacken.
2. Mit "py --version" pruefen, ob Python 3.11 oder neuer vorhanden ist.
3. Falls nicht: offiziellen Python Install Manager installieren.
4. Danach setup.bat einmal starten.
5. Nach erfolgreicher Einrichtung run.bat starten.
6. Beim ersten Test automatische Eingriffe ausgeschaltet lassen.
7. Bei Problemen diagnose.bat starten.
8. Zum Entfernen den Deinstallationsbutton oder uninstall.bat verwenden.

=====================================
KI System Manager - Windows 11 - V1
Testversion
=====================================
