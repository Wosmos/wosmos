# Wosmo logo

Shared brand assets, served straight off this repo via jsDelivr's GitHub CDN
instead of being copied into every app.

| File                     | What it is                                  |
| ------------------------ | -------------------------------------------- |
| `wordmark.svg`           | Full "wosmo" wordmark, white fill (dark bg)  |
| `wordmark.png`           | Wordmark raster, 1024px tall (alias of `wordmark-1024.png`) |
| `wordmark-{128,256,512,1024}.png` | Wordmark raster at fixed heights    |
| `mark.svg`               | "W" monogram only, white fill (dark bg)      |
| `mark.png`               | Monogram raster, 1024px tall (alias of `mark-1024.png`) |
| `mark-{128,256,512,1024}.png` | Monogram raster at fixed heights          |
| `favicon.ico`            | Monogram, padded to a square, multi-res (16/32/48/64/128/256) |

All PNGs are transparent — they're white-fill artwork meant for dark
backgrounds, generated straight from the SVGs with `rsvg-convert` (not
resized copies of each other, so each size stays crisp).

## Usage

Reference assets directly from GitHub via jsDelivr — no build step, globally
cached:

```
https://cdn.jsdelivr.net/gh/Wosmos/wosmos@master/public/logo/wordmark.svg
https://cdn.jsdelivr.net/gh/Wosmos/wosmos@master/public/logo/mark-256.png
https://cdn.jsdelivr.net/gh/Wosmos/wosmos@master/public/logo/favicon.ico
```

`@master` responses cache for up to ~12h. For an instant, immutable URL, pin
to a commit SHA or a tag instead (e.g. `@v1`) and purge on update via
https://www.jsdelivr.com/tools/purge.
