# zqmlabs-leaders

Source for **leaders.zqmlabs.com**, the ZQM Labs hosting and community-organizer site. It explains community and office game-hosting options, provides a four-step hosting guide, and renders a Communities directory from the public communities API. This repository contains the site source and its direct-upload deployment script; verify API availability, published offers, and the target Cloudflare Pages project before treating the site as operational.

## Layout

- `site/index.html` — the whole site (one self-contained page).
- `deploy.py` — direct-upload deploy to the Cloudflare Pages project
  `leaders` (the estate's pattern: production builds are direct-upload,
  not git-connected). Usage: `python3 deploy.py site main`.

## History

Stood up 2026-10-23 as a focused-content host (it previously mirrored
the apex site). Repo created the same day at Alex's direction so the
source survives any single machine.
