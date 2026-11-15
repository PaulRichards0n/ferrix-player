# Ferrix Player website

A static single-page site for **Ferrix Player**, the Windows IPTV player.

## Contents

- `index.html` — the whole site (styles and lightbox script are inline)
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
`downloads/` folders next to `index.html`.

## Refresh the download

After rebuilding Ferrix Player:

1. Copy `MoondoggieTV-Windows\dist\FerrixPlayer.exe` to `downloads\FerrixPlayer.exe`.
2. Rebuild the portable bundle with `FerrixPlayer.exe`, `app.ico`, `help.png`,
   `README.txt` and `SHA256SUMS.txt` at the root of the ZIP.
3. Update the sizes and SHA-256 values in `index.html` and
   `downloads/SHA256SUMS.txt`.
4. Replace the files in `assets/` if the screenshots changed.

The page has no analytics, cookies or external dependencies.
