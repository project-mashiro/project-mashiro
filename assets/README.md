# The sticker drawer

Self-contained artwork for [Mashiro’s profile](../README.md).

## M3 Expressive components

| Component | Files |
| --- | --- |
| Welcome | `mashiro-hero.svg`, `mashiro-hero-still.svg` |
| Section bars | `ritual-heading-v2.svg`, `rules-heading-v2.svg` |
| Mood cards | `mood-adorable-v2.svg`, `mood-supervise-v2.svg`, `mood-nap-v2.svg` |
| Personality cards | `identity-v2.svg`, `affection-v2.svg` |
| Shrine-rule cards | `offerings-v2.svg`, `personal-space-v2.svg` |
| Native link artwork | `projects-link-v2.svg`, `quiet-link-v2.svg` |
| Closing surface | `goodbye-v2.svg` |
| Original animated copies | `mashiro-blep.webp`, `mashiro-slipper.webp`, `mashiro-nap.webp` |

The README uses individual image cards so they wrap naturally in GitHub’s layout. Its two graphic navigation cards are wrapped in native links; their alt text describes the destinations. The hero references the verified artwork revision to avoid stale GitHub image caching.

The supplied Mashiro emotes are preserved. The SVG cards embed small first-frame PNG copies, with motion applied to the sticker groups, so the reduced-motion media query can stop every autonomous loop in those cards. The original animated WebP copies remain available separately.

The lilac/pink/cream tonal surfaces, shaped artwork, 30/23/17/12 rounding, 32-unit page inset, and entry curves adapt the expressive-motion style to GitHub. Entry uses 400ms cubic-bezier(.05,.7,.1,1); accent nudges use cubic-bezier(.38,1.21,.22,1). Ambient loops approximate the expressive character; they do not reproduce live Qt springs.

SVGs use no scripts, remote fonts, foreignObject, or external image dependencies. System reduced-motion preferences stop their CSS animation. GitHub’s image host has no app-level performanceMode or noShapes control. The still welcome artwork is also linked from the profile.
