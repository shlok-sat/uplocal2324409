# Uplocal Landing Page

This repository contains a static landing page for Uplocal’s automated ROI
platform tailored to multi location and franchise brands. The page showcases
messaging, feature summaries, social proof, and FAQ content with scroll based
animations implemented via IntersectionObserver.

## Preview

Open the page directly in your browser:

```bash
open /Users/shloksat/Desktop/uplocal/index.html
```

Or serve it via a lightweight HTTP server (recommended for testing
IntersectionObserver behavior):

```bash
cd /Users/shloksat/Desktop/uplocal
python3 -m http.server 8000
```

Navigate to `http://localhost:8000/index.html`.

## Structure

- `index.html` – All markup, styling, and animation logic live in this single file.
- Custom CSS defines the professional gradient theme, typography, and component
  system (cards, tables, timeline, FAQs).
- `.reveal` utility class plus IntersectionObserver add smooth fade + slide
  animations when sections enter the viewport.

## Customizing

1. Update copy or imagery inside the relevant sections in `index.html`.
2. Adjust colors, spacing, or timing in the `<style>` block at the top of the
   file.
3. Modify animation thresholds or delays in the script at the bottom if you need
   quicker or slower reveals.

## Deployment

Because everything is static HTML/CSS/JS, you can host the page on any static
hosting provider (Netlify, Vercel, GitHub Pages, S3, etc.) by uploading
`index.html` (and any supporting assets you might add later).

