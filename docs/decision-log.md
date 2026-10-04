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
