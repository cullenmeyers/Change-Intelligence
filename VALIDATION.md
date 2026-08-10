# Site Validation

## Current pivot — August 10, 2026

The passive WooCommerce payment-issue test did not show enough SEO momentum to keep building that wedge as a content engine. The domain remains useful, but the current test is now a developer/API change wedge:

- Hub: `/api-changes/`
- Shopify 2026-10 invalid metafield filter errors
- Shopify expiring offline access tokens required for public apps by January 1, 2027
- Shopify `returnProcess` migration from legacy return refund APIs
- Stripe API version 2026-07-29.dahlia versioning checklist
- GitHub REST API versioning and `X-GitHub-Api-Version` checklist

The new hypothesis is that developers search for official API changes, breaking changes, deprecations, version deadlines, and migration risks more consistently than store owners search for temporary WooCommerce plugin incidents.

## What changed in strategy

Previous broad idea:

- WordPress plugin changes and WooCommerce payment issue records.

Problem found:

- Google discovered pages, but impressions and clicks did not compound.
- The site reached 6 Google clicks and 390 impressions by the August 10 review, but there were no new clicks after the early July spike.
- Hub and alert pages did not get enough passive search exposure to prove demand.

New test:

- Developer/API change explainers.
- More evergreen version/deprecation pages.
- Official source-based migration checklists.
- Initial batch locked at one hub plus five records.

## Validation timeline

- WooCommerce payment test start: June 18, 2026
- WooCommerce payment test paused: August 10, 2026
- API changes pivot launched: August 10, 2026
- Next API pivot review: August 24, 2026

## API pivot decision rules

### Continue

Continue if the API change pages show at least one of:

- faster indexing than the WooCommerce pages
- relevant impressions from API/version/deprecation queries
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
- whether queries mention API version, breaking change, deprecation, migration, error, webhook, token, or SDK
- Vercel visits to `/api-changes/` and the five API records

## Previous test kept live

The WooCommerce payment issue records, hub, and alert page remain live as archived validation assets, but they are no longer the main build direction.

## Guardrails

- Do not delete the WooCommerce pages yet.
- Do not add 20 API pages immediately.
- Do not add unsupported summaries without official sources.
- Do not rely on broad product news or generic changelog summaries.
- Do not judge the pivot before Google has had time to index the new hub and five records.
