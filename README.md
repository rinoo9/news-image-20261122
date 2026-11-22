[![make.fun](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122)

# 22 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261122](https://make.fun/bounty/news-image-20261122) bounty: one image that sums up the world's news of Sunday 22 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of a Gulf port at night. Every story was first reported
on Sunday 22 November 2026 (checked against the morning's reporting):

- **New hero photo** — searchlights and smoke over a Gulf port at
  night, with a caption strip tying it to the Saturday-night strikes
  on US bases in Bahrain.
- **Lead — Iran hits US bases in Bahrain again.** Iran fires drones
  and missiles at two US bases on Saturday night — the fourth attack
  on Bahrain in nine days. Air-raid sirens sound in Manama; an
  industrial plant burns; tankers are hit off Oman.
- **Zelensky: Crimea Bridge strikes 'fair response'.** Ukraine's
  president defends the bridge strikes as he meets Britain's Wes
  Streeting.
- **Drones hit Russian cargo ship.** A Russia-bound freighter is
  attacked in the Gulf of Finland; Finland tightens security.
- **COP31 deadlocked on fossil fuels.** Climate talks in Antalya
  stall as the fight over fossil fuels leaves the summit in deadlock.
- **'El Chapo Isidro' arrested.** Mexico captures a cartel boss on
  the FBI's most-wanted list; the arrest sparks deadly violence in
  Sinaloa.
- **Ticker:** France takes the Myanmar ICJ ruling to the UN Security
  Council, Trump reaches Shenzhen for the Xi–Putin summit, Estonia
  border rush before the 1 December closure, Denmark accuses Russia
  of a plot to kill a US-Ukrainian rapper, FBI probing a hack of its
  criminal database, Palisades fire arson conviction.

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
