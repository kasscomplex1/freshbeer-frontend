# 🍺 FRESH BEER LAB — Frontend

Static site for the Fresh Beer Lab prototype. Deployed on Cloudflare Pages.

## Structure
- `/index.html` — Landing page with API docs and demo links
- `/scan/index.html` — Mobile scan page (reads `?batch=X&outlet=Y` from QR)
- `/badge/index.html` — Shareable outlet "FRESH SERVE CERTIFIED" badge

## Deploy
This folder (`static/`) is the Cloudflare Pages **build output directory**. No build step required.

Cloudflare Pages settings:
- Build command: *(none)*
- Build output: `static`
- Custom domain: `fresh.fauluhost.co.tz`

## API
The frontend calls `https://api.fauluhost.co.tz` — see `../freshbeer_api.py` for the backend.

CORS is enabled on the API for any origin.