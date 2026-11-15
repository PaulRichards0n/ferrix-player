# Ferrix Player website

A static single-page site for **Ferrix Player**, the Windows IPTV player.

**Live:** https://paulrichards0n.github.io/ferrix-player/  
**Repository:** https://github.com/PaulRichards0n/ferrix-player

## Contents

- `index.html` — the whole site (styles and lightbox script are inline)
- `preview.png` — screenshot of the light theme
- `ferrix_player_live_tv_for_windows_retro_crt_edition.html` — alternate retro/CRT edition (not linked from the main page)
- `assets/` — screenshots, icon and favicon
- `downloads/`
  - `FerrixPlayer-1.0.0-win64.zip` — portable bundle (exe, icon, help, readme, checksums)
  - `FerrixPlayer.exe` — bare executable for advanced users
  - `SHA256SUMS.txt` — checksums for the ZIP and exe

## Open it

Double-click `index.html`. Everything is relative and works offline; no server or
build step is needed.

To publish it, upload the contents of this folder to any static host (GitHub
Pages, Netlify, Cloudflare Pages, IIS, nginx, …). Keep the `assets/` and
`downloads/` folders next to `index.html`. This copy is published with GitHub
Pages from the `main` branch at the URL above.

## Refresh the download

After rebuilding Ferrix Player:

1. Copy `MoondoggieTV-Windows\dist\FerrixPlayer.exe` to `downloads\FerrixPlayer.exe`.
2. Rebuild the portable bundle with `FerrixPlayer.exe`, `app.ico`, `help.png`,
   `README.txt` and `SHA256SUMS.txt` at the root of the ZIP.
3. Update the sizes and SHA-256 values in `index.html` and
   `downloads/SHA256SUMS.txt`.
4. Replace the files in `assets/` if the screenshots changed.
5. Commit and push; GitHub Pages rebuilds automatically.

The main page has no analytics or cookies; the only third-party link is the
optional VLC download.
