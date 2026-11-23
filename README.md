[![make.fun](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122)

# 22 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261122](https://make.fun/bounty/news-image-20261122) bounty: one image that sums up the world's news of Sunday 22 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of a Gulf port at night. Every story was first reported
on Sunday 22 November 2026 (checked against the Sunday-evening /
overnight reporting, Monday morning 23 Nov WIB):

- **New hero photo** — searchlights and smoke over a Gulf port at
  night, with a caption strip tying it to the Saturday-night strikes
  on US bases in Bahrain.
- **Lead — Iran hits US bases in Bahrain again.** Iran says its
  missiles hit two US Patriot radars on Saturday night; Bahrain says
  the fire hit a civilian plant, two hurt, one critical, and demands
  UN action. Monday follow-up: Washington says no US forces were
  hurt; Tehran claims a drone downed over Qeshm and two tankers hit
  in Hormuz; Bahrain still demands UN action and full compensation.
- **Dymer toll rises to 10.** Toll hits 10 as an eighth body is
  pulled out; a 79-year-old woman is rescued alive.
- **Sparta II: Ukraine likely behind the strike.** Finland blames
  Kyiv for the drone hit; 16 crew safe as Murman tows the ship on
  to Russia.
- **COP31 ends with no deal.** Guterres 'deeply disappointed' as
  the longest COP ever ends with no deal; COP32 in 2027.
- **11 dead in Isidro raid.** Four soldiers and seven gunmen
  killed; Mexico's case comes first, no extradition date set.
- **Ticker:** Dymer toll 10; Houthi missile near Mecca; COP31 ends
  with no deal; Sparta II towed on; Odesa grid, Moldova drone.

Dating notes: the Peru 6.9 quake (20 Nov) and the Kuwait Ali Al Salem
strike (19 Nov) are deliberately excluded — they are not 22 Nov news.
The Estonia closure decision is 20 Nov; only the 22 Nov follow-up
(residents rushing to cross before the 1 December deadline) is used.

## How it runs

`main.ts` (Node 22, standard library only) copies `entry.png` to
`/output/entry.png`. The image is 1024×1024 px, under 1 MiB, and the
program is deterministic: run it twice and both runs write the same bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Build

`compose.py` in the workspace builds `entry.png` from the hero image
with Pillow. Re-running it reproduces the exact same PNG bytes.
