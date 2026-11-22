# pictus-public

Public website of [Pictus](https://getpictus.app), an iPhone app that grows French vocabulary with illustrated words and spaced repetition. GitHub Pages serves this repository from `main` at `getpictus.app` (see `CNAME`).

## Pages

- [`index.html`](index.html) - landing page: logo, tagline, App Store badge.
- [`confidentialite/index.html`](confidentialite/index.html) - privacy policy and legal notice, linked from the app's paywalls and its App Store listing.

## Assets

Everything but the App Store badge comes from the app repository (`../eloquent-app`), so the site keeps the app's look:

- `assets/logo.svg` - `assets/images/logo/pictus.svg`.
- `favicon.*`, `apple-touch-icon.png`, `assets/icon.png` - the `Classique` app icon, resized.
- `assets/mots/` - word illustrations from `content-generation/content-v1/`, resized to 360 px.
- `assets/app-store-badge.svg` - Apple's official French badge, from the App Store marketing toolbox.
- `assets/fonts/` - DM Serif Display and Inter, the app's fonts (SIL Open Font License, texts alongside). Self-hosted so that no visitor data reaches Google Fonts, in line with the privacy policy.

Colors are the app's design tokens (`src/constants/theme.ts`).

## Preview locally

```bash
python3 -m http.server 8765
```
