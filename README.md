# BOL-RUNNER

BOL-RUNNER is a mobile-friendly Dino-style web game where gameplay unlocks a spaghetti bolognese recipe.

## What it is

- A Chrome Dino-inspired runner themed around spaghetti bolognese
- The full recipe unlocks progressively based on high score
- Full unlock target: **2000**
- Includes mobile fullscreen mode, PWA install support, and offline caching

## App description

Only the skilled can unlock the secret sauce.
Get highscore of 2000 and the recipe is yours.

## How we built it (brief)

1. Started from a static web app shell (`index.html`) hosted on Cloudflare Pages.
2. Embedded and customized the Chromium Dino runner in `trex/`.
3. Wired runner score/high score to the host page for recipe unlock logic.
4. Replaced visuals with custom BOL-RUNNER branding and food-themed sprite sheets.
5. Added mobile UX features: touch/audio handling, fullscreen fallback, and install button.
6. Added PWA capabilities: manifest + service worker (`sw.js`) for offline use.
7. Iterated with frequent Git commits/tags and Cloudflare Pages deploys.

## Deploy

- Production: https://bol-runner.pages.dev
- Platform: Cloudflare Pages (static site)

## Key files

- `index.html` - main UI, controls, unlock/progress logic
- `trex/index.js` - runner engine customizations and score/night logic
- `trex/index.css` - runner visuals and inverted/night styling
- `sw.js` - offline cache service worker
- `site.webmanifest` - PWA manifest
