# Job Hunt Command Center

Live, auto-updating dashboard of Oracle PL/SQL & data-engineering roles in
Kolkata / remote, plus a job tracker. Hosted on GitHub Pages.

- **index.html** — the dashboard (the live page). Auto-reloads hourly.
- **Job_Tracker.xlsx** — live roles + application log.

## How it stays live
A scheduled task (every 4 hours) rebuilds the dashboard from live Naukri +
LinkedIn data, copies it here as `index.html`, and runs `push.sh`, which
pushes to this repo. GitHub Pages serves it at your public URL, so the shared
link is always current.

See **SETUP_GITHUB.md** for the one-time setup that turns the link on.
