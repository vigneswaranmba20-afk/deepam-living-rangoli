# DEEPAM — The Living Rangoli 🪔

An original, lightweight, responsive Diwali greeting-card studio inspired by traditional rangoli and diya arrangements.

## Features

- Ten original mathematical SVG rangoli illustrations (precise radial symmetry and bezier curves)
- Six curated palettes, plus individual color pickers for background, petals, accents and leaves
- Gently animated diyas, particle bursts with gravity and drag, reduced-motion support
- Default **Happy Diwali** greeting with optional recipient and sender
- High-resolution PNG export (1520×1760), editable SVG export, Android Web Share API and personal-design links
- No sign-in, tracking, server, OpenAI API calls, photo uploads or watermarks
- PWA caching for basic offline use; SVG art and export require no external assets
- Progressive animation enhancement via Motion (CDN) when available; works without the library

## Run locally

Open `index.html` in a modern browser, or host these files on any static server (GitHub Pages recommended). HTTPS is required for reliable native sharing, clipboard and service worker support.

## Publish on GitHub Pages

1. Create a public GitHub repository named `deepam-living-rangoli` (or another name).
2. Upload the four files `index.html`, `icon.svg`, `manifest.webmanifest`, `sw.js` to the repository root.
3. Open **Settings → Pages → Build and deployment → Deploy from a branch**, choose `main` and `/(root)`, and save.
4. Your URL will be `https://<username>.github.io/<repo>/` after deployment.

The website contains only original vector drawing code. User-supplied reference photography is **not embedded** or redistributed.

## Design notes

These are *vector reinterpretations* of supplied rangoli photographs, **not automatic pixel-perfect tracing**. Symmetry is enforced by rotations of `360/n` degrees; petal boundaries are cubic Bézier paths with independent palette fills. Candle flames animate with CSS transform; spark particles follow a time-stepped model with gravity and damping. Users can download the generated paths as editable SVG.

Copyright © 2026. All rights reserved by the project creator unless separately licensed.