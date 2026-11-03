# The Hum: What If? We Are AI (launch page)

Jekyll launch page for the book. No book text is published here: only the title, tagline, description and cover.

## Preview

```bash
bundle install
bundle exec jekyll serve
```

## Publish

1. The repo is `whatifweareai.github.io`, so the site is served at the root: https://whatifweareai.github.io/ (`baseurl` stays empty).
2. Repo settings > Pages > Source: GitHub Actions. Pushing to `main` deploys.
3. `noindex` in `_config.yml` is `false`, so search engines may list the site. `robots.txt` and `sitemap.xml` are generated from `url` in the same file.
4. The buy links for Amazon India, US and Canada are `buy_links` in `_config.yml`.
