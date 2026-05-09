# June Jam — Performance Proposal Site

A multi-page proposal site for Caroline Godwin's June Jam performance pitch.

## What's Inside

- `index.html` — Landing page, concept, and 3-day overview
- `friday.html` — Day 1: Neon Day characters
- `saturday.html` — Day 2: Red Day characters
- `sunday.html` — Day 3: Dark Day characters
- `info.html` — Production details, rig info, simulated fire, Desert Dwellers stage request, contact
- `css/style.css` — Mystical forest theme stylesheet
- `js/main.js` — Nav toggle and scroll reveal
- `images/` — Character reference photos

## Hosting Options

This is a fully static site — no build step, no dependencies. Host it anywhere:

### Option 1: GitHub Pages (recommended, free)
1. Create a new repository on GitHub (e.g., `june-jam`)
2. Drop all the files from this folder into the repo
3. Go to **Settings → Pages**
4. Under "Build and deployment", set source to **Deploy from a branch**, branch **main**, folder **/ (root)**
5. Save. Site goes live at `https://yourusername.github.io/june-jam/` within a minute.

### Option 2: Netlify Drop (fastest)
1. Go to https://app.netlify.com/drop
2. Drag the entire folder onto the page
3. Get a live URL instantly. Can rename / map a custom domain later.

### Option 3: Local preview
Just double-click `index.html`. Or run a local server:
```
python3 -m http.server 8000
```
Then open http://localhost:8000

## Editing

Each character is its own `<article class="character">` block in the day file. To add or change:
- **Photo**: replace the corresponding image in `images/` or update the `<img src>` path
- **Costume / makeup / mood / palette**: edit the `<dl class="character-meta">` block
- **Quote / tone**: edit the `<p class="character-quote">` and `<p class="character-tone">`

To add new characters with placeholder photos, copy the `character-image-placeholder` div pattern.

## Updating the proposal

The companion Word doc `June_Jam_Performance_Proposal.docx` (provided separately) covers the same lineup in printable / shareable format. Both should stay in sync if you update one.

— Built for Caroline Godwin · @carolinegodwin
