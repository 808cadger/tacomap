# TacoMap — Taco & Latin Food Spots Across America

## Download Links

- **iOS / iPhone:** Open the PWA in Safari: [TacoMap iOS install](https://808cadger.github.io/tacomap/) and choose **Share -> Add to Home Screen**.
- **Android:** Download the latest APK from GitHub Releases: [TacoMap Android releases](https://github.com/808cadger/tacomap/releases/latest).
- **Source download:** [Download the GitHub source ZIP](https://github.com/808cadger/tacomap/archive/refs/heads/main.zip).


<!-- INSTALL-START -->
## Install and run

These instructions install and run `tacomap` from a fresh clone.

### Clone
```bash
git clone https://github.com/808cadger/tacomap.git
cd tacomap
```

### Web app
```bash
npm install
python3 -m http.server 8080
```

### Android build/open
```bash
npm run cap:sync
npm run cap:android
```

### Notes
- Use Node.js 22 or newer for the current package set.
- Android builds require Android Studio, a configured SDK, and Java 21 when Gradle is used.

### AI/API setup
- If the app has AI features, add the required provider key in the app settings or local `.env` file.
- Browser-only apps store user-provided API keys on the local device unless a backend endpoint is configured.

### License
- Apache License 2.0. See [`LICENSE`](./LICENSE).
<!-- INSTALL-END -->


[![Last Commit](https://img.shields.io/gitea/last-commit/cadger808/tacomap?gitea_url=https%3A%2F%2Fcodeberg.org&label=last+commit&color=f97316&style=flat-square)](https://codeberg.org/cadger808/tacomap)
[![PWA](https://img.shields.io/badge/platform-PWA-f97316?style=flat-square)](https://cadger808.codeberg.page/tacomap)

> Find the best tacos near you — from Hawaii to NYC. Plan a taco crawl in minutes.

TacoMap surfaces authentic taco and Latin food spots using live OpenStreetMap data. Explore regional taco scenes, save your favorites, and build a taco crawl route with one tap.

## Features

- Live taco & Latin food spots via OpenStreetMap Overpass API
- Regional scene explorer — Hawaii, LA, Texas, NYC, Chicago, Miami
- Taco crawl planner — build a multi-stop route
- Save favorites to device
- PWA — installs in one tap, works offline for saved spots

## Stack

`Vanilla JS` · `HTML/CSS` · `OpenStreetMap Overpass API` · `Capacitor` · `PWA`

## Install

[**Live App →**](https://cadger808.codeberg.page/tacomap) · [**Download APK →**](https://codeberg.org/cadger808/tacomap/releases/download/v1.0.0/TacoMap-v1.0.0.apk) · [Releases](https://codeberg.org/cadger808/tacomap/releases)

## Deploy

```bash
npm install
npx cap sync android
cd android && ./gradlew assembleDebug
```

Built by [cadger808](https://codeberg.org/cadger808) · Pearl City, Hawaii
