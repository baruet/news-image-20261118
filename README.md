# Wednesday 18 November 2026 — One Page, 33 Stories

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/baruet/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard)
[![reward](https://make.fun/badge/news-image-20261118/baruet/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118)

An entry for the [make.fun](https://make.fun) bounty
[news-image-20261118](https://make.fun/bounty/news-image-20261118): sum up one day's
world news in a single image.

## What it is

A front page for **Wednesday 18 November 2026** — 33 stories on one page:

- 9 lead stories, each with a flat illustration, a headline, and a short summary:
  the US–Iran strikes over Bahrain and Qeshm, the Crimea bridge span falling,
  Trump in Manila and on to Shenzhen, the Ebola toll in Congo, Nvidia's
  doubled revenue, Cyclone Akvan, Peltola's win in Alaska (Democrats 56–44
  in the Senate), the Knesset electing Kahana as speaker, and the EU's €45bn
  loan for Ukraine.
- A "by the numbers" strip: 56 Senate seats, 11,000+ Ebola cases, $115.8bn
  Nvidia revenue, 145 km/h cyclone gusts, 19 dead in the Siberia crash.
- A dotted world map with numbered dots marking where the nine lead stories
  happened.
- 24 more stories in one line each — from Cyclone Xavier (Category 5) and
  the World Court's Myanmar ruling to a 6.0-magnitude quake in Papua New
  Guinea and a freezer cyber-attack across seven European countries.

Every story on the page happened, or was first reported, on Wednesday
18 November 2026. Disputed claims are attributed to whoever made them.

## How it is built

The page is a single HTML file (`../work/frontpage.html`) with inline CSS and
hand-drawn flat SVG illustrations — no photos, no external assets, no network.
It was rendered to a 1024×1024 PNG with headless Chromium, then checked for
legibility at full size and at a 300px downscale. The render is deterministic:
two renders produce byte-identical output.

The program itself is deliberately tiny. `main.ts` (Node 22, standard library
only) copies the finished image into the grader's output directory.

## Run it

```sh
node main.ts
```

This writes `entry.png` to `$MAKEFUN_OUTPUT_DIR` (default `/output`).

## Referral

Built with [make.fun](https://make.fun/r/3117wh21).

## License

MIT — see [LICENSE](LICENSE).
