ANDALUSIEN 2026 – Reise-App (GitHub Pages / PWA)

Diese 6 Dateien alle in den ROOT deines Repos hochladen (nicht in einen Unterordner):
  index.html
  manifest.webmanifest
  sw.js
  icon-192.png
  icon-512.png
  apple-touch-icon.png
  robots.txt

SO GEHT'S:
1. GitHub-Konto anlegen (falls noch keins).
2. Neues Repository erstellen, Sichtbarkeit: PUBLIC (z. B. Name "andalusien").
3. Alle Dateien oben hochladen (Add file -> Upload files -> committen).
4. Settings -> Pages -> Source "Deploy from a branch" -> Branch: main, Ordner: / (root) -> Save.
5. ~1 Minute warten. Seite ist live unter:
   https://<DEIN-BENUTZERNAME>.github.io/<REPO-NAME>/
6. iPhone: Link in SAFARI oeffnen -> Teilen -> "Zum Home-Bildschirm".
   -> App-Icon erscheint. Einmal bei Netz oeffnen, damit sie sich fuer offline speichert.

HINWEISE:
- noindex ist eingebaut (Meta-Tag + robots.txt): taucht nicht in Suchmaschinen auf.
  Der Link selbst bleibt fuer jeden erreichbar, der ihn kennt.
- Alle Pfade sind relativ -> der Repo-Name ist egal.
- Offline: Nach dem ersten Oeffnen mit Netz laeuft die App auch ohne Internet.
- Update: Wenn eine neue index.html kommt, in sw.js die Zeile
  const CACHE = 'andalusien-2026-v1';  auf ...-v2 aendern (erzwingt Neu-Cachen).
