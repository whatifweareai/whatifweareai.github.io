# The Hum: What If? We Are AI (launch page)

Jekyll launch page for the book. Book text on the site is limited to six short passages in `inside.html`, about 1% of the book, taken word for word from the published chapters.

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

## Design

`assets/img/hum.svg` is the waveform that continues the one on the cover, and `assets/img/nodes.svg` is the faint network behind the page. Literata and Archivo are self-hosted in `assets/fonts/`, under the SIL Open Font License. The Archivo file holds only the letters of the title and subtitle, so changing either one means regenerating it.
