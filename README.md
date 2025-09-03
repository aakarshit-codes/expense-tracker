# Expense Tracker

A simple client-side Expense Tracker web app. It uses plain HTML, CSS and JavaScript organized into small modules and pages to record and visualize expenses.

## Features
- Add, view and categorize transactions (client-side).
- Simple chart page for visualizing expenses.
- Modular JavaScript split under `modules/` for routing, transactions and chart logic.

## Tech stack
- HTML/CSS/JavaScript (vanilla)
- Uses assets in `assets/` for icons and images

## Project structure
- `index.html` — app entry page
- `main.js` — application bootstrap / entry JavaScript
- `styles.css` — global styles
- `modules/` — JavaScript modules (e.g., `chart.js`, `router.js`, `tx.js`)
- `pages/` — HTML partials/pages (`home.html`, `chart.html`)
- `assets/` — images and icons
- `src/output.css` — generated CSS output (if a preprocessor or utility was used)

## How to run
This is a static web app. You can open `index.html` directly in a browser, or serve it with a local static server for a better development experience (recommended).

Open directly:

```bash
# macOS: double-click index.html or open in browser from Finder
open index.html
```

Serve with Python 3 (simple):

```bash
python3 -m http.server 8080
# then open http://localhost:8080 in your browser
```

## Development notes
- Edit UI and pages in `pages/` and `styles.css` or `src/output.css`.
- App logic lives in `modules/`:
  - `router.js` — client-side routing
  - `tx.js` — transaction handling
  - `chart.js` — chart rendering
- If `src/output.css` is generated (e.g., from a preprocessor or Tailwind), check your build setup or package scripts to regenerate it.

