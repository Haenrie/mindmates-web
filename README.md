# MindMates Web

Öffentliche Seiten für MindMates Sudoku und MindMates Kreuzworträtsel, ausgeliefert über GitHub Pages:
https://haenrie.github.io/mindmates-web/

- **Datenschutz:** [index.html](index.html), Startseite der Pages-Adresse.
  - Löschweg ohne App, für Googles Feld „Link zum Löschen des Kontos“: https://haenrie.github.io/mindmates-web/#loeschen
  - Bei Änderungen das Datum „Stand“ oben auf der Seite anpassen.
  - Die Seite beschreibt das Schema der beiden App-Repos (`supabase/migrations`). Ändert sich dort, welche Daten gespeichert werden oder wie lange, wird diese Seite im selben Zug angepasst.
- **Einladungen:** [join/index.html](join/index.html), z. B. `join/?app=sudoku&code=ABC123`. Die Apps hängen den Code an `extra.inviteUrl` aus ihrer `app.json` an. Der Knopf öffnet das Game in der installierten App über ihr URL-Schema (`mindmates-sudoku://join/<code>`, `mindmates-crossword://join/<code>`), auf Android als Chrome-Intent mit Rückfall auf diese Seite.
  - Mit eigener Domain (Ausbaustufe 3) wird derselbe Pfad ein Android App Link und iOS Universal Link; dann ändert sich in den Apps nur `extra.inviteUrl`.

Statische Dateien ohne Build-Schritt.
