# nullgrid.dev

The Null website, by Null Labs. Three families: **Suite** (Null Grid, Null Search, Null Notes, Null Drive, Null Scribe), **Systems** (Null OS, Null Short, Null File) and **Labs** (Null Play).

Plain static HTML, no build step. Served by GitHub Pages from the `main` branch root.

| File | Page |
|---|---|
| `index.html` | Home: lockup, three paths, the three families |
| `suite.html`, `systems.html`, `labs.html` | One page per family |
| `grid.html`, `search.html`, `notes.html`, `drive.html`, `scribe.html`, `os.html`, `short.html`, `file.html`, `play.html` | One page per product, each ending in its `#download` section |
| `downloads.html` | Every product, grouped by family, with its version line |
| `docs.html` | Install, README and changelog links per product |
| `data.html` | Data stance: what each product keeps and sends |
| `about.html`, `privacy.html` | About Null Labs; privacy policy and credits |
| `terminal.html` | Keyboard-only downloads (nullgrid.dev/terminal) |
| `backup.html` | Plain backup downloads page |
| `download-*.html` | Redirects to each product's `#download` section |
| `*.mp4`, `*-poster.jpg`, `*.png` | Tour videos and screenshots |

Download links point straight at each product's GitHub release.

## Publish
1. Push to the root of this repo's `main` branch.
2. Settings → Pages → Deploy from a branch → `main` / root.
3. Custom domain: `nullgrid.dev` (set by `CNAME`), Enforce HTTPS on.
4. DNS: `A` records for `nullgrid.dev` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`; `CNAME` for `www` → `null0grid.github.io`.

© NULL LABS. All rights reserved.
