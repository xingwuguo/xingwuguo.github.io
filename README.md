# Surface Science & Film Technology Lab

This repository hosts the official Jekyll-based personal academic/research website for **Dr. Xingwu Guo** and his laboratory at Shanghai Jiao Tong University (SJTU).

Website: [https://xingwuguo.github.io/](https://xingwuguo.github.io/)

---

## Technology Stack

- **Static Site Generator:** [Jekyll](https://jekyllrb.com/) (using the [Minima](https://github.com/jekyll/minima) theme)
- **Internationalization:** [jekyll-multiple-languages-plugin](https://github.com/untra/jekyll-multiple-languages-plugin)
- **SEO & Metadata:** [jekyll-seo-tag](https://github.com/jekyll/jekyll-seo-tag), [jekyll-sitemap](https://github.com/jekyll/jekyll-sitemap)
- **Deployment:** GitHub Actions with `jeffreytse/jekyll-deploy-action`

---

## Project Structure

- `docs/`: Root directory for the Jekyll project.
- `docs/_i18n/`: Translation files (YAML) and localized markdown content (folders `en/` and `cn/`).
- `docs/_pages/`: Page entry points using Liquid templates to pull localized content.
- `docs/assets/images/`: Standardized image assets (English naming convention).
- `docs/assets/成功案例/` & `docs/assets/可转移技术/`: Technical documents (PDF/DOCX).

---

## Multi-language Support

The site supports **English** and **Chinese**. 
- Translations are managed in `docs/_i18n/en.yml` and `docs/_i18n/cn.yml`.
- Page content is synchronized between `docs/_i18n/en/*.md` and `docs/_i18n/cn/*.md`.
- Use the language toggle in the header to switch between versions.

---

## SEO & Google Search Console

To ensure the site is correctly indexed and marketed to industrial partners:

1. **Sitemap Generation:** The site automatically generates a `sitemap.xml` and `robots.txt` pointing to it.
2. **Production Build:** SEO features (like Google Analytics and absolute sitemap URLs) are only activated in the production environment.
3. **Manual Indexing Request:**
   - Log in to your [Google Search Console](https://search.google.com/search-console).
   - Add the property: `https://xingwuguo.github.io/`.
   - Go to **Sitemaps** and submit `sitemap.xml`.
   - Use the **URL Inspection** tool to request indexing for the homepage if you want to speed up the process.

---

## Local Development

To run the site locally for testing and content updates:

1. Navigate to the `docs/` directory:
   ```bash
   cd docs
   ```
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Start the development server:
   ```bash
   bundle exec jekyll serve
   ```
   Access at: `http://127.0.0.1:4000/`

### Testing Production Features Locally
To verify the sitemap or Google Analytics locally, run:
```bash
JEKYLL_ENV=production bundle exec jekyll build
```
The output will be in `docs/_site/`. Note that `jekyll serve` will override the production sitemap with local links.

---

## Deployment

**Automated Deployment:** 
Every push to the `xingwuguo` branch triggers a GitHub Actions workflow (`.github/workflows/build-jekyll.yml`). This builds the site with `JEKYLL_ENV=production` and deploys it to the `gh-pages` branch.

---

## Asset Guidelines

- **Images:** Always use standardized English names (lowercase, hyphens, e.g., `magnesium-anodizing.jpg`) for better SEO and file management.
- **Documents:** Technical PDFs and DOCXs for Success Cases and Transferable Technologies should maintain their original Chinese filenames to serve domestic industrial partners accurately.
