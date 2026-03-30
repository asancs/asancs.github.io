# Alejandro Sánchez — Academic Personal Site

A static academic personal website built with plain HTML, CSS, and minimal JavaScript. Ready for GitHub Pages.

## Structure

```
alejandro-site/
├── index.html          ← About Me
├── research.html       ← Research page
├── cv.html             ← Web CV
├── styles.css          ← All styles
├── script.js           ← Nav toggle + active link
├── YOUR_CV_FILE.pdf    ← ⚠️ Replace with your actual PDF
├── .github/
│   └── workflows/
│       └── pages.yml   ← Auto-deploy to GitHub Pages
└── README.md
```

## Before deploying

1. **Replace** `YOUR_CV_FILE.pdf` with your actual CV PDF file (keep the same filename, or update references in all three HTML files).
2. **Verify** `YOUR_LINKEDIN_URL` → already set to `https://linkedin.com/in/sanchezalejandro` in the HTML.
3. **Verify** `YOUR_EMAIL` → already set to `alejandro-737@hotmail.com` in the HTML.

## Deploy to GitHub Pages

### Option A — Automatic (recommended)

1. Create a new repository on GitHub (e.g., `alejandro-sanchez-site` or `yourusername.github.io`).
2. Push all files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
3. Go to **Settings → Pages** in your repository.
4. Under **Source**, select **GitHub Actions**.
5. The workflow at `.github/workflows/pages.yml` will run automatically and deploy your site.
6. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`

### Option B — Manual (simpler)

1. Push files to a repo named exactly `YOUR_USERNAME.github.io`.
2. Go to **Settings → Pages → Source: Deploy from branch → main → / (root)**.
3. Site live at `https://YOUR_USERNAME.github.io`.

## Customization

- **Colors**: Edit CSS variables in `:root {}` block at the top of `styles.css`.
- **Content**: Edit the HTML files directly — each section is clearly commented.
- **Fonts**: The site uses Google Fonts (Cormorant Garamond, Source Serif 4, DM Mono). Works offline only if you self-host them.
