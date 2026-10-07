# មុន្នីរ័ត្ន & វឌ្ឍនៈ — Khmer Wedding E‑Invitation

Vite static-site starter for a cinematic Khmer wedding invitation.

## Assets
Place the supplied files here:
- `public/images/hero.jpg`
- `public/images/photo-01.jpg` … `photo-06.jpg`
- `public/images/khqr.png`, `public/images/aba-qr.png`
- `public/audio/wedding.mp3`
- Optional starter kit SVGs/textures under `public/assets/`

The current build intentionally uses material-style placeholders because no wedding photos/card/QR/music were attached to this conversation.

## Data
All wedding details: `src/data/wedding.js`.
All interface copy: `src/data/i18n.js`.

## Run
```bash
npm install
npm run dev
npm run build
```

## Deployment
Set `VITE_SITE_URL` in your hosting environment and update the absolute `og:image` URL in `index.html` for the final public domain.

## Image processing
The `photos:webp` script documents the intended Sharp pipeline. In a normal build environment, generate 640/1280/2000px WebP derivatives and strip GPS/EXIF before deployment.

## Motion
This offline build uses native CSS/JS motion so it can be previewed without fetching third-party packages. For the final production deployment, GSAP + ScrollTrigger + Lenis can be installed and wired into the existing section hooks without changing the content/data architecture.
