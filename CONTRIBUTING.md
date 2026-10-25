# Contributing to zqmlabs-leaders

Source for [leaders.zqmlabs.com](https://leaders.zqmlabs.com/) — the
organizer/host home for ZQM Labs quests: the hosting offers, the
four-step hosting how-to, and the Communities directory, rendered live
from the public communities API. The whole site is one self-contained
page, so the contribution path is short — and the checkout links on it
are live, so it has one rule that matters more than the rest.

## What lives here

- `site/index.html` — the whole site (one self-contained page).
- `deploy.py` — direct-upload deploy to the Cloudflare Pages project
  `leaders`. Usage: `python3 deploy.py site main`.

## How to contribute

1. Fork the repo, or branch from `main` if you have write access, and
   make your edit in `site/index.html`.
2. Keep the page self-contained: this site deliberately has no build
   step and no second page. If your addition needs a full guide rather
   than a section, link out to the host handbook on
   [docs.zqmlabs.com](https://docs.zqmlabs.com/hosting/) instead of
   growing a second page here.
3. **Flag price and checkout-link changes in the PR description.**
   The kit cards link straight to live Stripe checkout. A price or
   checkout-link edit must be confirmed by the maintainer before merge —
   never change a price or a buy link on the strength of this file alone.
4. Keep the Communities directory honest: it renders from the public
   communities API and already handles the empty state (no hosts listed
   yet) and the fetch-failure state. Don't replace either state with
   placeholder names or sample listings.
5. Open a pull request against `main` describing what changed.

## Check before you open the PR

This repo has no CI workflow and no test suite, so these checks run
locally, by the author:

- Open `site/index.html` in a browser and read the changed section in
  place — layout, copy, and every link you touched.
- Confirm every link you added or changed points at a real destination
  (host handbook, Organizer Toolkit, software site, tiers page, or a
  live checkout link), and that no link you touched is a placeholder.

Do not deploy from a branch: deploys go through `main` via `deploy.py`
after merge.

## License

MIT — see `LICENSE`. By contributing you agree your changes are covered
by the same license.
