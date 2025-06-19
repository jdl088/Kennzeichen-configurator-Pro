# 🚗 Kennzeichen‑Konfigurator **Pro**

Ein schlanker Web‑Konfigurator für deutsche Kfz‑Kennzeichen – jetzt mit **Autocomplete**, Zufalls‑Gags und jeder Menge Komfort. Perfekt zum Lachen, Teilen … oder als kleines Front‑End‑Showcase 😄

> **Live‑Demo:** [https://jdl088.github.io/Kennzeichen-configurator](https://jdl088.github.io/Kennzeichen-configurator-pro)

---

## 🔥 Features

| Kategorie       | Highlights                                                                                                |
| --------------- | --------------------------------------------------------------------------------------------------------- |
| **Smart Input** | **Autocomplete** für Stadtkürzel (tippe „B…“ → „B“, „BB“, …); Livesyntax‑Check (blockt NS, SS, SA usw.).  |
| **Fun‑Stuff**   | **Randomizer**‑Button (seriös / peinlich / maximal albern, z. B. `S EX 69`); 140 + Emoji‑ & Meme‑Sticker. |
| **UX‑Extras**   | Retina‑Vorschau, Dark‑Mode, Copy‑to‑Clipboard, Social‑Share.                                              |
| **Performance** | 100 % Vanilla JS + SVG, < 10 kB gzipped, **PWA‑fähig** (offline editieren).                               |
| **Dev Goodies** | TypeScript‑Quellcode, ESLint + Prettier, Vitest‑Tests, GitHub Actions CI.                                 |

---

## 🖼️ Screenshots


---

## 📦 Installation & Entwicklung

```bash
# Repo clonen
pnpm create vite kennzeichen-configurator-pro --template vanilla-ts
cd kennzeichen-configurator-pro
pnpm install

# Dev‑Server mit Hot‑Reload starten
pnpm dev
# öffnet i. d. R. http://localhost:5173
```

> **Tipp:** `http://localhost:5173/?preset=FUN` startet direkt mit Zufallskennzeichen.

### Produktion bauen

```bash
pnpm build   # statische Dateien in ./dist
```

---

## 🌍 Deployment auf GitHub Pages

1. `pnpm run deploy` (skript legt Branch **gh‑pages** an)
2. Repository → **Settings › Pages**
3. Branch = **gh‑pages**, Ordner = `/`
4. Speichern – dein Pro‑Konfigurator ist live.

---

## 🧭 API / Services

| Endpoint                         | Returns             | Zweck                              |
| -------------------------------- | ------------------- | ---------------------------------- |
| `GET /api/cities`                | `string[]`          | Liste aller Stadt‑/Landkreis‑Codes |
| `GET /api/random?mode=fun\|mild` | `{ plate: string }` | Zufallskennzeichen                 |
| `POST /api/report`               | `204 No Content`    | Anstößige Kombination melden       |

*(Lokal als Mock implementiert; lässt sich leicht an echte Back‑Ends koppeln.)*

---

## 📅 Roadmap

* [x] Autocomplete Stadtcode
* [x] Zufalls‑Generator (seriös / Fun)
* [x] Emoji‑/Sticker‑Overlay
* [ ] **SVG‑Download mit transparentem Hintergrund**
* [ ] Mehrsprachigkeit (i18n)
* [ ] Drag‑&‑Drop‑Reihenfolge ändern

---

## 🤝 Contributing

Pull‑Requests sind willkommen! Bitte `pnpm lint` & `pnpm test` ausführen, bevor du committest.

---

## 📄 Lizenz

[MIT](LICENSE) – frei für jeden Unsinn 😉

---

> Viel Spaß beim Basteln deines persönlichen Wunsch‑ oder Unfug‑Kennzeichens!
