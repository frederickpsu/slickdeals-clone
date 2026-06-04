# Slickdeals Clone

A pixel-perfect, fully functional static clone of [Slickdeals.com](https://slickdeals.com) built as a single-file website.

## Features
- **Authentic Slickdeals UI**: Orange accent colors (#ff6600), clean card-based layout, navigation, and typography
- **Interactive Deal Cards**: 
  - Search across titles, stores, and categories
  - Filter by Hot Deals, Trending, and Categories
  - Click any card to open a detailed modal
  - Upvote deals (votes update live)
- **Post a Deal**: Add your own deals via the "Post a Deal" form (adds to the live list)
- **Community Section**: Clickable forum highlights that open simulated threads
- **Fully Responsive**: Works great on desktop, tablet, and mobile
- **No Build Step**: Single `index.html` with Tailwind via CDN + Font Awesome

## Quick Start (Local)
1. Clone or download this folder
2. Open `index.html` directly in any browser

```bash
# If you have the files locally:
open slickdeals-clone/index.html
```

## Publish to GitHub Pages (Recommended)
### Option 1: Using GitHub CLI (fastest)
```bash
cd slickdeals-clone
gh repo create slickdeals-clone --public --source=. --remote=origin --push
```

Then go to your repo → Settings → Pages → Source: "Deploy from a branch" → Branch: `main` → Save.

Your site will be live at: `https://YOUR_USERNAME.github.io/slickdeals-clone`

### Option 2: Manual (if no gh CLI)
```bash
cd slickdeals-clone

# Initialize if not already done
git init -b main
git add .
git commit -m "Initial Slickdeals clone"

# Create repo on GitHub.com first (use web UI), then:
git remote add origin https://github.com/YOUR_USERNAME/slickdeals-clone.git
git branch -M main
git push -u origin main
```

### Enable GitHub Pages
1. Go to repo on GitHub
2. Settings → Pages
3. Under "Build and deployment", set Source to "Deploy from a branch"
4. Select branch `main` and folder `/ (root)`
5. Save — your site will be published in ~1 minute

## Project Structure
```
slickdeals-clone/
├── index.html    # The entire website (HTML + Tailwind + JS)
└── README.md
```

## Demo Notes
- All data is client-side JavaScript (no backend or database)
- Added deals and votes are temporary (page refresh resets)
- This is a fan-made educational clone and not affiliated with Slickdeals
- Perfect for portfolios, demos, or learning front-end development

## Future Improvements (Ideas)
- Add localStorage to persist user-added deals and votes
- Infinite scroll / pagination
- Dark mode toggle
- Real API integration for live deals (if available)
- User accounts simulation

Built with ❤️ using HTML, Tailwind CSS, and vanilla JavaScript.

Enjoy hunting for deals!