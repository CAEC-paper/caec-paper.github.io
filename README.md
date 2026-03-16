# Paper Page Starter

This folder contains a cleaned-up version of the
[Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
for a paper website.

## What to edit first

Open [index.html](/home/netsys1/test/paper-page/index.html) and replace:

- `Your Paper Title`
- author names and links
- venue/year
- abstract
- button links for PDF, arXiv, code, and demo
- BibTeX block
- GitHub Pages URLs like `https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPOSITORY_NAME/`

Then replace these files:

- `static/pdfs/paper.pdf` with your actual paper PDF
- `static/images/carousel1.jpg` with your main teaser figure
- `static/images/carousel2.jpg`, `carousel3.jpg`, `carousel4.jpg` with your result figures
- `static/images/social_preview.png` with a 1200x630 preview image for sharing
- `static/images/favicon.ico` with your own favicon

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish on GitHub Pages

### Option 1: Repo named `yourusername.github.io`

1. Create a GitHub repo named exactly `yourusername.github.io`.
2. Push the contents of this folder to that repo.
3. Your site will be live at:

```text
https://yourusername.github.io/
```

### Option 2: Normal repo name like `my-paper-page`

1. Create a GitHub repo such as `my-paper-page`.
2. Push the contents of this folder to that repo.
3. On GitHub, go to `Settings` -> `Pages`.
4. Under `Build and deployment`, choose:
   `Deploy from a branch`
5. Select:
   `main` branch and `/ (root)` folder
6. Save, then wait about 1-2 minutes.

Your site URL will be:

```text
https://yourusername.github.io/my-paper-page/
```

## Push commands

If you want to publish this exact folder as a new repo:

```bash
cd /home/netsys1/test/paper-page
git remote remove origin
git branch -M main
git add .
git commit -m "Set up paper project page"
git push -u origin main
```

## Notes

- The file `.nojekyll` is already included, which is good for GitHub Pages static sites.
- If your page shows broken links after publishing, check that your URLs include the repo name for non-user sites.
- If you do not need a section in `index.html`, delete it instead of leaving placeholder text.
