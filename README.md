# OmniTG — Stitch UI Export

This repository contains the HTML screen exports and preview images from the supplied Google Stitch project.

## Preview locally
Open `index.html` in a browser, or run a local static server from the repository root:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

Each screen is also available as `/<screen-folder>/` because an `index.html` copy is included alongside the original `code.html`.

## Deploy with GitHub Pages
1. Create a new **public** or **private** GitHub repository.
2. Upload the contents of this folder (not the outer ZIP folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. Wait for the Pages deployment to finish. The site will be available at the URL shown there.

## Important scope
This is a **static UI export**, not a complete functioning Telegram bot or Android app. The exported HTML may load fonts, icons, or CSS frameworks from external CDNs and therefore may need an internet connection. Telegram Bot API calls, authentication, persistence, moderation, voice-chat streaming, games, and other backend behavior are not supplied by these visual screens and must be implemented and secured separately.

## Project structure
- `index.html` — screen gallery / landing page
- `omnitg_*/index.html` — openable screen pages
- `omnitg_*/code.html` — original Stitch HTML exports
- `omnitg_*/screen.png` — original previews where supplied
- `cyber_telegram_mini_app/DESIGN.md` — design notes
