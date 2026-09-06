# Leadership Tracker â€” Web

Static GitHub Pages assets for the **Leadership Tracker** mobile app.
This repo contains no application source code.

## Contents
- **`picker.html`** â€” Google Picker bridge. Opened in the system browser by the
  app to let a user select their Google Drive folder, then returns the folder
  selection to the app via a custom URL scheme.
- **`privacy.html`** â€” Privacy policy for the app (linked from the Google Play
  and App Store listings).

## Hosting
Served via GitHub Pages at `https://leadershiptracker.app/` (custom domain; the old `shapirobh.github.io/leadership-tracker-web/` URLs 301-redirect).
Pushing to `main` publishes automatically.

## Badge assets (`badges/`)

Store badges for the landing page and for outbound email. Both are the official
assets and neither is recolored, re-lettered, or cropped.

- **`google-play-badge.png`** (646x250) is Google's official "Get it on Google Play"
  web badge, downloaded unmodified. Its uniform 41px transparent margin is the
  clear space Google requires, so the visible badge is 67.2% of the canvas height.
- **`app-store-badge.svg`** is Apple's official "Download on the App Store" badge
  from Apple Marketing Tools, unmodified. It carries no clear space of its own.
- **`app-store-badge.png`** (420x180) is that SVG rasterized at 3x on a transparent
  canvas whose clear space matches Google's proportions. Clear space was *added*;
  the artwork itself is untouched.

The two PNGs are built so that a single shared height aligns them: at
`height="60"` each visible badge is about 40px tall. Link them only to the live
store listings, keep the proportions, and keep the alt text exactly
"Get it on Google Play" and "Download on the App Store" so the links still work
for readers whose mail client blocks remote images.
