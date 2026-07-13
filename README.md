# Protein Gap

**Log a meal, get the ONE longevity nutrient you're most likely missing today.**

A tiny, single-file web app. No build step, no backend, no account - your log lives in `localStorage` on your device. Type what you ate in plain English ("salmon, spinach, brown rice") and Protein Gap scans it against six longevity pillars, then surfaces the single highest-priority gap with the easiest fix.

![Protein Gap - light and dark](docs/preview.png)

## Why

Most diet apps make you weigh food and count calories. You don't need that to live longer - you need to reliably hit a handful of nutrient pillars every day. Protein Gap tracks coverage, not calories, and only ever tells you the *next* thing to fix.

## The six pillars

Prioritised by how commonly people miss them:

1. **Omega-3 (EPA/DHA)** - oily fish, chia, flax, walnuts
2. **Fermented foods** - yogurt, kimchi, kefir, miso
3. **Leafy greens** - spinach, kale, rocket
4. **Fiber** - beans, lentils, oats, whole fruit
5. **Colour + polyphenols** - berries, peppers, cocoa, matcha
6. **Protein** - eggs, fish, tofu, greek yogurt

The nutrient model is a transparent keyword map (Layne Norton / Huberman / Blueprint flavoured), all in `index.html` - edit it to taste.

## Features

- Daily meal logging with instant pillar detection
- Circular coverage ring + "today's gap" focus card
- Per-meal breakdown of which pillars each meal covered
- This-week strip with a logging streak
- Light + dark themes (auto / light / dark toggle)
- 100% offline, one HTML file, zero dependencies

## Run it

Open `index.html` in a browser. That's it.

Or serve it:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy (GitHub Pages)

Settings -> Pages -> deploy from `main` / root. Done.

## Stack

Vanilla HTML/CSS/JS. Space Grotesk + Manrope. SVG progress ring. CSS `backdrop-filter` glass. No frameworks.

## License

MIT
