# Null Drive → website

## Videos (2026-10-22)

| File | What |
|---|---|
| `null-drive-feature-demo.mp4` | Feature tour: 1600×900, 30 fps, H.264, 3:13, no audio, 4.9 MB, faststart, chapters built in |
| `null-drive-server-setup.mp4` | Setting up the server: 1600×900, 30 fps, H.264, 1:13, no audio, 1.4 MB, faststart, chapters built in |

Both have on-screen captions and are filmed from the real app (v5.1.1) on a running server. In the live-sync
and conflict scenes the real Linux desktop app syncs beside the web app. The terminal in the setup video is
a card with the real command and the server's real log lines.

**Feature tour chapters:** 0:00 Intro · 0:06 Your drive in the browser · 0:24 Upload and organise ·
0:45 Every version kept · 1:01 Recently deleted · 1:08 Live sync with the desktop app · 1:25 Conflicts keep both ·
1:40 Add devices · 1:50 Part of Null Grid · 2:03 Two-factor and the security log · 2:16 On your phone ·
2:22 End-to-end encryption · 3:03 Runs where you do · 3:08 Get it

**Server setup chapters:** 0:00 Intro · 0:04 Start the server · 0:20 Create the admin account ·
0:46 Connect a computer · 1:08 Next steps

Suggested placement on `drive.html`: the feature tour near the top; the setup video in the Server part of
the download section (next to the `docker run` quick-start). They're long and captioned, so use controls
rather than autoplay-loop:

```html
<video controls playsinline preload="metadata" width="1600" height="900">
  <source src="null-drive-feature-demo.mp4" type="video/mp4">
</video>
```

## Release notes for the download tables

- The site lists 5.1.0's `nulldrive-desktop-5.1.0-1.*.rpm` and `NullDrive-5.1.0-*.AppImage` as missing: they
  were built but not attached (a release-workflow bug, now fixed).
- **5.1.1** is ready on `main` but not released yet. When it is, its release adds those files plus
  `NullDrive-<v>-x86_64.flatpak` / `-aarch64.flatpak`, server snaps `nulldrive_<v>_amd64.snap` / `_arm64.snap`,
  `nulldrive_<v>_aur.tar.gz` (AUR PKGBUILDs for `nulldrive-bin` and `nulldrive-desktop-bin`) and the Flathub
  manifest `dev.nullgrid.NullDrive.yml`: about 30 files, all in its `SHA256SUMS.txt`. Use that file for the
  SHA-256 table.
- Web-app encryption needs HTTPS (or localhost); over plain http:// the web app now says so. Worth a line
  wherever the site mentions end-to-end encryption.
