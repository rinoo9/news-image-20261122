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
  UN action. Monday follow-up: Tehran blames a crashed US interceptor
  for the Sitra fire as Qatar mediates.
- **Boy, 7, pulled alive from the Dymer rubble.** Three bodies found,
  ~10 still feared trapped; rescuers pull a boy, 7, alive after
  14 hours.
- **Sparta II leaves Finnish waters.** President Stubb confirms the
  ship is out; restrictions lifted, no leaks, Murman tows it on.
- **Saudi blamed as COP31 talks fail.** O'Brien: the summit was
  'hijacked by some oil states'; 130 nations backed fossil-fuel
  wording.
- **'El Chapo Isidro' faces a US extradition wait.** Mexico's case
  comes first and no extradition date is set; US intelligence aided
  the raid.
- **Ticker:** Kryvyi Rih: 73 hurt, 9 children; boy, 7, pulled alive
  from Dymer rubble; Saudi blamed for COP31; Sparta II out of Finnish
  waters; Isidro extradition waits.

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
