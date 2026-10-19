# nullgrid.dev

The Null Grid website: Null Search, Null Grid, Null Notes and Null Drive.
*Your data. Your grid.*

Plain static HTML, no build step. Served by GitHub Pages from the `main` branch root.

| File | Page |
|---|---|
| `index.html` | Home |
| `about.html` | About: the slogan, how we build, who we are |
| `downloads.html` | Every download, plus SHA-256 checksums |
| `search.html`, `grid.html`, `notes.html`, `drive.html` | One page per app |
| `download.html` | Null Drive's detailed downloads (server, Docker, NAS, binaries) |
| `*.mp4`, `*-poster.jpg` | Tour videos for Null Grid and Null Notes |

Store and download links live in the `LINKS` list at the bottom of each page.

## Publish
1. Push these files to the root of this repo's `main` branch.
2. Settings → Pages → Deploy from a branch → `main` / root.
3. Custom domain: `nullgrid.dev` (this repo's `CNAME` file sets it), then tick Enforce HTTPS.
4. DNS at your registrar:
   - `A` records for `nullgrid.dev` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `null0grid.github.io`
5. Org Settings → Pages → verify `nullgrid.dev`.
