# Mycel — Releases

> **The wood wide web for your codebase.**

Hier liegen die Installer von Mycel, sonst nichts. Der Quelltext ist nicht öffentlich.

## Installieren

Unter [Releases](https://github.com/PhilippBellia/mycel-releases/releases/latest) die Datei
`Mycel-Setup-<version>.exe` herunterladen und ausführen. Installiert wird für den eigenen
Benutzer, ohne Administratorrechte.

Der Installer ist derzeit **nicht signiert**. Windows SmartScreen warnt deshalb beim ersten
Start: „Weitere Informationen" → „Trotzdem ausführen".

## Updates

Eine installierte Mycel-Version fragt beim Start und danach alle vier Stunden hier nach einer
neueren. Ist eine da, wird sie im Hintergrund geladen; danach fragt Mycel, ob es gleich neu
starten soll. Wer „Später" wählt, bekommt das Update beim nächsten Beenden.

Die Dateien `latest.yml` und `*.blockmap` in jedem Release gehören zu diesem Mechanismus:
die eine nennt Version und Prüfsumme, die andere erlaubt, nur geänderte Teile zu laden.

## Was Mycel auf dem Rechner braucht

Mycel läuft ohne weitere Programme. Einzelne Funktionen setzen etwas voraus:

| Funktion | braucht |
|---|---|
| Coding-Agenten in der Agenten-Karte | Node.js mit `npx` |
| Kontingent von Claude | eine Anmeldung in Claude Code |
| Signalweg in einer Qt-Anwendung | Python 3.12 und PyQt5 oder PyQt6 in der Anwendung |
| Branch-Anzeige, Git-Zustand im Graphen | Git |

## Lizenz

Mycel ist proprietär; die mitgelieferten Bibliotheken behalten ihre eigenen Lizenzen. Deren
Texte liegen jeder Installation als `THIRD-PARTY-LICENSES.md` bei.
