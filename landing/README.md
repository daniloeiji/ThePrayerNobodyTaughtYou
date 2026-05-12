# The Divine Calling — Landing Page

## Structure
```
landing/
├── index.html        ← main page
└── assets/
    ├── sky-bg.png    ← sky background
    └── book-only.png ← book mockup
```

## How to open in VS Code
1. Unzip the file.
2. In VS Code: **File → Open Folder…** and choose the `landing/` folder.
3. Recommended: install the **Live Server** extension (Ritwick Dey), then right-click `index.html` → "Open with Live Server". This opens the page with automatic reload on save.

## Insert the VTURB video
Open `index.html` and look for the marked block:
```html
<!-- ============================================================
     VIDEO · Paste your embed here (VTURB, unlisted YouTube, Vimeo, etc.)
============================================================ -->
```
Replace `<div class="video-placeholder">…</div>` with your VTURB snippet:
```html
<vturb-smartplayer id="vid-XXXXXXXXX"></vturb-smartplayer>
<script src="https://scripts.converteai.net/.../player.js" async></script>
```
The frame is already sized at 16:9 — the player expands to 100%.

## Publish
Upload **the entire `landing/` folder** (not only the HTML) to your hosting:
- **Hostinger / cPanel:** upload it to the `public_html` directory and unzip it.
- **Netlify / Vercel / Cloudflare Pages:** drag the folder and get a free HTTPS URL.
- **GitHub Pages:** push the folder contents to a repo and enable Pages.

If your platform only accepts one HTML file, ask for the self-contained "single-file" version.
