# Iron Ledger — hosting kit

Everything in this folder is ready to upload as-is. `index.html` is the full app (same build as the
single file), already wired to `manifest.webmanifest`, the icons and `sw.js`.

## Put it online (free, any of these)
GitHub Pages, Cloudflare Pages or Netlify. Upload the whole folder; a sub-path is fine
(e.g. `username.github.io/iron-ledger/`). It must be served over HTTPS.

## Install on the phone
Delete any old shortcut first (icons are cached at install time), then:
- **iOS / iPadOS**: Safari → Share → Add to Home Screen
- **Android**: Chrome → ⋮ → Add to Home screen / Install app (Samsung Internet: menu → Add page to → Home screen)

## Bring your data across
A hosted copy has its own storage, separate from the file you open locally. On your current copy,
System → **Export the Ledger**; then open the hosted app and System → **Import** that file (Replace or Merge).

## Updating
Replace `index.html` with a newer build and bump `VERSION` in `sw.js` so phones pick it up.
(The kit generator stamps `VERSION` with the app version automatically.)

**A local file can't get this icon.** Phones only apply home-screen icons to a page served over http(s).

## Palette
Background `#121519` → `#2C323A` · Brass `#D4AA5E` · Steel `#EEF1F4` → `#6D757F`
