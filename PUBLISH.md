# Publish this static site to GitHub Pages

This folder is a complete static website. It is designed to replace the current generated GitHub Pages output; do **not** copy it inside the existing React `src/` folder.

## Push in about one minute

1. Download this `seo_site` folder to your computer.
2. Open a terminal and run these commands, replacing `/path/to/seo_site` with the downloaded folder’s actual path.

```bash
git clone https://github.com/Yusuf-Gadelrab/Yusuf-Gadelrab.github.io.git
cd Yusuf-Gadelrab.github.io
git fetch origin
git checkout gh-pages
git pull --ff-only origin gh-pages
rsync -av --delete --exclude='.git/' /path/to/seo_site/ ./
git add -A
git commit -m "Rebuild personal site for search"
git push origin gh-pages
```

If `git checkout gh-pages` says the branch does not exist, use `git checkout -b gh-pages`, then run the remaining commands and push with `git push -u origin gh-pages`. In GitHub repository **Settings → Pages**, select **Deploy from a branch**, then choose `gh-pages` and `/ (root)`.

## Post-publish checklist

- Open `https://yusuf-gadelrab.github.io` in an incognito/private window and confirm the Home, Research, IntakeKit, Writing, and About links work.
- Submit `https://yusuf-gadelrab.github.io/sitemap.xml` in [Google Search Console](https://search.google.com/search-console) and [Bing Webmaster Tools](https://www.bing.com/webmasters/).
- Add `https://yusuf-gadelrab.github.io` to the Website field on LinkedIn and the profile/bio link on GitHub.
- Request indexing for the home page and research page in Google Search Console after the Pages deployment is visible.
