# TacoMap — Taco & Latin Food Spots Across America

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

[**Live App →**](https://cadger808.codeberg.page/tacomap) · [Releases](https://codeberg.org/cadger808/tacomap/releases)

## Deploy

```bash
npm install
npx cap sync android
cd android && ./gradlew assembleDebug
```

Built by [cadger808](https://codeberg.org/cadger808) · Pearl City, Hawaii
