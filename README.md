# cocapn-ai-pages

GitHub Pages source for [cocapn.ai](https://cocapn.ai) — the fleet hub landing page for the Cocapn AI ecosystem.

## What is this?

This repository hosts the static landing page for the Cocapn AI fleet. It serves as the central hub connecting all domain agents, architecture documentation, and operational portals within the Dojo Model ecosystem.

## Fleet Context

Cocapn operates a distributed network of autonomous domain agents:

- **Keeper**: `Oracle1` — central truth anchor and conflict resolver
- **Edge Nodes**: `JC1`, `Forgemaster`, `CCC` — compute, build, and command nodes
- **Domain Agents**: 8 specialized agents across fishing, study, lucid dreaming, making, DMing, gaming, fitness, and community knowledge
- **Coordinator**: `PLATO` — shared knowledge mesh and fleet-wide state management

## Deployment

This site is deployed via **GitHub Pages** from the `main` branch:

1. Push changes to `main`
2. GitHub Pages automatically builds and serves from the repository root
3. Custom domain `cocapn.ai` is configured via `CNAME` file

No build step is required — `index.html` is a self-contained static file with inline CSS and JavaScript.

## Local Development

Open `index.html` directly in a browser, or serve with any static file server:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## PLATO Integration

The landing page includes a live PLATO Knowledge Browser that attempts to fetch from `http://localhost:8847/room/cocapn-fleet`. When the local PLATO instance is unavailable, it gracefully falls back to sample knowledge tiles.

## Links

- **Live Site**: https://cocapn.ai
- **Crab Trap Portal**: http://147.224.38.131:4059/?domain=cocapn.ai
- **GitHub Org**: https://github.com/cocapn-ai
- **Issues**: https://github.com/cocapn-ai/cocapn-ai-pages/issues
- **Discussions**: https://github.com/cocapn-ai/cocapn-ai-pages/discussions

## License

MIT License — see repository for full terms.
