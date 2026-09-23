# Blankroom

A fully working photo editor. Every slider, curve, and panel works exactly as it should. There is just no way to open a photo.

[Live demo →]

## What it is

Blankroom looks and behaves like a professional editing app with exposure, curves, HSL, sharpening, vignette, grain, crop, and a real histogram, all fully interactive. The catch is the subject: every control edits a single grey rectangle instead of a photo, and the Import button is built to fail in a new way every time you press it.

Nothing here is a bug. It's the whole purpose of this program.

## Features

- **A real editing pipeline.** Exposure, brightness, contrast, highlights/shadows, whites/blacks, a draggable tone curve, HSL by hue/saturation/luminance, sharpening, noise reduction, vignette, grain, crop, and straighten — all computed live against one flat color.
- **A live histogram** that responds to every adjustment, including clipping indicators and vignette falloff.
- **Import that always fails**, with a rotating pool of in-character error messages, an escalating tone after 10 and 25 attempts, and a drag-and-drop overlay that reads "Drop not allowed."
- **A history panel**, styled as a timeline, that logs every change in its own deadpan voice, getting wearier the longer you play ("on nothing," then "on nothing again," then "on nothing, still").
- **Presets** (Vintage, Moody, Punchy, Film Fade, and more) that preview correctly as color swatches.
- **Before/After compare** with a draggable divider, and a fake Enhance flow that ends in "Nothing to enhance. Try again with less nothing."
- **Chaotic controls.** Several buttons quietly do something other than what they say — Rotate Left rotates right, presets apply their neighbor, crop buttons apply the next aspect ratio, and Reset All applies a random preset instead of resetting. The history log always tells the truth about what actually happened, in its own witty voice, with several phrasings that rotate at random. (Double-click Reset All for the real thing.)
- **An animated wordmark.** The "Blankroom" logo carries its own small color-blob background and a slow gradient shift, so the personality lives in the header instead of a banner that eats into the canvas.

## Design

The interface runs on a warm five-color palette — deep maroon, dark red, burnt orange, gold, and blue — used consistently across section accents, sliders, the tone curve, the history timeline, and the photo's glowing border. Light and dark mode each get their own tuned variant of the palette, and the page follows the system color scheme automatically.

## Running it

It's a single self-contained HTML file. No build step, no dependencies to install.

```
open blankroom.html
```

or just double-click it, or drop it onto any static file host / GitHub Pages / Netlify.

The only external request is a Google Fonts stylesheet (Instrument Sans and Instrument Serif); the page falls back to system fonts if that request is blocked or offline.

## Why

Because the internet has enough photo editors that actually edit photos.
