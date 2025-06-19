🚗 Kennzeichen-Konfigurator Pro

Ein knackiger Web-Konfigurator für deutsche Kfz-Kennzeichen – jetzt mit KI-Vervollständigung, Zufalls-Gags und jeder Menge Komfort. Perfekt zum Lachen, Teilen … oder als kleines Frontend-Showcase 😄

🔥 New & Improved Features

Kategorie	Was ist neu?
Smart Input	Autocomplete: Du tippst „B…“ – sofort erscheinen „B“ (Berlin), „BB“ (Böblingen) etc.
Live-Validierung: Fängt unerlaubte Buchstaben (NS, SA, SS …) ab und blockt zu lange Eingaben.
Fun-Stuff	Randomizer-Button für wahlweise „seriös“, „peinlich“ oder „maximal albern“ (Beispiel: S EX 69).
140+ Emoji- & Meme-Sticker zum Aufpimpen des Schildes („lustige Kennzeichen“).
UX-Extras	Sofort-Vorschau in Retina-Qualität, Dark Mode, Copy-to-Clipboard, Social-Share (Twitter, Threads & Co).
Performance	100 % Vanilla JS + SVG, < 10 kB gzipped, PWA-fähig (offline editieren).
Dev Goodies	TypeScript-Quellcode, ESLint & Prettier, Vitest-Unit-Tests, GitHub Actions CI.
🖼️ Live Preview

Siehe Demo – generiere spontan dein Wunschkennzeichen und exportiere es als PNG oder SVG.
🚀 Live-Demo

👉 Zur Website – läuft in jedem modernen Browser.

🛠️ Installation & Entwicklung

git clone https://github.com/jdl088/kennzeichen-configurator.git
cd kennzeichen-configurator
pnpm install         # eleganter & schneller als npm/yarn
pnpm dev             # Vite-Dev-Server mit Hot Reload
Tipp: Öffne http://localhost:5173/?preset=FUN für einen sofortigen Spaß-Start.
Produktion bauen
pnpm build           # erzeugt statische Files in /dist
🌍 Deployment (GitHub Pages)

Repository → Settings › Pages
Source = gh-pages Branch, Folder =/root
Pushen & fertig – dein Pro-Konfigurator ist live.
🧭 API / Services

Endpunkt	Rückgabe	Zweck
GET /api/cities	JSON [String]	Liste aller Stadt-/Landkreis-Kennzeichen
`GET /api/random?mode=<fun	mild>`	JSON {plate}
optional: POST /api/report	204	Melde anstößige Kombinationen
(Alles lokal als Mock implementiert; kann leicht an echte Backends gehängt werden.)

📅 Roadmap

 Autocomplete Stadtcode
 Zufalls-Generator (seriös / Fun)
 Emoji-/Sticker-Overlay
 SVG-Download mit transparentem Hintergrund
 Multi-Language (i18n)
 Drag-&-Drop-Reihenfolge ändern
📄 Lizenz

MIT License – frei für jeden Unsinn 😉

Viel Spaß beim Basteln deines persönlichen Wunsch- oder Unfug-Kennzeichens!
