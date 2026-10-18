# nuvio-aspect-badges

Aspect-ratio stream badges for [Nuvio](https://github.com/NuvioMedia). They flag streams whose release name or filename states a ratio, so you can spot sources that fill a 16:9 screen and ones that show black bars.

## Import URL

```
https://raw.githubusercontent.com/shreyas-bangera/nuvio-aspect-badges/main/aspect-badges.json
```

In Nuvio: **Settings > Layout > Streams > Fusion Badge URLs** (on some versions: **Settings > Streams > Stream Badges**), paste the URL above and import.

## Badges

| Badge | Colour | Matches |
| --- | --- | --- |
| 16:9 FULL | green | `16:9`, `1.78:1`, `full frame`, `unmatted`, `expanded aspect/ar/ratio`, or 3840x2160 / 2560x1440 / 1920x1080 / 1280x720 |
| ~16:9 (1.85) | light green | `1.85` / `1.85:1`, or 3840x20xx-21xx / 1920x10xx (tiny bars) |
| BARS 2.39 | red | `2.35`, `2.39`, `2.40` (optionally `:1`), `scope`, `cinemascope`, or sizes such as 3840x1600, 2560x1080, 1920x800 |
| BARS 21:9 | red | `21:9`, `21x9`, `ultrawide` |
| 1.43:1 SIDES | orange | `1.43` / `1.43:1` (bars on the left and right) |
| 4:3 SIDES | orange | `4:3`, `1.33:1` (bars on the left and right) |

## Notes

- Badges only appear when the stream text actually states a ratio or pixel size. Most Torrentio and MediaFusion results do not, so most streams get no badge from this pack.
- Size matches are guarded so file sizes like `2.40 GB` do not trigger a badge.
- IMAX, IMAX Enhanced and OPEN MATTE badges are not included. Use the [Kingsize badge pack](https://github.com/kingsizew/badges) alongside this one for those.
- For streams with no badge, use the player's Crop / Fill aspect mode (or your TV's Zoom mode) to remove black bars.
