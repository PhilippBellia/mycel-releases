<p align="center">
  <img src="icon.png" width="128" alt="Mycel">
</p>

<h1 align="center">Mycel</h1>

<p align="center">
  <strong>The wood wide web for your codebase.</strong><br>
  A code editor whose main view is not a file tree, but a living graph of your code.
</p>

<p align="center">
  <a href="https://github.com/PhilippBellia/mycel-releases/releases/latest"><img src="https://img.shields.io/github/v/release/PhilippBellia/mycel-releases?label=download&color=2f9e6e" alt="Latest release"></a>
  <img src="https://img.shields.io/badge/platform-Windows-0078d4" alt="Windows">
  <img src="https://img.shields.io/badge/language-English%20%C2%B7%20Deutsch-555" alt="English · Deutsch">
  <a href="[PATREON_LINK_HIER_EINSETZEN](https://www.patreon.com/cw/PhilippBellia)"><img src="https://img.shields.io/badge/Patreon-support%20Mycel-f96854?logo=patreon&logoColor=white" alt="Support on Patreon"></a>
</p>

<p align="center">
  <a href="#english">English</a> · <a href="#deutsch">Deutsch</a>
</p>

---

<a id="english"></a>

## What is Mycel?

In a forest, fungal threads connect the trees underground and carry signals between them —
the *wood wide web*. Mycel does the same for code: it grows through your project and shows
what is connected to what. Folders, files and functions become nodes; imports, calls,
references and inheritance become the threads between them.

You read a codebase the way you would look at a map, not the way you would page through a
filing cabinet.

## Highlights

- **The graph is the editor.** Zoom from folders to files to single functions. Click a node
  and the file opens right next to it. Works with JavaScript, TypeScript and Python.
- **What breaks if I change this?** Calls, references and inheritance come from real
  program analysis, not from a text search.
- **Hidden coupling.** Mycel reads your Git history and shows files that are always
  changed together, even though neither imports the other — the dependency nobody wrote
  down.
- **Your Git changes, in context.** Modified, new and deleted files are marked in the graph,
  so you see not only what you touched, but also what depends on it.
- **The signal path.** Start your Qt application from Mycel, point at a button and see what
  it *would* trigger; click it and watch the path the call actually takes through your
  code. *New in 0.2.1:* Mycel finds out by itself how your project starts — venv, Conda,
  uv, Poetry or the interpreter set in VS Code — and checks beforehand which environment
  can actually load it.
- **Notes on the code.** Attach Markdown notes to any node; they live in your repository and
  show up as `◆` in the graph.
- **Coding agents built in.** Run Claude Code, Codex and other agents right in the
  window — and keep an eye on your Claude quota while you do.
- **The graph for your AI.** Claude Code, Codex and opencode can query the graph directly
  (MCP): "who calls this?" is answered from the real call graph.
- **A full editor.** Completion, errors and go-to-definition, extensions from Open VSX, an
  AI chat that works with any provider — including local models via Ollama.

## Download and install

