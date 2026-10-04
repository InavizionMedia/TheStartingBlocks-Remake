# CURSOR-BLUEPRINT.md — The Starting Blocks Redesign

Living briefing for anyone building on this repo. Newest entry wins.

## What this is

A redesign **draft** (not live, not client-approved) of https://thestartingblocks.com/ —
Yolando Mitchell Brown's done-for-you one-page website service.
Private repo. GitHub Pages serves `main` as a preview link for Jon's review only.
**Do not contact Yolando. Do not touch the live WordPress site.**

## Source of truth

- The Muse web artifact `the-starting-blocks-redesign-draft` is the build surface.
- `index.html` at repo root is the **exported artifact** — never hand-edit it.
- Change flow: `artifact.edit` → verify → `artifact.export` → push export as `index.html` → refresh `assets/screenshot.png` → update this log line.

## Design tokens (her brand — do not restyle to Jon's charcoal)

- Headings: **Prata** (serif). Body: **Roboto**.
- Red primary `#E02B20`; CTA buttons `#ff0000`, uppercase, letter-spacing 1px, radius 5px.
- Blue secondary `#2EA3F2`. Deep navy `#0B1B33` for portfolio/pricing feature surfaces.
- Warm light page background, near-black text. Emoji icon language used deliberately (✅ 💰 💳 🎯 🔒).

## Locked content facts (from her live page — do not invent alternatives)

- Pricing: **$297** one payment (light card) / **$157 × 2** (dark navy featured card). Feature lists carry her full descriptions. "Click Here" buttons → her PayPal link `https://www.paypal.com/ncp/payment/UTSVJPJFQ6SQ4`.
- Timeline: 7–10 business days. Revisions: 1 included, within 3 days.
- Videos: Vimeo `1120977751` ("One page website is all you need"), YouTube `RCUzzoS8HO4` ("How I Got My Start") with the full-bleed custom poster.
- Contact email on record: `hellostart@startthepossible.com` (domain mismatch vs site — flagged, unresolved).
- Service copy under the first video is hers **word-for-word** — do not paraphrase, do not duplicate elsewhere.

## Open questions for Yolando (do not fill in — flag)

1. Actual transaction fee percentage (her Terms had an `[insert fee percentage]` placeholder).
2. Email domain mismatch (site vs `startthepossible.com`).
3. `$157 × 2` vs her "third and final payment" note — draft uses ×2.

## Conventions

- New branches per round (`redesign-round-N`); merge to `main` only on Jon's approval.
- `assets/screenshot.png` refreshes on every build change.
- Decisions append to `docs/decision-log.md` with dates.
