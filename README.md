# Rollage

Turn any picture into a ribbed, mirrored "rolled collage" — right in your browser.

**One file. No installs, no servers, no uploads.** Everything happens on your own
computer: download `index.html`, double-click it, and it opens in your browser.
Your photos never leave your machine.

## What does it do?

A rollage, step by step:

1. **Mirror** your picture into four panels (like mirror-folding paper before
   cutting a snowflake), so every edge matches its neighbour. This is the new
   base image.
2. **Slice** the base into *Cuts* vertical strips.
3. **Shuffle** the strips from the ends inward: `1, 8, 2, 7, 3, 6, 4, 5`.
4. **Repeat** the slice-and-shuffle on the rows (the same trick, turned 90°).
5. Repeat steps 2–4 up to *Steps* times to deepen the effect.

## How to use it

- **Image** — pick a photo from your computer (or drag one onto the dashed zone).
- **Panels** — after uploading, you see the four mirrored quadrants. Click any
  panel to swap in a *different* image, and roll four pictures into one.
- **Cuts** (2–256) — how many strips each shuffle uses.
- **Steps** (− / + buttons, 1–32) — how many times the shuffle repeats.
- **Download PNG** — save your creation.

Works in any modern browser. iPhone photos in HEIC format aren't supported by
Chrome/Firefox — export them as JPEG or PNG first (the app will tell you if you
try).

## For the curious

The whole app is a single `index.html`, hand-written in plain HTML, CSS and
JavaScript with **no libraries**. The code is heavily commented in
plain language, explaining not just *what* it does but *why* each choice was
made. Open it in a text editor and have a look — it's meant to be read.

## The look

Rollage wears the **TFE** ("There For Everything") house style, taken from the
design tokens in [tfeSvelteTemplates](https://github.com/Jktfe/tfeSvelteTemplates):
brand blue `#004695`, Anton headlines, IBM Plex Sans and Mono, thin rules, and
the ink footer. It follows your system's light/dark setting.

The fonts are the only thing the page fetches from the internet. Offline, it
falls back to fonts already on your computer, so it still works the same.

## Try it with

- A photo with strong colours meeting at an edge (they smear into ribbons)
- Four completely different photos in the four panels
- Lots of cuts (64+) at 1 step vs few cuts at many steps — very different looks
