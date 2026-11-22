[![make.fun](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/rinoo9/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122)

# 22 November 2026 — One Day in Pictures

A make.fun entry for the [news-image-20261122](https://make.fun/bounty/news-image-20261122) bounty: one image that sums up the world's news of Sunday 22 November 2026.

## The image

A newspaper front page, drawn by `compose.py` (Pillow) from a generated
hero photograph of a Gulf port at night. Every story was first reported
on Sunday 22 November 2026 (checked against the Sunday-evening /
overnight reporting, early Monday 23 Nov WIB):

- **New hero photo** — searchlights and smoke over a Gulf port at
  night, with a caption strip tying it to the Saturday-night strikes
  on US bases in Bahrain.
- **Lead — Iran hits US bases in Bahrain again.** Iran says its
  missiles hit two US Patriot radars on Saturday night; Bahrain says
  its defences held. Sunday follow-up: two hurt in the Sitra plant
  fire, Bahrain takes Iran to the UN Security Council, 25 tankers hit
  in a week as the blockade hits day 130.
- **14 missing after a drone hits a Kyiv block.** A five-storey block
  in Dymer partly collapses; 186 drones launched overnight, 161
  downed.
- **Sparta II towed out of Finnish waters.** Flames out after two
  days of firefighting; a Russian tug takes the drone-hit ship as
  crews cool its warm containers.
- **COP31: longest summit ends in failure.** Guterres 'deeply
  disappointed' as the Antalya Pact dies — the first major COP
  breakdown since 2009.
- **'El Chapo Isidro' perp-walked after the Guasave raid.** Mexico
  parades the FBI's most-wanted boss; the US unveils narcoterrorism
  charges.
- **Ticker:** Kryvyi Rih toll rises to 73 hurt, 9 children; Zelensky
  renews his call for Patriot interceptors; Bahrain appeals to the UN
  Security Council; 25 tankers hit in a week at Hormuz; Estonia border
  rush before the 1 December closure; FBI probing a hack of its
  criminal database.

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
