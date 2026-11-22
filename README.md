[![make.fun](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122)

# 22 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261122](https://make.fun/bounty/news-image-20261122) bounty: one image that sums up the world's news of Sunday 22 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of a Gulf port at night. Every story was first reported
on Sunday 22 November 2026 (checked against the evening's reporting):

- **New hero photo** — searchlights and smoke over a Gulf port at
  night, with a caption strip tying it to the Saturday-night strikes
  on US bases in Bahrain.
- **Lead — Iran hits US bases in Bahrain again.** Iran says its
  missiles hit two US Patriot radars on Saturday night; Bahrain says
  its defences held, with no casualties and a factory fire. Three
  tankers are hit near Hormuz, and 14 Iranian tankers mass off Kharg
  Island to break the US blockade.
- **Zelensky: Crimea Bridge strikes 'fair response'.** Ukraine's
  president defends the bridge strikes as he meets Britain's Wes
  Streeting.
- **Sparta II still burning off Finland.** The drone-hit Russian
  cargo ship drifts at anchor in Finnish waters; its 16 crew are
  evacuated as the fire rages on.
- **COP31 collapses with no deal.** The final text — silent on fossil
  fuels — is rejected on Sunday; the first climate summit to end
  with no deal since 2000.
- **'El Chapo Isidro' faces US extradition.** Eleven die in the
  Guasave raid; the cartel boss is flown to Mexico City.
- **Ticker:** 14 missing as a Russian drone hits a Kyiv-region block,
  Iran tankers mass at Kharg, Kryvyi Rih double-tap kills a boy of 7
  and a medic, Estonia border rush before the 1 December closure, FBI
  probing a hack of its criminal database, Palisades fire arson
  conviction.

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
