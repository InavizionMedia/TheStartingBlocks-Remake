# DECISION LOG — Harvest Prompt first drive run (2026-10-04)

Jon delegated all decisions for this pass ("you make all the decisions... no need for my approval yet"). Every judgment call below is mine. Spots where the prompt's machinery would have asked its ONE question are marked [Q-SPOT], with my verdict on whether deciding beat asking — this is the prompt-iteration data for dialing the prompt in.

## Factual conflicts (prompt Part 2: omit or ask one question)

1. **Timeline: "by end of day" vs "7–10 business days"** [Q-SPOT]
   - Decided: 7–10 business days (FAQ = operational truth; end-of-day is marketing puff, implausible with content submission + queue).
   - Ask-vs-decide verdict: DECIDING was right for a first pass, but this is the canonical example of the prompt's one question being well spent — it's the highest-stakes unknown on the page. Next run: ask this one.
2. **Payments: "$157 × 2" vs "third and final payment"** [Q-SPOT]
   - Decided: $157 × 2 (the "third and final" line reads as a copy error; 2-payment math $314 > $297 works as a financing premium).
   - Verdict: deciding fine — low stakes, flagged for Yolando either way.
3. **Revision window: "3 days" vs "48 hours"**
   - Decided: 3 days (primary offer copy; friendlier).
   - Verdict: deciding fine.
4. **Scarcity "40 spots / limited time"** — unverified → DROPPED per refusal machinery (never invent scarcity). Replaced with honest queue note ("first come, first served").
   - Verdict: the refusal rule handled it — no question needed. Good.
5. **Terms "[insert fee percentage]" placeholder** — removed the bracket text; clause now reads "late payments may incur a fee as stated on your invoice." Flagged for Yolando's number.
6. **Copyright 2025 → 2026.**

## Creative decisions (all mine)

7. **Hero headline:** "Still Don't Have a Website? / We've Got You." — picked from the three competing headlines; it names the pain. One headline only.
8. **Primary CTA:** "Sign Up and Pay — $297". Secondary: free 15-min call (moved up from buried contact section).
9. **Palette:** charcoal #121210 + warm grays + gold #C9A227 (prompt defaults). [Q-SPOT] Real brand colors unverifiable — headless screenshot blocked by the site's host (ERR_EMPTY_RESPONSE), text fetch carries no color data.
   - Verdict: defaulting beat asking — Jon wouldn't know Yolando's palette offhand either; needs real brand assets next round.
10. **Portrait:** monogram "YB" placeholder in a gold-ring frame — clearly a photo slot, NOT a fake person (never invent a founder). [Q-SPOT]
    - Verdict: placeholder right for pass one; next round ask Jon for a real Yolando photo.
11. **One background metaphor:** track starting-block lane geometry (subtle SVG line motif). "Starting blocks" = the brand's own metaphor, earned not decorated.
12. **Brand reconciliation:** "The Starting Blocks" canonical; kept the real contact email hellostart@startthepossible.com (functional) — flagged the domain mismatch for Yolando (should mail move to @thestartingblocks.com?).
13. **Title tag:** "The Starting Blocks — Your One-Page Website, Done For You" (was 4 keyword phrases).
14. **Emoji strip:** removed all per-line ✅📅💰 emojis (guru-template slop tell).
15. **Pricing cards:** two cards, identical feature lists, honest "all sales final" note (their real policy, stated plainly).
16. **FAQ:** deduped the repeated questions (site asks "what do I provide" twice); kept the real ones.
17. **Motion:** subtle reveal-on-scroll only. Sales job here is trust, not spectacle — animation second.
18. **Testimonials:** kept all three, lightly condensed, names + businesses intact. Site-published (not independently verified) — no new claims added.

## Prompt-iteration notes (for dialing in)

- The **one-question rule** worked as designed on the timeline conflict — that's the question to spend it on. Consider: prompt should rank conflicts by stakes before asking.
- The **"flag, don't fill"** rule produced 5 clean flags (colors, photo, email domain, fee %, scarcity) without stalling the build. Keep.
- **Refusal machinery** (drop unverified scarcity) fired correctly with zero deliberation — the strongest pattern in the set.
- Gap: prompt has no rule for **brand/email domain mismatch** (Start The Possible vs The Starting Blocks). Candidate addition: "if the contact email domain differs from the site domain, flag it."
- Gap: **screenshot/visual review** isn't in the prompt — palette and imagery were decided blind. Candidate addition: a visual-reference step (attach screenshot or brand assets) before Part 5.

## CORRECTION — light version in her colors (Jon, 2026-10-04)

Jon redirected: this is Yolando's site, not his — his personal charcoal/gold taste does not apply. The build is now a LIGHT version in her actual brand scheme.

**Her real palette** (extracted from thestartingblocks.com's Divi theme CSS, not guessed): accent red **#E02B20** (theme customizer accent — links, buttons, footer headings, menu highlights), white backgrounds, near-black text. The site is light and warm; the earlier charcoal/gold was my default, not her brand.

**New tokens:** bg warm white #FDFCFA · panels #F7F5F1 · ink #1A1A1A · muted #6B6560 · accent #E02B20 · hairlines rgba(224,43,32,.14). Red used sparingly — many small touches, never large areas.

**Prompt-iteration note:** this validates the "visual-reference step" gap flagged above — the prompt needs a rule to pull the real palette (theme CSS / screenshot / brand assets) before art direction, instead of falling back to defaults. Defaults silently applied the wrong taste. New candidate rule: "extract the site's actual accent color from its theme CSS or a screenshot; never default to the builder's house palette on someone else's brand."

## Round 2 — full asset migration (Jon, 2026-10-04)

Jon: "I need all the info and assets from her current page into our new design."

- **Blue restored.** Her site is red + blue; the light rebuild had dropped the blue. New rule: red #E02B20 primary (~70%), blue #2EA3F2 secondary (~30%: links, secondary buttons, markers, video frames). Confirmed from her Divi CSS that #2ea3f2 is live on her page, not just a Divi default assumption.
- **Pricing → tables like hers.** Rebuilt as two tables with checkmark rows per feature (SVG checks, no emoji), $297 featured with red border.
- **Her real logo** in the nav (Copy-of-Divi-text-logo-1.png).
- **Her profile photo** (uploaded by Jon) in hero + About. Hosted temporarily on Muse file storage (expires 2026-10-06) — production must self-host.
- **Portfolio section added** — "What We've Built" with her 9 client site images (was missing entirely from pass 1; her live site leads with it).
- **Testimonial avatars** — her real hart/mk/kits images next to each quote.
- **Both videos embedded** — Vimeo "One page website is all you need" (player.vimeo.com/video/1120977751) after What-you-get; YouTube "How I Got My Start" (youtube.com/embed/RCUzzoS8HO4) in About.
- All her-site images hotlink to thestartingblocks.com for the draft; flagged in code comments to self-host for production.

**Prompt-iteration note:** pass 1 was text-only and missed the entire visual layer (photos, portfolio, videos, logo, secondary color). The prompt needs an "asset inventory" step: extract images, embeds, and the full color story from the source BEFORE building — not just copy. Text-first drafting lost half the site.
