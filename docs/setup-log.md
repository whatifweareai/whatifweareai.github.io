# Setup log

Newest entry first. No secrets here: names and IDs only.

## 2026-11-10: Umami Cloud replaces Google Analytics

**Why:** Umami sets no cookies and stores no personal data, so no consent banner is needed. Google Analytics 4 needed one for EU/UK (and arguably Canadian) visitors.

**Created, in Umami Cloud, by the site owner:**
- Account on the free Hobby plan (100k events a month, 1 website, 6 months of data), data region US. Signed up with the book's Gmail account (address kept in the private accounts file, not in this repo).
- Website: `whatifweareai.com` (domain `whatifweareai.com`), website ID `25e958a2-6058-447c-b336-c760feccd8a7` (public, it is in the page source).

**Wired into the site:** `umami_id` in `_config.yml`, rendered by `_includes/analytics.html` (production builds only). The `ga4_id` setting and the GA4 snippet were removed.

**Google Analytics:** the property `The Hum website` (measurement ID `G-6HVCT6L5DB`) still exists in the GA console but receives no data now. Delete it in GA Admin when no longer wanted.

**Undo:** set `umami_id: ""` to stop tracking; delete the website in Umami to remove its data.

**Still open:** the free plan keeps 6 months of data; export before then if older data matters.

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
