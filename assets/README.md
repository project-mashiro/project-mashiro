# The sticker drawer

[Back to Mashiro’s profile](../README.md)

## Active theme: Shrine OS

The profile uses the selected dark-plum M3 Expressive media layout. Its header, three native navigation links, public-activity panel, sleepy current-mode player, and footer are separate SVG surfaces.

| Component | Asset |
| --- | --- |
| Header | `shrine-os-header.svg` |
| Real navigation | `shrine-os-nav-overview.svg`, `shrine-os-nav-projects.svg`, `shrine-os-nav-offerings.svg` |
| Public activity | `shrine-os-overview.svg` (template), `shrine-os-live-*.svg` (current image) |
| Current mode | `shrine-os-mode.svg` |
| Footer | `shrine-os-footer.svg` |
| Public counts | `shrine-os-stats.json` |

The **Refresh Shrine OS stats** workflow runs daily at 23:23 UTC (06:23 Asia/Bangkok), and can also be started from the Actions tab. It reads GitHub’s public GraphQL data and updates the activity SVG, its count snapshot, and the README image reference when the figures or month change. A content-based image filename avoids stale GitHub image caches; only the latest generated image is retained.

The large counter is GitHub’s contribution-calendar total for the past year. The month counter is GitHub’s commit contributions in the current UTC month; it is not an all-time commit total. The repository counter counts public repositories owned by this profile. Contributions may take time to appear in GitHub’s API.

The workflow uses the repository’s built-in `GITHUB_TOKEN`, with write access scoped to its refresh job. It needs no personal access token and reads no private repositories. If the API fails, existing artwork is preserved. Scheduled GitHub workflows can be delayed and may be disabled after 60 days without repository activity; the manual run remains available.

## Artwork and motion

Icons are genuine **Google Material Symbols Rounded**, embedded as vector paths. Their Apache-2.0 license is bundled in `LICENSE-material-symbols.txt`. The Mashiro emotes come from the supplied artwork collection; originals are preserved.

The SVGs are self-contained: no scripts, remote fonts, foreignObject, or external image dependencies. Floating sticker groups and token-based pulse curves express Mashiro’s personality. System reduced-motion preferences stop their autonomous CSS loops. These are GitHub-image adaptations, not live Qt spring parity. The 30/23/17 rounding, layered aubergine surfaces, lilac accents, and pink tuna card retain the selected design.

Earlier hero, card, and animated WebP assets are retained for reuse.
