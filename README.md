# App Store

An Apple App Store–inspired storefront built as a **single self-contained HTML file** — a clean, modern, fully client-side app catalog with categories, multiple app sections, and live search. No backend required, ideal for prototyping and UI experiments.

## Features

- **Horizontal category navigation** — scrollable category bar with active-state filtering
- **App sections** — Top Charts, New Releases, and Editor's Choice, rendered from an in-page dataset
- **Real-time search** — filters apps across all sections as you type
- **Apple-style design** — minimalist white-space layout, card-based UI with subtle shadows, circular app icons, "Get" buttons, system-font typography
- **Fully responsive** — grid layout on desktop, horizontal scroll on mobile
- **Zero build step / zero dependencies** — one HTML file, vanilla CSS + JavaScript

## Tech Stack

- HTML5
- CSS3 (custom, no frameworks)
- Vanilla JavaScript (ES6 template rendering)

## Quick Start

No installation or build required:

```bash
# Option 1 — open directly in a browser
open index.html

# Option 2 — serve locally (any static server)
npx serve .
```

Then visit the URL the server prints (e.g. `http://localhost:3000`).

## Project Structure

```text
App-Store/
├── index.html      # Complete app: markup, styles, and JS in one file
│                     (originally committed as "App Store"; copied to
│                     index.html so static hosts serve the site at the root URL)
├── App Store       # Original file (kept for history)
├── User Guide      # Feature notes and expansion ideas
├── README.md
└── LICENSE
```

The app catalog is a plain JavaScript array near the bottom of `index.html` (`renderApps()`), so adding your own apps is just a matter of editing that array — fields per app are `name`, `developer`, `category`, `section`, `icon`, and `rating`.

## Deploy Notes

Static site — deploy anywhere that serves static files:

- **GitHub Pages** (live): served from the `main` branch root — https://girishlade111.github.io/App-Store/
- Alternatives: Cloudflare Pages, Netlify, Vercel — drop the repo contents into any of them, no build command needed.

## License

See [LICENSE](LICENSE).

---

Built by Girish Lade — https://ladestack.in
