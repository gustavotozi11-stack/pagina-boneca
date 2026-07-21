# Kit Casinhas de Boneca — Sales Page

A pre-built static sales page (Portuguese) for a printable paper dollhouse kit ("Kit Casinhas de Boneca Realistas em Papel"). Originally built with Lovable/Vite and exported as a static bundle.

## Stack

- Pure static HTML/CSS/JS — no build step required
- Served via Python's built-in HTTP server

## How to run

The workflow **Start application** serves the site on port 5000:

```
python3 -m http.server 5000
```

## File structure

```
index.html          — Main sales page (single-file, fully inlined)
css/
  styles-BAsjNBlu.css   — Compiled Tailwind/app styles
images/
  hero-kit.jpg          — Hero product image (placeholder — replace with real image)
  bonus-*.webp          — Bonus product images
  review-*.webp         — Customer review photos
js/
  E-v1.js               — Wistia video player
  latest.js             — UTMify tracking
  lbzxg14f3c.jsonp      — Wistia embed config
  pixel.js              — UTMify pixel
```

## Notes

- `images/hero-kit.jpg` is a placeholder (79-byte text file). Replace it with the real hero product image to fix the broken image in the hero section.
- Two JS bundle files (`assets/index-CC1XeYrQ.js`, `assets/index-B8QECkvs.js`) referenced as `<link rel="modulepreload">` are missing from the export but are not critical — the page renders fully without them.
- Tracking/pixel scripts (UTMify, Wistia) may show console errors in the Replit preview due to network restrictions; they work normally on a public deployment.
