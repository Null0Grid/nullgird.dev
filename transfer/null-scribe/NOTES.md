# Null Scribe → website

## Demo video (2026-10-22)

| File | What |
|---|---|
| `null-scribe-demo.mp4` | 1920×1080, 30 fps, H.264, 1:34, no audio, 3.9 MB, faststart |
| `null-scribe-demo.webm` | Same video, VP9, 3.4 MB |
| `null-scribe-demo-poster.jpg` | First frame (title card), for `poster=` |

Captioned walkthrough of Null Scribe 5.1: Meeting mode (Discord + Zoom in, Spotify out), live transcript
(sped up 4×, the caption says so), on-device processing, the summary, renaming "Discord" to "Tom",
summary templates + custom words in Settings, the Download menu (PDF, subtitles, audio) and Send to Notes,
then an end card with the platforms and nullgrid.dev.

The UI is the real app; the recording replays the sample "Q4 Budget Review" meeting, and its summary is
the prepared sample summary, so don't caption it as a live recording.

Suggested placement: `scribe.html`, near the top, matching the existing `null-grid-tour.mp4` /
`null-notes-tour.mp4` treatment. Embed:

```html
<video autoplay muted loop playsinline preload="metadata" poster="null-scribe-demo-poster.jpg" width="1920" height="1080">
  <source src="null-scribe-demo.webm" type="video/webm">
  <source src="null-scribe-demo.mp4" type="video/mp4">
</video>
```

## Current release (for download tables)

- Latest: **v5.1.1** (2026-10-22, new app icon), https://github.com/Null0Grid/null-scribe/releases/tag/v5.1.1
- 17 files + `SHA256SUMS` (use that file for the site's SHA-256 table):
  `null-scribe_5.1.1_amd64.deb` / `_arm64.deb`, `null-scribe-5.1.1.x86_64.rpm` / `.aarch64.rpm`,
  `NullScribe-5.1.1-x86_64.AppImage` / `-aarch64.AppImage`, `null-scribe_5.1.1_x64.tar.gz` / `_arm64.tar.gz`,
  `null-scribe_5.1.1_x86_64.flatpak` / `_aarch64.flatpak`, `null-scribe_5.1.1_amd64.snap` / `_arm64.snap`,
  `null-scribe-bin.PKGBUILD` + `.SRCINFO` (AUR), `dev.nullgrid.scribe.flathub.yml`,
  `NullScribe-5.1.1-Setup.exe`, `NullScribe_5.1.1.0_x64.msix` (Store package; link the Store, not this file).
- Install commands: see the release notes table on GitHub.
