# Fruits n' Vegetables 🍎🥕

A free, browser-based tile-connect puzzle game (in the style of Onet / Lianliankan / the
"Fruits and Vegetables" game on games.inbox.lv). Find two matching tiles and connect them
with a path that bends **no more than 3 times** before the timer runs out.

Play it live once GitHub Pages is enabled (see below), or just open `index.html` locally.

## Features
- Levels get bigger and faster as you clear crates
- Hint and Shuffle tools (limited uses per level)
- Auto-reshuffle if no moves remain
- Best score saved locally in your browser
- Single file, zero build step, zero dependencies (besides Google Fonts)

## Deploy to GitHub Pages (free hosting)
1. Create a new **public** repo on GitHub named `fruits-n-vegetables` (or anything you like).
2. Upload `index.html` (and this `README.md`) to the repo — either drag-and-drop on
   github.com, or from your machine:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Fruits n' Vegetables game"
   git branch -M main
   git remote add origin https://github.com/<your-username>/fruits-n-vegetables.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: "Deploy from a branch"**,
   branch `main`, folder `/ (root)`. Save.
4. Wait a minute, then your game will be live at:
   `https://<your-username>.github.io/fruits-n-vegetables/`

## Editing
Everything (HTML, CSS, JS) lives in the one `index.html` file. Useful spots to tweak:
- `ICONS` — the emoji set used for tiles
- `MAX_TURNS` — how many bends a connecting path may have (currently 3)
- `BASE_LEVELS` — grid size / tile-type count / time per level
