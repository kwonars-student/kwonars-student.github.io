# SoonUk Kwon — Research Portfolio

A zero-build static site designed for research-intern recruiting. It can be published directly with GitHub Pages.

## Before publishing

1. Replace `YOUR_EMAIL@EXAMPLE.COM` in `index.html`.
2. Put your current PDF CV at `assets/SoonUk_Kwon_CV.pdf`.
3. Verify author roles and venue wording.
4. Replace the abstract SVG/CSS visuals with project figures or short muted MP4/WebM clips if you have publication-safe assets.

## Clarity rules used in this site

- Hero identity: 1 line.
- Hero positioning: 1 sentence, ~20 words.
- Project problem: ideally <= 12 words before the colon.
- Project contribution: 1 sentence, ideally <= 24 words.
- Methods/evidence: max 3 tags on the homepage.
- Ongoing projects: title + one sentence only; no unpublished results.
- Future direction: exactly 1 question + 1 sentence.

The homepage is intentionally layered for three reading depths:

- ~10 seconds: identity, point of view, signature project.
- ~1 minute: repeated reality-centered research pattern.
- ~3 minutes: capability, methods, trajectory, and next question.

## Publish as `username.github.io`

Create a GitHub repository named exactly `YOUR_GITHUB_USERNAME.github.io`, then push the contents of this folder to the repository root.

### Terminal method

```bash
cd soonuk-research-portfolio
git init
git add .
git commit -m "Launch research portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME.github.io.git
git push -u origin main
```

Then on GitHub open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.

Your site will be available at:

`https://YOUR_GITHUB_USERNAME.github.io/`

## Publish from another repository name

If you use a repository such as `portfolio`, GitHub Pages can also publish it at:

`https://YOUR_GITHUB_USERNAME.github.io/portfolio/`

Because this template uses relative file paths, it works in either setup.

## Notes

- `.nojekyll` is included so GitHub Pages serves this static site directly.
- No framework or build step is required.
- The site is responsive and uses only HTML/CSS/JS.
- GitHub Pages sites are public on the web. Do not include confidential or under-review results you do not want publicly accessible.

## Optional: keep the site out of search results

If you want to share the URL only through your CV/application, add this inside `<head>` in `index.html`:

```html
<meta name="robots" content="noindex, nofollow">
```

This discourages search-engine indexing, but it is **not a security control**. Anyone with the URL can still open a GitHub Pages site.
