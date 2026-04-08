# TacoMap - Taco & Latin Food Finder (US + Hawaii Scenes)
Live taco spots via OpenStreetMap Overpass API. GPS finder, regional scenes (Hawaii/LA/Texas/NYC), taco crawl planner, favorites. PWA/Capacitor. Haiku chat.

Repo: https://github.com/808cadger/tacomap. Dev: cadger808 (Pearl City, HI).

## Stack & Design System
- Frontend: Vanilla JS (index.html, api-client.js, avatar-widget.js)
- Mobile: Capacitor (android/, capacitor.config.json, geolocation)
- PWA: manifest.json, sw.js (O(1) region index)
- APIs: OpenStreetMap Overpass (tacos/Latin food), Claude Haiku (chat)
- Design: Claude parchment #f5f4ed, Terracotta #c96442 "Taco Crawl" CTAs

## Key Files & Taco Pipeline
api-client.js (Overpass) | avatar-widget.js (Haiku) | index.html (map/regions)

## Commands
npm install
npx cap sync android && cd android && ./gradlew assembleDebug
npx serve .

## Code Rules — Taco Location Pipeline
- **Pipeline**: GPS → Overpass "taco OR 'latin food'" → Filter (Hawaii/LA/Texas/NYC/Chicago/Miami) → Region rank → Taco crawl route
- **Regional Scenes**: Hawaii (local), Texas (authentic), LA/NYC (fusion), Chicago/Miami
- **#ASSUMPTION**: Geolocation permission; TODO: manual zip entry
- **Favorites**: Offline localStorage with route export
- **O(1) Index**: Region pre-filter (sw.js), Capacitor GPS accuracy
- **Phases**: MVP (map+regions) → Ratings → AR directions → Taco reviews

## AI Prompts — Taco Critical

## Claude Workflow (Auto-Debug ON)
1. Read CLAUDE.md + api-client.js first
2. /doctor → GPS/SW cache check
3. "Overpass query correct? Regional ranking? Crawl route optimal?"
4. Review: Geolocation accurate? Offline favorites? Hawaii-first?
5. Output: "Debug complete" + patches
6. Commit: "feat: [map|regions|crawl|gps] [desc]"

## Deploy Checklist

**15/15 cadger808 factory**. TacoMap = perfect local-first app (Pearl City origins). **Taco crawl planner** with Haiku chat = viral Hawaii launch. Your empire spans AI skincare → construction safety → **taco discovery**. **Commit → TacoMap ships.** 🌮📍