1. Download **`Mycel-Setup-<version>.exe`** from the
   [latest release](https://github.com/PhilippBellia/mycel-releases/releases/latest).
2. Run it. Mycel installs for your user account; no administrator rights needed.

The installer is currently **not code-signed**, so Windows SmartScreen shows a warning on
first launch. Click **"More info" → "Run anyway"**.

## Updates

Mycel updates itself. It checks for a new version at startup and every four hours, downloads
it in the background and then asks whether to restart. If you choose "Later", the update is
installed the next time you close Mycel.

The files `latest.yml` and `*.blockmap` in each release belong to this mechanism: one names
the version and its checksum, the other lets Mycel download only the parts that changed.

## What Mycel needs

Mycel runs on its own. A few features rely on tools you may already have:

| Feature | needs |
|---|---|
| Coding agents in the agent card | Node.js with `npx` |
| Claude quota display | a Claude Code login |
| Signal path in a Qt application | Python 3.12 and PyQt5 or PyQt6 in the application |
| Branch display, Git state in the graph | Git |

## Support Mycel

Mycel is free to download and use. If it saves you time and you would like to help it grow,
you can support its development on **[Patreon](PATREON_LINK_HIER_EINSETZEN)** — entirely voluntary, and very
much appreciated.

## License

Mycel is proprietary software; this repository contains only the installers, not the source
code. The bundled libraries keep their own licenses; their texts are included with every
installation as `THIRD-PARTY-LICENSES.md`.

---

<a id="deutsch"></a>

## Was ist Mycel?

Im Wald verbinden Pilzfäden die Bäume unter der Erde und tragen Signale zwischen ihnen hin
und her — das *wood wide web*. Mycel macht dasselbe mit Code: Es wächst durch dein Projekt
und zeigt, was womit zusammenhängt. Ordner, Dateien und Funktionen werden zu Knoten;
Importe, Aufrufe, Referenzen und Vererbung zu den Fäden dazwischen.

Du liest eine Codebasis wie eine Landkarte, nicht wie einen Aktenschrank.

## Was Mycel kann

- **Der Graph ist der Editor.** Zoome von Ordnern über Dateien bis zu einzelnen Funktionen.
  Ein Klick auf einen Knoten öffnet die Datei direkt daneben. Für JavaScript, TypeScript und
  Python.
- **Was bricht, wenn ich das ändere?** Aufrufe, Referenzen und Vererbung stammen aus echter
  Programmanalyse, nicht aus einer Textsuche.
- **Verborgene Kopplung.** Mycel liest die Git-Historie und zeigt Dateien, die fast immer
  gemeinsam geändert werden, obwohl keine die andere importiert — die Abhängigkeit, die
  niemand aufgeschrieben hat.
- **Deine Git-Änderungen im Zusammenhang.** Geänderte, neue und gelöschte Dateien sind im
  Graphen markiert. So siehst du nicht nur, was du angefasst hast, sondern auch, was daran
  hängt.
- **Der Signalweg.** Starte deine Qt-Anwendung aus Mycel, zeig auf einen Knopf und sieh, was
  er auslösen *würde*; klick ihn und verfolge den Weg, den der Aufruf tatsächlich durch
  deinen Code nimmt. *Neu in 0.2.1:* Mycel findet selbst heraus, wie dein Projekt startet —
  venv, Conda, uv, Poetry oder der in VS Code eingestellte Interpreter — und prüft vorher,
  welche Umgebung es wirklich laden kann.
- **Notizen am Code.** Hänge Markdown-Notizen an jeden Knoten; sie liegen in deinem
  Repository und erscheinen im Graphen als `◆`.
- **Coding-Agenten eingebaut.** Claude Code, Codex und weitere Agenten laufen direkt im
  Fenster — mit deinem Claude-Kontingent im Blick.
- **Der Graph für deine KI.** Claude Code, Codex und opencode fragen den Graphen direkt ab
  (MCP): „Wer ruft das auf?“ beantwortet der echte Aufrufgraph.
- **Ein vollwertiger Editor.** Vervollständigung, Fehler und Go-to-Definition, Extensions von
  Open VSX, ein KI-Chat mit jedem Anbieter — auch mit lokalen Modellen über Ollama.

## Herunterladen und installieren

1. Unter [neueste Version](https://github.com/PhilippBellia/mycel-releases/releases/latest)
   die Datei **`Mycel-Setup-<version>.exe`** herunterladen.
2. Ausführen. Mycel wird für dein Benutzerkonto installiert, ohne Administratorrechte.

Der Installer ist derzeit **nicht signiert**. Windows SmartScreen warnt deshalb beim ersten
Start: **„Weitere Informationen“ → „Trotzdem ausführen“**.

## Updates

Mycel aktualisiert sich selbst. Es fragt beim Start und danach alle vier Stunden nach einer
neuen Version, lädt sie im Hintergrund und fragt dann, ob es gleich neu starten soll. Wer
„Später“ wählt, bekommt das Update beim nächsten Beenden.

Die Dateien `latest.yml` und `*.blockmap` in jedem Release gehören zu diesem Mechanismus: die
eine nennt Version und Prüfsumme, die andere erlaubt, nur geänderte Teile zu laden.

## Was Mycel auf dem Rechner braucht

Mycel läuft ohne weitere Programme. Einzelne Funktionen setzen etwas voraus:

| Funktion | braucht |
|---|---|
| Coding-Agenten in der Agenten-Karte | Node.js mit `npx` |
| Kontingent von Claude | eine Anmeldung in Claude Code |
| Signalweg in einer Qt-Anwendung | Python 3.12 und PyQt5 oder PyQt6 in der Anwendung |
| Branch-Anzeige, Git-Zustand im Graphen | Git |

## Mycel unterstützen

Mycel kostet nichts. Wenn es dir Zeit spart und du mithelfen möchtest, dass es weiterwächst,
kannst du die Entwicklung auf **[Patreon](PATREON_LINK_HIER_EINSETZEN)** unterstützen — ganz freiwillig, und
sehr willkommen.

## Lizenz

Mycel ist proprietär; dieses Repository enthält nur die Installer, nicht den Quelltext. Die
mitgelieferten Bibliotheken behalten ihre eigenen Lizenzen; deren Texte liegen jeder
Installation als `THIRD-PARTY-LICENSES.md` bei.
