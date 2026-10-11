<h1><img src="favicon.svg" height="24"> ubcworkday.ca</h1>

[![Website](https://img.shields.io/website?url=https%3A%2F%2Fubcworkday.ca&label=ubcworkday.ca)](https://ubcworkday.ca)
[![Link check](https://img.shields.io/github/actions/workflow/status/munr0/ubcworkday.ca/link-check.yml?label=links)](https://github.com/munr0/ubcworkday.ca/actions/workflows/link-check.yml)

Quick links for UBC students – Workday, Canvas, and other tools.

Some UBC tools, like Workday, aren't indexed and don't show up in search engine results. [*ubcworkday.ca*](https://ubcworkday.ca)
 does, so searching "UBC Workday" gets you there.

*Not affiliated with the University of British Columbia.*


## Development

Plain HTML/CSS – no build step. GitHub Pages serves `master` directly, so every push goes live; `_config.yml` keeps repo-only files off the site.

Preview locally with <kbd>Ctrl</kbd> <kbd>Shift</kbd> <kbd>B</kbd> in VS Code – a live-reloading server at `localhost:8000` (needs [Node.js](https://nodejs.org)).

## CI

[lychee](https://github.com/lycheeverse/lychee) checks every link on the page, including ubcworkday.ca itself:

- Runs every Monday, and on any change to the page, icons, or check config
- Opens a `stale-links` issue when a link dies, or comments on the one already open
- Closes the issue once every link passes again
