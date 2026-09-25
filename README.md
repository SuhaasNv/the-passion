# The Passion — a print in four inks

Twenty-one isometric dioramas, from the entry into Jerusalem to the empty tomb, printed as a
risograph sheet. Everything is drawn by code in a single `index.html`: no images, fonts or libraries.

- `index.html` — the whole experience (open it directly in a browser)
- `server.js` — a tiny dependency-free static server used for hosting
- `media/` — build time-lapse videos

## Run locally

```sh
npm start        # http://localhost:3000
```

## Deploy on Railway

1. In Railway: **New Project → Deploy from GitHub repo →** pick this repository (and branch).
2. Railway detects Node and runs `npm start` (see `railway.json`); the health check is `/healthz`.
3. In the service's **Settings → Networking**, click **Generate Domain** to get the public link.

Live: https://the-passion-production.up.railway.app
