# Xingwu Guo Lab Website

This repository hosts the Jekyll site for https://xingwuguo.github.io/.

## Structure
- Site source lives in `docs/`.
- Built output is generated into `docs/_site/` (ignored by Git).
- Main stylesheet entrypoint is `docs/assets/main.scss`.

## Deployment
Deployment is handled by the GitHub Actions workflow in `.github/workflows/build-jekyll.yml`.
It uses `jeffreytse/jekyll-deploy-action` to build the site from this repo’s `docs/Gemfile` and publish to the `gh-pages` branch.  
This means the build environment is controlled by the Gemfile, not GitHub Pages’ built-in Jekyll.

## Theme overrides (Sass)
The Minima theme (version 2.5.2) is customized with minimal overrides.

- Main stylesheet entrypoint is `docs/assets/main.scss` with variable overrides before `@import "minima";` and custom styles after.
- Sass deprecation warnings from dependencies suppressed with `sass: quiet_deps: true` in `_config.yml`.

## Analytics
Google Analytics is configured via `_config.yml`:
```
google_analytics: G-YXCBMGS22L
```
The script is injected by `docs/_includes/google-analytics.html` and only loads when `JEKYLL_ENV=production`.

To test GA locally:
```
JEKYLL_ENV=production bundle exec jekyll serve
```

## Baidu Map AK
Baidu Maps AK is configured in `_config.yml` and referenced in the contact pages:
```
baidu_map_ak: <your-ak>
```
Used in:
- `docs/_i18n/en/09_contact.md`
- `docs/_i18n/cn/09_contact.md`

## Local development
From `docs/`:
```
bundle install
bundle exec jekyll serve
```
The site will be available at http://127.0.0.1:4000/.
