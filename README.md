# Mikan Beat 🎵🐱

A tiny 4-lane rhythm game (D / F / J / K) with a fully **procedural chiptune
soundtrack** — kick, snare, hi-hat, bass and a lead melody are all synthesized
live with WebAudio. No audio files, no images: everything is code.

Made for [Crescent](https://crescent.hackclub.com/) (the Rhythm card).

## Play

Open `index.html`. Press SPACE, then hit the notes as they reach the line.

- **D F J K** — the four lanes
- PERFECT (<90ms) / GREAT (<160ms) / OK (<240ms), combo multiplies score
- Mikan dances when you hit, sulks when you miss
- The song is ~36 seconds; the results screen shows score, max combo and accuracy

## How it works

- **Chart**: hand-authored 8th-note patterns cycled across 14 bars
- **Music**: an AudioContext scheduler with lookahead — each bar schedules a
  kick, hats, a snare on 2 & 4, a bass line, and a sprinkled lead melody from
  a C-major-ish scale
- **Art**: canvas rectangles (the same pixel-cat lineage as the rest of the
  Mikan series)

## Run locally

Just open `index.html`, or:

```bash
python3 -m http.server 3844
```
