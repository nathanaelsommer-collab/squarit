# SquarIt

A Pythagorean field calculator for squaring up rectangular layouts — foundations,
decks, fences, anything staked out with string lines. Enter any two of the two
sides and the diagonal; it solves the third live, draws the layout to scale, and
tells you which stake to swing (and how far) to square the corner.

Built as an installable, offline-first progressive web app: add it to your home
screen and it works with zero cell signal.

## Use

Open `index.html` (or the deployed GitHub Pages site):

1. Enter any two values — **A** (long side), **B** (short side), **C** (diagonal) —
   in feet, inches, and sixteenths.
2. The third calculates live, shown in feet/inches to the 32nd.
3. Pick **Option 1** (swing the TL stake) or **Option 2** (swing the BR stake) to
   see how far to move it along its compass arc to square the corner.
4. Toggle the math steps to see the full Pythagorean work.

## Files

- `index.html` — the app (canonical; this is what the Pages site serves)
- `manifest.json` — PWA manifest (name, icons, theme)
- `service-worker.js` — offline cache; bump `CACHE_VERSION` to force updates
- `icon.PNG` — app icon
- `square-calculator.html` — older near-duplicate of `index.html`, kept for
  backward compatibility with existing bookmarks

## Deploy

Hosted with GitHub Pages from the `main` branch. Any push to `main` goes live
within a minute or two; the service worker refreshes clients in the background.
