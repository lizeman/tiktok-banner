# tiktok-banner

A scrolling call-to-action banner for TikTok LIVE Studio.

- Banner URL: https://lizeman.github.io/tiktok-banner/
- Preview on a checkerboard: https://lizeman.github.io/tiktok-banner/?preview

## Add it in TikTok LIVE Studio

1. Add source → Link.
2. Paste the banner URL.
3. Turn on Custom resolution and set it to 1080 × 160.
4. Turn sound off and keep "Always keep active" on.
5. Drag the source to where it should sit on the portrait canvas.

## Change the text

Edit `banner.json` and push. The page checks for changes every 5 seconds, and
GitHub Pages usually publishes a push within a minute.

| Key | What it does |
| --- | --- |
| `visible` | `false` fades the banner out |
| `mode` | `"scroll"` scrolls all messages; `"rotate"` shows one at a time |
| `messages` | The lines to show |
| `label` | Optional pill on the left, e.g. `"NEW"`; `""` hides it |
| `speed` | Scroll speed in pixels per second |
| `hold` | Seconds per message in rotate mode |
| `fontSize`, `height` | Text size and bar height in pixels |
| `textColor`, `barColor`, `accentColor`, `separatorColor` | Colors |

If `banner.json` can't be loaded, the page keeps showing the last text it had.
