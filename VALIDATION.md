# Initial Site Validation

## Scope lock

The first public validation set launched with four decision records:

1. WooCommerce Stripe 10.8.x payment status not updating
2. Mollie Payconiq removal
3. WooCommerce PayPal Pay with Crypto enabled by default
4. WP Super Cache requiring WordPress 6.8

After the first review on June 25, 2026, one additional operational record was added because the strongest early search signal came from the active payment-incident pattern:

5. WooCommerce PayPal Payments 4.0.4 amount mismatch

After the delayed second review on July 6, 2026, the site showed enough repeated payment/revenue signal to justify one controlled batch of three more operational records:

6. WooCommerce Stripe 10.8.3 checkout error after update
7. WooCommerce Stripe shipping cost not charged
8. Mollie cancelled payment order note loop

After the July 13, 2026 review, the site again showed that operational payment, checkout, shipping, and reconciliation pages were the strongest direction. One page with impressions but no clicks was title-tested, and one more controlled batch of three operational records was added:

9. WooCommerce Stripe captures 1/100 amount with WPML Multi-Currency
10. WooCommerce PayPal total missing shipping
11. WooCommerce PayPal/card payments fail intermittently with OrderProcessor.php:109

After the July 20, 2026 main review, public record expansion was paused. The broad WordPress-plugin-change version looked too weak for a simple SEO content machine, but the narrower WooCommerce payment-issue direction remained the strongest signal. Instead of adding more records, a hub page was created:

- WooCommerce payment issues tracker: `/woocommerce-payment-issues/`

The validation set is now locked at eleven records plus one hub page until the next review. New changes may be researched and queued privately, but the public site should not expand until the hub has been indexed and the July 13 pages have had more time to settle.

## Validation start

- Start date: June 18, 2026
- First review: June 25, 2026
- Delayed second review: July 6, 2026
- Third review: July 13, 2026
- Main decision review: July 20, 2026
- Next review: July 27, 2026

## First review notes — June 25, 2026

Google Search Console showed early discovery across the site. The Stripe payment-status record produced the clearest signal with all recorded Google clicks in the first cohort. This did not prove the business, but it justified one more test page in the same urgent operational-decision family.

Decision from first review:

- Continue, but do not scale volume yet.
- Add exactly one more urgent operational record.
- Keep tracking whether payment-incident pages outperform compatibility, default-change, or capability-removal pages.
- Do not judge the market from Vercel visitor count alone because some visits may come from owner testing, email recipients, previews, or link checks.

## Delayed second review notes — July 6, 2026

Google Search Console export through July 4 showed 131 impressions and 4 clicks. All clicks came from the WooCommerce Stripe payment-status incident page. The WooCommerce PayPal amount-mismatch page also generated fast impressions shortly after publication, even before clicks.

Decision from delayed second review:

- Continue.
- Expand from five records to eight records with one controlled batch.
- Keep the batch focused on operational pain: checkout failure, revenue mismatch, order/payment reconciliation, database/server load.
- Do not add broad compatibility, general changelog, affiliate, or comparison pages yet.
- Review again on July 13 before adding more public records.

## Third review notes — July 13, 2026

Google Search Console data through July 11 showed 311 total impressions and 6 clicks. The strongest pattern remained urgent WooCommerce/Stripe/payment/revenue incidents. The Stripe payment-status page remained the strongest page, and the new July 6 Stripe operational pages generated fast impressions and some clicks.

Decision from third review:

- Continue.
- Rewrite the PayPal amount-mismatch title to emphasize the concrete pain: discount applied twice / amount mismatch.
- Add one controlled batch of three more records in the same category: amount capture error, shipping total mismatch, and intermittent PayPal/card failure.
- Keep the site locked at eleven records until the next review.
- Review again around July 20 before adding more pages.

## Main review notes — July 20, 2026

Google Search Console data through July 18 showed the site was not compounding like a broad SEO content engine. The strongest pages were still payment, checkout, and order-money issues, but impressions slowed after the prior peak. The interpretation changed from "publish more individual pages" to "tighten the product surface around the winning pattern."

Decision from main review:

- Do not add more individual records right now.
- Keep the eleven existing records locked.
- Create a WooCommerce payment issues hub to group the strongest category into one clearer product surface.
- Treat the next test as whether the hub improves internal linking, product clarity, and search understanding.
- Recheck on July 27, 2026.

## What to measure

### 1. Indexing

For each record and the hub, capture:

- Google indexing status
- first indexed date
- whether the canonical selected by Google matches the permanent URL

### 2. Search demand

From Google Search Console, capture by page:

- impressions
- clicks
- queries
- average position
- whether queries show decision intent rather than only plugin-name navigation

Examples of useful intent include questions about whether to update, migrate, disable, reconcile, restore checkout, audit orders, or change configuration.

### 3. Visits and referrals

From Vercel Web Analytics, capture by page:

- visitors
- views
- referrer/source
- country only when useful for interpreting a region-specific change

The purpose is to distinguish Google discovery from direct links, support-thread referrals, email outreach, and manual sharing.

### 4. Recommendation usefulness

Ask at least one relevant WordPress user, developer, agency operator, or store owner to review the WooCommerce payment issues hub:

- Can you tell what kind of problems this tracker is for?
- Can you quickly find the issue closest to your situation?
- Is the recommended first action clear?
- What information is still missing before you would trust or use it?

Record the answer, not just a yes/no score.

### 5. Freshness

Recheck source evidence when the underlying change is still active:

- Stripe incident: recheck official releases and support status when a new release appears
- Mollie Payconiq: recheck if Payconiq is restored, replaced, or addressed in a later release
- PayPal Pay with Crypto: recheck when eligibility, defaults, or documentation changes
- WP Super Cache: recheck when requirements or the current release change
- PayPal amount mismatch: recheck if 4.1.x follow-up releases, reopened support threads, or additional mismatch reports appear
- Stripe 10.8.3 checkout error: recheck for official fix, new support responses, or changelog mentions of Stripe.js conflicts
- Stripe shipping cost mismatch: recheck if additional reports appear or a specific release confirms a fix
- Mollie order note loop: recheck if a release explicitly fixes repeated order notes, abandoned-payment loops, or stale pending-payment cleanup
- Stripe WPML 1/100 amount capture: recheck if thread details, plugin responses, or confirmed fixes appear
- PayPal shipping total mismatch: recheck if thread details, plugin responses, or confirmed fixes appear
- PayPal OrderProcessor.php:109 intermittent failures: recheck for a confirmed fix, issue link, or new release notes mentioning order-processing timing or webhook recovery

## Decision rules

### Continue and expand carefully

Continue when pages are indexed and at least some records show relevant non-branded impressions, useful referrals, or clear user-action value. Add the next record only after identifying which page pattern produced the strongest signal.

### Refine before expanding

Refine when pages are indexed but the queries or referrals do not match the intended decision. Change the angle, title, summary, decision framing, or hub organization before adding volume.

### Investigate distribution or technical problems

Investigate when pages are not indexed, Google selects a different canonical, analytics receives no real visits after distribution, or users cannot tell what action to take.

## Prohibited during the current validation window

- Do not expand to 15-25 public pages.
- Do not redesign the site.
- Do not add broad comparison or affiliate content.
- Do not repeatedly request indexing every day.
- Do not change several variables at once.
- Do not judge the market from raw traffic alone; query intent and action usefulness matter more at this stage.
