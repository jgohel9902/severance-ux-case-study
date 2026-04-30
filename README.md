# Severance — Case Study Website

A complete multi-page case study site for the Severance UX project.

## Structure

```
Severance-Case-Study-Site/
├── index.html ........... Overview · TL;DR · headline outcomes
├── process.html ......... Full double-diamond walkthrough
├── research.html ........ Interviews · themes · personas · journey · IA · flows
├── wireframes.html ...... Paper wireframes + digital wireframes + iterations
├── designs.html ......... Final hi-fi designs (iPhone 14 Pro Dark, 9 screens)
├── testing.html ......... Usability test plan, results, v3 → v4 fixes
├── about.html ........... About Jenil + contact
├── style.css ............ Shared styles for all pages
├── README.md ............ You are here
└── assets/
    ├── paper-wireframes.svg
    ├── digital-wireframes.svg
    ├── user-journey-map.svg
    ├── information-architecture.svg
    └── user-flows.svg
```

## How to view locally

Just double-click `index.html`. It opens in your default browser. Navigate via the sticky top nav.

## How to host for free

### Option 1: GitHub Pages (recommended)

1. In PowerShell, navigate to this folder:
   ```powershell
   cd "$env:USERPROFILE\Desktop\Severance-Case-Study-Site"
   ```
2. Initialize git and push:
   ```powershell
   git init
   git branch -M main
   git add .
   git commit -m "Initial commit — Severance case study site"
   gh repo create severance-case-study-site --public --source=. --remote=origin --push
   ```
3. On GitHub: Settings → Pages → Source: `main` branch, root folder → Save
4. Wait ~60 seconds. Your site is live at:
   `https://YOUR-USERNAME.github.io/severance-case-study-site/`

### Option 2: Netlify Drop (no git needed)

1. Go to https://app.netlify.com/drop
2. Drag this entire folder onto the drop zone
3. Live in 10 seconds at a `random-name.netlify.app` URL
4. (Optional) Sign up free → claim the site → rename it to `jenil-severance.netlify.app`

### Option 3: Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. In this folder: `vercel`
3. Follow prompts. Live in 30 seconds.

### Option 4: Cloudflare Pages

1. Create a free Cloudflare account
2. Pages → Create project → Direct upload
3. Drag the folder, live in 30 seconds with a `pages.dev` URL

## Customization

- **Update LinkedIn / GitHub URLs:** open `about.html`, find the `[paste your LinkedIn URL]` placeholders, replace with real URLs.
- **Change accent color:** open `style.css`, find `--coral: #e87a6a;` and replace with your preferred color.
- **Change typography:** Inter / Inter Tight / JetBrains Mono are loaded from Google Fonts at the top of `style.css`. Swap in any other Google Fonts.
- **Add more case studies:** duplicate any of the page files (e.g., `case-study-2.html`), update the nav in all pages, link from `index.html`.

## Browser support

Modern browsers (Chrome, Edge, Firefox, Safari, Arc). Uses CSS variables, backdrop-filter, and modern flexbox/grid. Tested at 1280px, 1440px, and mobile (375px width).

— Jenil Gohel · 2026
