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
  Monday evening: Trump dares Iran to test the Hormuz blockade and
  says he may resume strikes after the New Year; Tehran claims two
  tankers hit mines near Hormuz; Houthi drones target Riyadh; Iran
  starts rolling power cuts.
- **Dymer toll rises to 11.** An 11th body is pulled out; 11
  still missing, two of them children.
- **Kremlin cries 'terror' over Sparta II.** Moscow calls the
  drone strike terrorism; the ship is towed on to Russia, Kyiv
  silent.
- **COP31: blame game erupts.** Calls to sack Australia's Bowen;
  Pacific islands despair — 90 nations sign a power pledge.
- **Isidro heir named as violence feared.** Successor Óscar
  Gastélum tipped as Sinaloa braces for a turf war; no
  extradition date.
- **Ticker:** Dymer toll 11; Trump dares Iran on Hormuz; Kremlin
  cries terror; COP31 blame game; Isidro heir named.

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
