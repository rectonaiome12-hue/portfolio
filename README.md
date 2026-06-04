# Portfolio — Naiome Recto

A clean, editorial-style software developer portfolio. Built with vanilla HTML, CSS, and JavaScript — no build step required.

## Customizing

Open `index.html` and update:
- **Your name** — search for "Alex Rivera"
- **Hero section** — tagline, subheading, location, availability
- **Projects** — title, description, tags, links, and stats
- **About** — bio paragraphs, work experience entries
- **Writing** — article titles, excerpts, and links
- **Contact** — email address and social links

Open `style.css` and update:
- `--accent` (currently `#b84b2e`) — change to your preferred accent color
- Font choices at the top of the `:root` block

## Deploying to Vercel

### Option 1 — Vercel CLI (recommended)
```bash
npm install -g vercel
vercel
```
Follow the prompts. Done.

### Option 2 — Vercel Dashboard (no CLI needed)
1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Click **Deploy** — Vercel auto-detects the static site

### Option 3 — Drag & drop
1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag the entire `portfolio/` folder into the browser
3. Done — you'll get a live URL instantly

## File structure
```
portfolio/
├── index.html    ← Main page (edit your content here)
├── style.css     ← All styles + responsive
├── main.js       ← Scroll animations + mobile nav
├── vercel.json   ← Vercel routing config
└── README.md
```

## Adding a résumé
Place your PDF at `resume.pdf` in this folder. The "Download résumé" button already links to it.

## Adding a real photo
Replace the `.portrait-placeholder` div in `index.html` with:
```html
<img src="your-photo.jpg" alt="Your Name" class="portrait-photo" />
```
And add to `style.css`:
```css
.portrait-photo { width: 180px; height: 220px; object-fit: cover; }
```
