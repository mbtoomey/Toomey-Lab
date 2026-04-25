# Toomey Lab Website

Academic lab website for the Toomey Lab at the University of Tulsa. Built as a static HTML/CSS site for hosting on GitHub Pages.

## Pages

- `index.html` — Home / overview
- `research.html` — Research themes
- `publications.html` — Full publication list with publisher links
- `people.html` — Lab members and alumni
- `teaching.html` — Courses taught
- `join.html` — How to join the lab

## How to deploy on GitHub Pages

### Option A: New repository

1. Create a new repository at https://github.com/new (e.g., `mbtoomey.github.io` or `lab-website`)
2. Upload all files in this folder to the repository
3. Go to **Settings → Pages**
4. Under "Source", select **Deploy from a branch → main → / (root)**
5. Click Save — your site will be live at `https://mbtoomey.github.io/` (or `https://mbtoomey.github.io/lab-website/`)

### Option B: Using existing repository

If adding to an existing repo, put all files in a `/docs` folder, then set GitHub Pages source to `main → /docs`.

### Option C: Command line

```bash
git init
git add .
git commit -m "Initial lab website"
git remote add origin https://github.com/mbtoomey/YOUR-REPO-NAME.git
git branch -M main
git push -u origin main
```

Then enable GitHub Pages in repository Settings.

## Updating publications

The `publications.html` page lists all publications with direct links to publisher websites. To add new papers:
1. Open `publications.html`
2. Add a new `<li class="pub-item">` entry at the top of the appropriate year section
3. Link to the publisher DOI/URL rather than a local PDF

## Images

Lab member photos are in the `images/` folder. To update a photo, replace the file with the same name, or update the `src` attribute in `people.html`.
