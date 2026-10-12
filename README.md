# This Saturday website

The landing page for **This Saturday**, a screen-free weekly comic magazine for kids, delivered every Saturday morning.

It is a single static page: `index.html` plus the images in `art/`. No build step, no dependencies.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

Any static host works (GitHub Pages, Netlify, Vercel, Cloudflare Pages). Point it at the repo root; `index.html` is the entry page.

For GitHub Pages: Settings → Pages → Deploy from a branch → `main` / root.

## What's in the page

- Hero: the cover rolls off to the left, then Subbu, Arjun and Gappu fly in around the logo.
- How it works, what's inside, the three-panel sample comic, editions by age, the characters, the parent guide, pricing, delivery area, FAQ.
- "Your community" opens a pop-up form to request delivery outside Sarjapur Road.

## Before going live

- The two forms (founding family and community request) only show a confirmation on screen. Connect them to a real destination (Google Sheet, form service or your backend) in the `<script>` at the bottom of `index.html`.
- Add your contact details, Instagram and WhatsApp to the footer.
- Confirm the offer copy ("First 4 Saturdays free", ₹299 for 4 Saturdays) is final.

## Images

| File | Used for |
| --- | --- |
| `art/subbu-crossed.webp`, `art/arjun.webp`, `art/gappu-sleep.webp` | Hero animation (transparent cut-outs) |
| `art/crew.jpg` | Characters section and social share image |
| `art/fest-cashbox.jpg`, `art/fest-empty.jpg`, `art/fest-reader.jpg` | Sample comic spread |
