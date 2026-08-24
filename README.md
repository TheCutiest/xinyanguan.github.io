# xinyanguan.github.io

Personal academic homepage for Xinyan Guan. Pure static HTML/CSS — no build step, no framework.

## Structure

```
index.html   — all page content (edit sections directly here)
style.css    — styling
assets/      — images, CV
```

## Editing content

Everything lives in `index.html`, organized into clearly commented sections:

- **Header / About** — name, affiliation, research interests, bio, contact links
- **Research** — three publication cards (ETCO, ECGTwin, WearECG), each with title, authors, venue, links, teaser image
- **Education**
- **Research Experience** — edit the placeholder `<li>` entries in the list
- **Contact**

Still to fill in:

- ETCO "Paper" `href="#"` → arXiv URL, once available
- CV link — currently removed from the header nav (not ready to make it public). To re-add: drop your PDF in `assets/`, then uncomment the CV link in `index.html` (commented out next to the Google Scholar link) and point its `href` at the file.

Already filled in:

- Email: `xinyanguan015@gmail.com` (header link + contact section)
- Google Scholar link
- Paper/Code links: ECGTwin (arXiv), WearECG (PLOS Digital Health paper + GitHub code)
- `assets/profile.png`, `assets/etco-teaser.png`, `assets/ecgtwin-teaser.png`, `assets/ecg-reconstruction-teaser.png` — real images; replace the file to update
- Research Experience: UCL (advised by He Wang, Sep 2025–Now), Peking University (advised by Shenda Hong, Apr–Oct 2025)

All three teaser images render at the same fixed size (`.paper-media`, 240×180, 4:3) using `object-fit: contain`, so scientific figures of any aspect ratio display in full without cropping.

## Local preview

Just open `index.html` directly in a browser — all paths are relative, no server required.

## Deploying with GitHub Pages

This repo is already named `xinyanguan.github.io`, so GitHub Pages will serve it from the root automatically once enabled:

1. Push `index.html`, `style.css`, and `assets/` to the `main` branch.
2. On GitHub: **Settings → Pages → Build and deployment → Source** → set to **Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)` → **Save**.
4. Site will be live at `https://TheCutiest.github.io/` within a minute or two.

No further configuration needed — no Jekyll, no `_config.yml`, no build step.
