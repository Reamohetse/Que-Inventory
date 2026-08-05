# Que Inventory

A single-page stock ledger and sales-analysis dashboard built for **Que Construction PTY(LTD)**.

Everything runs client-side in the browser — no server, no build step, no dependencies to install. Open `index.html` and it works.

## Features

- **Dashboard** — total items, units on hand, stock value, low-stock and out-of-stock counts, plus a "needs attention" list and recent activity feed
- **Stock List** — searchable, category-grouped table of every item, with a built-in purchase-order builder: tick items, set quantities, and get a running total to buy. Export as a text quote or open it directly in your email app
- **Enter / Update** — add new stock items or record stock in / stock out / physical recounts
- **Monthly Report** — pick any month for units received/consumed, closing stock value, low-stock and out-of-stock lists, and the month's most active items. Downloadable as text or emailed directly
- **Sales Analysis** — monthly trend chart, sales-by-category breakdown, and a top-sellers leaderboard, built from recorded "stock out" movements over a selectable period (3/6/12 months or all time)

## Data & storage

Stock and transaction data is stored locally through the app's built-in storage — nothing is sent to a server. The ledger is pre-seeded with Que Construction's accessories price list on first load; quantities start at 0 until counted stock is entered under **Enter / Update**.

## Running it

Just open `index.html` in any modern browser. No installation needed.

### Hosting on GitHub Pages

1. Push this repo (or just `index.html`) to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — GitHub will publish it at `https://<username>.github.io/<repo-name>/`.

## Tech notes

- Plain HTML/CSS/JS, no build tools
- Charts via [Chart.js](https://www.chartjs.org/) (loaded from CDN)
- Fonts: Arial / Helvetica system stack
