# Wosmo logo

Shared brand assets, served straight off this repo via jsDelivr's GitHub CDN
instead of being copied into every app.

| File            | What it is                                   |
| --------------- | --------------------------------------------- |
| `wordmark.svg`  | Full "wosmo" wordmark, white fill (dark bg)   |
| `wordmark.png`  | Raster export of the wordmark, 1293×261       |
| `mark.svg`      | "W" monogram only, white fill (dark bg)       |

`mark.png` is intentionally not included yet — it needs a real SVG rasterizer
(e.g. `rsvg-convert`, Inkscape, or a browser-based renderer) to generate
correctly; QuickLook's thumbnailer silently produces a blank image for this
file's `<style>`-based fill, so don't use it for that.

## Usage

Reference assets directly from GitHub via jsDelivr — no build step, globally
cached:

```
https://cdn.jsdelivr.net/gh/Wosmos/wosmos@main/public/logo/wordmark.svg
https://cdn.jsdelivr.net/gh/Wosmos/wosmos@main/public/logo/mark.svg
```

`@main` responses cache for up to ~12h. For an instant, immutable URL, pin to
a commit SHA or a tag instead (e.g. `@v1`) and purge on update via
https://www.jsdelivr.com/tools/purge.
