# Setup log

Newest entry first. No secrets here: names and IDs only.

## 2026-11-10: Google Analytics 4 for whatifweareai.com

**Why:** to see how much traffic the book's launch page gets.

**Created, in the Google Analytics console, by the site owner:**
- Account: `whatifweareai`
- Property: `The Hum website` (time zone India, currency INR, industry Books & Literature, size Small)
- Web data stream: `whatifweareai.com` (`https://whatifweareai.com`), stream ID `16306476225`, Enhanced measurement on (page views, scrolls, outbound clicks and more)
- Measurement ID: `G-6HVCT6L5DB` (not secret, it is visible in the page source)

**Identity:** created while signed in to the site owner's Google account (the address is not recorded in this repo). Account data-sharing boxes were left at Google's defaults (modeling contributions, technical support and recommendations on; Google products & services off).

**Wired into the site:** `ga4_id` in `_config.yml`, rendered by `_includes/analytics.html`, only in production builds.

**Checked (2026-11-10):** after deploy, `G-6HVCT6L5DB` is in the served HTML of the home page and `/inside/`. A visit from Chrome showed as 1 active user (India) in GA Home. Full reports can take up to 48 hours. More detail: `wiki/analytics/` in the book-meta repo.

**Undo:** set `ga4_id: ""` in `_config.yml` to stop tracking; delete the property in GA Admin to remove the data.

**Still open:**
- Google shows a separate Google tag container (`GTM-...`) in the stream's install view. It is not used; the site uses the `G-` ID directly.
- EU/UK visitors strictly need consent before GA cookies are set. There is no consent banner yet.
