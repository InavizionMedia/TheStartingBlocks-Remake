
## Round 7 (Jon, 2026-10-04)
- Process section (01-04): scroll-driven timeline — red spine fill tracks scroll progress via rAF-throttled scroll listener, each step gets .is-active (blue→red numeral + entrance) via IntersectionObserver at 0.28 threshold; reduced-motion shows all steps statically. Verified functionally in headless Chromium (steps 0→4 active, progress 0→1 through the section) — the builder's QA-critic P0 was a false alarm from a truncated source review.
- Link preview: og:title/description/image/url/type + twitter:card(summary_large_image) tags added; og:image = https://agentzlab.github.io/TheStartingBlocks-Remake/assets/screenshot.png. Verified live on the Pages URL (200) and the screenshot serves current (442987 bytes).
- Republished: index.html + fresh hero screenshot pushed to main (commit c3dc180), live on Pages.
