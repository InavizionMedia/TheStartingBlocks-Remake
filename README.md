# The Starting Blocks — Redesign Draft

> A full redesign draft of **thestartingblocks.com** — Yolando Mitchell Brown's done-for-you one-page website service for service-based businesses.

[![Last commit](https://img.shields.io/github/last-commit/agentzlab/TheStartingBlocks-Remake)](https://github.com/agentzlab/TheStartingBlocks-Remake/commits/main)
[![Repo size](https://img.shields.io/github/repo-size/agentzlab/TheStartingBlocks-Remake)](https://github.com/agentzlab/TheStartingBlocks-Remake)
[![Static site](https://img.shields.io/badge/site-static-blue)](https://github.com/agentzlab/TheStartingBlocks-Remake)

**Preview:** via the private Muse artifact for now — see below for the GitHub Pages note.

![Hero screenshot](assets/screenshot.png)

## What's inside

- Sticky navy nav with her exact 7 labels (Home, What We Do, Price, Your Site, FAQ, The Designer, Portfolio) + Price dropdown + polished mobile slide-in menu
- Hero: "Still don't have a website? We've Got You." with Yolando's portrait
- First video (Vimeo) + her six service descriptions, word-for-word, with her bold/red emphasis
- Founder's story: "How I Got My Start" with custom full-bleed thumbnail, click-to-play YouTube
- "Who We Build For" — six audience cards (Business Owners, Creators, Creatives, Entrepreneurs, Small Businesses)
- Pricing matching her real setup: **$297 light card** / **$157 dark featured card**, full feature copy, real PayPal checkout buttons
- "Your Journey" — Who This Is For / What's Included / What Your Site Will Have / What You'll Walk Away With / Free Prep Session
- "What We've Built" — full-bleed horizontal scroll-snap project showcase (9 projects)
- Testimonials with avatars, FAQ, contact with real email + free 15-min call CTA

## Design language

- Warm light background, near-black text
- Red primary `#E02B20` (buttons `#ff0000`), blue secondary `#2EA3F2`
- Deep navy `#0B1B33` for portfolio/pricing feature surfaces
- **Prata** serif headings + **Roboto** body — her actual brand fonts
- Her emoji icon language (✅ 💰 💳 🎯 🔒 …), used deliberately

## Tech stack

| Layer | Choice |
|---|---|
| Page | Single self-contained `index.html` (exported from the Muse web-artifact build) |
| Fonts | Google Fonts: Prata + Roboto |
| Video | YouTube + Vimeo embeds |
| Checkout | PayPal payment links (her real ones) |
| Hosting | GitHub Pages (pending — needs repo public or plan upgrade), no build step |

> **Pages note:** this repo is private on the free plan, which doesn't allow GitHub Pages.
> The live preview currently runs on the private Muse artifact. Flipping the repo public
> would enable `https://agentzlab.github.io/TheStartingBlocks-Remake/` — Jon's call.

## Project structure

```
├── index.html                  # the site (self-contained)
├── assets/
│   ├── screenshot.png          # README hero (refresh on every build change)
│   ├── yolando-portrait.jpg    # founder portrait
│   └── img/                    # supplied lifestyle, audience + video poster images
├── docs/
│   ├── CURSOR-BLUEPRINT.md     # builder briefing for future work
│   ├── audit.md                # source-site audit + resolved contradictions
│   ├── context-block.md
│   ├── decision-log.md         # every design decision, dated
│   └── prebuild-readouts.md
├── .nojekyll
└── README.md
```

## Workflow

- `main` = the live preview. Changes land on a new branch first (`redesign-round-N`), then merge when approved.
- Screenshots refresh on every build change — no stale screenshots.
- Nothing here touches the live WordPress site or goes to Yolando until Jon approves.
