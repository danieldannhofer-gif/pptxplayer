# pptx-morph Player

Spielt mit morphkit erzeugte `.pptx`-Decks im Browser ab, inklusive Morph (ohne Microsoft-Abo).

- `player.html` ist eigenständig und offline lauffähig: in Edge/Chrome öffnen, `.pptx` hineinziehen.
- Bedienung: Pfeiltasten/Leertaste/Klick = weiter, Pfeil links/Rechtsklick/linker Rand = zurück, F = Vollbild.
- Neu bauen nach Änderungen an `src/`: `node build.js`.
- Tests (Python + Playwright, Edge): `test/parser.py <deck.pptx>…`, `test/behavior.py <deck>`, `test/morph.py <deck> 3-4 …`, `test/sweep.py <deck>…`, `test/shots.py <deck> <outdir>`.
- Design und Grenzen: `SPEC.md` (Stufe 1; byWord/byChar, Gruppen, Custom-Geometrie, Tabellen/Diagramme fehlen noch).
