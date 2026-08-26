# Portfolio site

Static, single-file portfolio (`index.html`). No build step, no dependencies.

## Deploy to Vercel — without GitHub

**Option A — drag & drop (easiest)**
1. Go to https://vercel.com/new
2. Look for "Deploy without Git" / drag-and-drop area on that page
3. Drag the whole `portfolio` folder in
4. Vercel deploys it instantly and gives you a live URL

**Option B — Vercel CLI**
```bash
npm install -g vercel
cd portfolio
vercel
```
Follow the prompts (login, confirm project settings — defaults are fine since this is a static site). Run `vercel --prod` to push it live.

## Editing content

Everything is in `index.html`:
- Hero text near the top (`<h1>...</h1>`)
- "3D work" cards — search for `id="work-3d"`, duplicate/edit the `.card` blocks
- "Mechanical work" cards — search for `id="work-mech"`
- About section specs — search for `id="about"`
- Contact links — search for `id="contact"`, update the `mailto:` and social links

To add real project images, drop image files in an `/images` folder next to `index.html` and reference them with `<img src="images/yourfile.jpg">` inside a card.
