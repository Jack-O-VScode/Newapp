# Social assets

1080x1350 (Instagram portrait — takes the most feed space).

| File | Use |
|---|---|
| `post-steam.png` | Steam wallet codes |
| `post-website.png` | Website launch |

Captions live in the conversation; regenerate these by asking Claude — the
brand colours, fonts and logo all come from `assets/logo.png` and the site's
palette, so they stay consistent with the page.

## Reels

| File | Use |
|---|---|
| `reel-steam.mp4` | Steam codes, 1080x1920, 6.5s |
| `reel-website.mp4` | Website launch, 1080x1920, 6.5s |

9:16 with content kept clear of Instagram's UI overlay (top ~170px,
bottom ~400px). Silent by design — add trending audio in the Instagram
editor at upload, since that's where the algorithmic signal comes from.

## Tutorial

`reel-website-sale.mp4` — 1080x1920, ~31s, launch-sale framing.
`reel-how-to-order.mp4` — 1080x1920, ~14s, faster cut of the same flow. A real Playwright recording of
the live page on a phone viewport with a drawn cursor, not a mockup. The
Web3Forms endpoint is stubbed during recording so filming never sends a
real order. Regenerate after any change to the order form, or the tutorial
will show a form that no longer exists.
