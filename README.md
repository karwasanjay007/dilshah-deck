# Dil Shah Tea — Market Entry Strategy

Interactive 23-slide briefing on the South India market opportunity. Self-contained HTML; the only runtime dependencies are Tailwind and Google Fonts, both loaded from CDN.

## View locally

```bash
npm install
npm run dev
```

Opens the deck at `http://localhost:5173`. Navigation: arrow keys, spacebar, the dot row at the bottom, or swipe.

## Open in bolt.new

Once this repo is on GitHub, you can open it in [bolt.new](https://bolt.new) two ways:

1. **From a URL** — visit `https://bolt.new/github.com/<your-username>/dilshah-deck` and bolt will import, install, and start the dev server.
2. **From the dashboard** — open bolt.new, paste the repo URL.

## Deploy

From inside bolt.new, click **Deploy** → pick Netlify (default) or Vercel. Bolt will run `npm run build` and ship the static output. No backend, no env vars needed.

For a manual deploy without bolt:

```bash
npm run build       # output goes to dist/
```

Then drop `dist/` on Netlify Drop, Vercel, Cloudflare Pages, or GitHub Pages — any static host works.

## Project layout

```
dilshah-deck/
├── index.html        # the whole deck — one self-contained file
├── package.json      # vite dev/build scripts (the only build dep)
├── .gitignore
└── README.md
```

The deck is intentionally a single HTML file (no framework, no bundling needed). Vite is here purely for a nice local dev server and a build step bolt's deploy flow can hook into.
