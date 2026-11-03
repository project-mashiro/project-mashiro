# Mashiro’s sticker drawer

[Back to the profile](https://github.com/project-mashiro)

## Active theme: Orbit Shrine

The selected design 07 uses an original radial composition: Mashiro sits in a scalloped lilac center, with public GitHub statistics in petal satellites, orbit rings, and floating personality stickers. The profile image opens Mashiro’s repositories. Separate artist and workflow cards are native links.

| Purpose | Asset |
| --- | --- |
| Orbit artwork and editable template | `orbit-shrine.svg` |
| Current generated image | `orbit-shrine-live-*.svg` |
| Public count snapshot | `orbit-shrine-stats.json` |
| Linked artist credit | `shrine-os-artwork-credit.svg` |
| Linked workflow footer | `shrine-os-footer.svg` |
| Material Symbols license | `LICENSE-material-symbols.txt` |

## Automatic public statistics

The [Refresh Orbit Shrine stats workflow](../.github/workflows/shrine-stats.yml) runs daily at 23:23 UTC (06:23 Asia/Bangkok), with a manual run in Actions. It updates the SVG template, creates a content-addressed image, and points the root README to that image. Only the latest generated Orbit image is retained. A new filename prevents stale GitHub image caches.

- **Contributions:** GitHub’s contribution-calendar total for the last year.
- **Month commits:** commit contributions in the current UTC month, not an all-time total.
- **Public repo:** public repositories owned by this profile.

The workflow uses the repository’s built-in `GITHUB_TOKEN`, with write access scoped to the refresh job. No personal access token or private-repository data is needed. API errors preserve the published artwork; unchanged counts do not cause an extra commit. Public contribution counts can take time to settle. Scheduled runs may be delayed or disabled after 60 days without repository activity; manual runs remain available.

## Artwork credit

Mashiro character and emote artwork by **[@fuffi_fufi](https://x.com/fuffi_fufi)**. Original supplied emotes are preserved; a still PNG is embedded in the SVG so reduced-motion can stop the complete scene.

Icons are genuine **Google Material Symbols Rounded**, embedded as vector paths under Apache-2.0. See `LICENSE-material-symbols.txt`.

## Motion and earlier themes

The self-contained SVG has rotating petal shapes, floating Mashiro artwork, and a moving wave. It uses no scripts, remote fonts, external image dependencies, or `foreignObject`. System reduced-motion preferences stop autonomous CSS loops. The SVG loops are a GitHub-image adaptation of Expressive Motion, not live Qt spring physics.

The `shrine-os-*` surfaces and earlier `*-v2.svg` / hero / WebP assets remain available for reuse. They are historical themes; the active daily workflow updates only Orbit Shrine.
