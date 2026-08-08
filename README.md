# ricespin

A single grain of rice, spinning forever.

That's the whole website. It is a loving, entirely safe-for-work tribute to a
certain infamous single-serving site of the early internet — same energy,
different subject matter.

## What's in it

- `index.html` — the entire site. No build step, no dependencies, no tracking.

## Features

- A hand-drawn SVG grain of rice rotating on the Y axis, forever
- A live rotation counter and RPM readout
- **Faster** / **Slower** / **Reverse** controls
- **Turbo:** the speed limit starts at 900 RPM and lifts to 6767 RPM once your
  all-time counter passes 1000 rotations, announced with a klaxon nobody asked for
- Progress saved to `localStorage` — all-time rotations, speed, direction,
  visit count, top RPM, and whether turbo has been earned. **Reset** clears it
- An optional WebAudio chiptune loop (off by default — nothing autoplays)
- Throbbing conic-gradient backdrop, scanlines, and a marquee, because it
  would be dishonest to do this tastefully
- `prefers-reduced-motion` support: the flashing and wobbling stop, and the
  grain slows to a gentle 6-second rotation

## Running it

Open `index.html` in a browser. That's it.

Or serve it locally if you prefer:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

It's one static file, so any static host works. For GitHub Pages: enable Pages
for the repository and point it at the branch root.
