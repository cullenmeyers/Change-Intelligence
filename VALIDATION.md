# Site Validation

## Current pivot — August 18, 2026

The passive WooCommerce payment-issue test did not show enough SEO momentum to keep building that wedge as a content engine. The domain remains useful, but the current test is now a developer/API change wedge.

Initial API pivot assets:

- Hub: `/api-changes/`
- Shopify 2026-10 invalid metafield filter errors
- Shopify expiring offline access tokens required for public apps by January 1, 2027
- Shopify `returnProcess` migration from legacy return refund APIs
- Stripe API versioning and safe upgrade checklist
- GitHub REST API versioning and `X-GitHub-Api-Version` checklist

The new hypothesis is that developers search for official API changes, breaking changes, deprecations, version deadlines, authentication changes, webhook risks, SDK versioning, and migration problems more consistently than store owners search for temporary WooCommerce plugin incidents.

## What changed in strategy

Previous broad idea:

- WordPress plugin changes and WooCommerce payment issue records.

Problem found:

- Google discovered pages, but impressions and clicks did not compound.
- The site reached 6 Google clicks and 390 impressions by the August 10 review, but there were no new clicks after the early July spike.
- Hub and alert pages did not get enough passive search exposure to prove demand.

New test:

- Developer/API change explainers.
- More evergreen version/deprecation/authentication pages.
- Official source-based migration checklists.
- Initial batch locked at one hub plus five records.

## Validation timeline

- WooCommerce payment test start: June 18, 2026
- WooCommerce payment test paused: August 10, 2026
- API changes pivot launched: August 10, 2026
- First API pivot read: August 18, 2026
- Next API pivot review: August 24, 2026

## First API pivot read — August 18, 2026

Google Search Console data through August 16 showed 477 total impressions and 6 total clicks. The prior week, August 2-8, had 9 impressions. The first API pivot week, August 9-16, had 87 impressions. There were still no new Google clicks.

API pages visible in the Pages export:

- Shopify returnProcess API: 0 clicks, 8 impressions, average position 50.6
- Shopify expiring offline access tokens: 0 clicks, 7 impressions, average position 39.4
- Stripe API version page: 0 clicks, 6 impressions, average position 6.5
- GitHub REST API versioning: 0 clicks, 5 impressions, average position 46.2

Decision from August 18 review:

- Keep the API pivot alive for one more review cycle because impressions increased from 9 to 87 week-over-week.
- Do not add new records yet.
- Refine the pages that already showed impressions.
- Reframe the Stripe page from a one-version page into a broader Stripe API versioning and safe-upgrade checklist.
- Add clearer developer-search language to the Shopify expiring offline access token page.
- Recheck around August 24 before adding pages or changing the wedge again.

## API pivot decision rules

### Continue

Continue if the API change pages show at least one of:

- faster indexing than the WooCommerce pages
- relevant impressions from API/version/deprecation/authentication queries
- clicks from developer-intent searches
- repeat visits or alert/event interest from API pages

### Refine

Refine titles, summaries, or record format if pages index but queries are too broad, irrelevant, or not tied to migration decisions.

### Stop or pivot again

Stop the API wedge if it gets indexed but remains at near-zero impressions/clicks after 2-3 weeks.

## What to measure

For the API pivot, capture by page:

- Google indexing status
- impressions
- clicks
- queries
- average position
- whether queries mention API version, breaking change, deprecation, migration, error, webhook, token, OAuth, SDK, or versioning
- Vercel visits to `/api-changes/` and the five API records

## Previous test kept live

The WooCommerce payment issue records, hub, and alert page remain live as archived validation assets, but they are no longer the main build direction.

## Guardrails

- Do not delete the WooCommerce pages yet.
- Do not add 20 API pages immediately.
- Do not add unsupported summaries without official sources.
- Do not rely on broad product news or generic changelog summaries.
- Do not judge the pivot before Google has had time to index the new hub and five records.
