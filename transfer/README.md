# transfer/ — hand-off folder for the website

This branch (`transfer`) is a drop box between Claude conversations. Any conversation working on a
Null Grid app puts files here that the **website conversation** (nullgrid.dev) should use: videos,
screenshots, posters, release notes, copy, checksums.

It lives on its own branch on purpose: GitHub Pages publishes `main`, so nothing here goes live until
the website conversation copies it onto a page and the owner says "push it".

## Layout

One folder per app (`null-scribe/`, `node-grid/`, `null-notes/`, `null-drive/`) or `suite/` for
anything shared. Each folder has a `NOTES.md` that says what the files are and where they should go.

## Adding files (any conversation)

```
git clone --branch transfer --single-branch --depth 1 https://github.com/Null0Grid/nullgird.dev transfer-wt
cd transfer-wt
# add files under transfer/<app>/, update transfer/<app>/NOTES.md and the log below
git add -A && git commit -m "<app>: <what>" && git push origin transfer
```

## Taking files (website conversation)

```
git fetch origin transfer
git checkout origin/transfer -- transfer/<app>/<file>   # then move it where the page needs it
```

After a file is on the site, mark it **used** in the log (or delete it from this branch).

## Log

| Date | App | Files | For | Status |
|---|---|---|---|---|
| 2026-10-22 | Null Scribe | `null-scribe/null-scribe-demo.mp4`, `.webm`, `-poster.jpg` | Demo video for `scribe.html` | new |
| 2026-10-22 | Null Drive | `null-drive/null-drive-feature-demo.mp4`, `null-drive/null-drive-server-setup.mp4` | Feature tour and server setup videos for `drive.html` (see `null-drive/NOTES.md`) | new |
