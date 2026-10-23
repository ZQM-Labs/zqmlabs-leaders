# zqmlabs-leaders

Source for **leaders.zqmlabs.com** — the organizer/host home for ZQM Labs
quests: the Community and Office hosting offers, a four-step hosting
how-to, and the Communities directory, rendered live from the public
communities API.

## Layout

- `site/index.html` — the whole site (one self-contained page).
- `deploy.py` — direct-upload deploy to the Cloudflare Pages project
  `leaders` (the estate's pattern: production builds are direct-upload,
  not git-connected). Usage: `python3 deploy.py site main`.

## History

Stood up 2026-10-23 as a focused-content host (it previously mirrored
the apex site). Repo created the same day at Alex's direction so the
source survives any single machine.
