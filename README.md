# PattyPlot

A grid based garden planner where you can map out what you want to grow.

Open `index.html` in a browser — no build step, no server required. Paint
tiles (ground, raised beds, pots, walkways, arches), place plants from the
palette, and manage your plant library in the Plants screen. Everything is
saved in your browser's localStorage.

## Offline use

By default the app loads Alpine.js and HTMX from the unpkg CDN. To run fully
offline, download the two libraries into a `vendor/` folder next to
`index.html` — the app automatically prefers local copies when they exist:

```sh
mkdir -p vendor
curl -o vendor/alpine.min.js https://unpkg.com/alpinejs@3.14.1/dist/cdn.min.js
curl -o vendor/htmx.min.js   https://unpkg.com/htmx.org@1.9.12/dist/htmx.min.js
```

The `vendor/` folder is gitignored; it is a local convenience, not part of
the repository.
