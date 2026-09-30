# elepe.tech

Static landing page (plain HTML/CSS/vanilla JS), hosted on Donweb/Ferozo. Live at https://elepe.tech.

## Layout

- `index.html` (repo root) and `public_html/index.html` must always be identical. `public_html/` is what gets deployed.
- Demo media lives in `assets/demos/` and `public_html/assets/demos/` (GIFs only; source MP4s stay untracked and are never deployed).
- The `.dc.html`, `support.js` and `image-slot.js` files are Claude Design sources, not deployable.

## Change workflow (mandatory)

For every change requested:

1. Make the change in the repo, keeping `index.html` and `public_html/index.html` identical (and any asset copied to both places).
2. Test it (in the browser when possible) before reporting it done.
3. Commit it (do not commit `*.mp4`). Push only when the user asks.
4. Tell the user exactly which files changed, using their `public_html/`-relative paths.
5. The user uploads only those files to `/public_html/` via the Ferozo file manager. Never instruct a full wipe-and-reupload for a small change.
6. If many files changed, regenerate `elepe-tech-site.zip` from `public_html/` with forward-slash paths (Python `zipfile`, not PowerShell `Compress-Archive`). Extracting it over `/public_html/` overwrites matches and deletes nothing.
7. Remind the user to hard-refresh (Ctrl+F5) after uploading. If a same-named GIF is replaced and the old one keeps showing, rename the file (e.g. `-v2`) and update the reference.

Do not edit files on the server or upload via FTP without the user's explicit go-ahead each time.
