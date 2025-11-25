# tailwind-translator

Webbasierter Tailwind Generator: CSS/SCSS-Deklarationen einfügen und direkt als Tailwind Utility-Klassen kopieren. Ideal, um vorhandene Styles schnell in ein Tailwind-Projekt zu übernehmen.

## Nutzung
- `index.html` im Browser öffnen (kein Build, keine Abhängigkeiten).
- Links CSS/SCSS einkopieren, rechts die generierten Tailwind-Klassen kopieren.
- Nicht zugeordnete Deklarationen werden gelistet und auf Tailwinds Arbitrary Values (`[...]`) zurückgeführt, falls möglich.

## GitHub Pages veröffentlichen
1. Repo auf GitHub pushen (Name: `tailwind-translator`).
2. In den Repository-Einstellungen unter **Pages** als Source den Branch `main` (oder `master`) wählen und den Root (`/`) veröffentlichen.
3. Nach dem Deploy ist die App unter `https://<dein-user>.github.io/tailwind-translator/` erreichbar.

## Features (Kurzfassung)
- Unterstützung für gängige Layout-, Spacing-, Typografie-, Border-, Hintergrund- und Flex/GAP-Properties.
- Shorthand-Erkennung für `margin`, `padding`, `gap`, `border`-Sides sowie Auto-Margins.
- Fallback auf Tailwind Arbitrary Values bei speziellen Werten.
- Copy-Button, Live-Debounce, Counter für konvertierte vs. unsupported Deklarationen.

## Hinweis
Kein Tailwind-Build erforderlich; alles läuft im Browser. Für Erweiterungen (weitere CSS-Properties oder Mapping-Regeln) kann die Logik im Script der `index.html` ergänzt werden.
