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
3. `noindex: true` in `_config.yml` keeps search engines out. Set it to `false` to be listed.
4. Replace the "Coming soon" badge in `index.md` with buy links once the book is live.
