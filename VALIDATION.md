# Site Validation

## Current pivot — September 7, 2026

What Just Changed is no longer being treated as a broad passive SEO site or a broad API-change site. The current direction is a tighter productized wedge:

> Revenue-stack breakage radar for ecommerce merchants.

The job to solve:

> A software update or payment-flow issue changed something, and now checkout, captured funds, order status, totals, shipping, tax, refunds, webhooks, payouts, or reconciliation may be wrong. What changed, am I affected, how do I verify it, and what is the safest next action?

## Why this pivot happened

Google Search Console through September 5 showed 8 total clicks and 692 total impressions.

The API pivot got discovered, but it did not get clicks:

- API pivot pages: 0 clicks, about 188 impressions.
- Shopify Returns API page: meaningful impressions, but still around position 47 and 0 clicks.
- Stripe API versioning page: closer average position, but still 0 clicks.

The only pages that produced real Google clicks were older urgent payment/revenue-risk pages:

- WooCommerce Stripe payment status not updating.
- WooCommerce Stripe 10.8.3 checkout error after update.
- Stripe charged an order without shipping cost.

Decision:

- Stop treating broad API changes as the main wedge.
- Do not delete the API pages; keep them live as a secondary archive.
- Reposition the homepage and WooCommerce payment hub around revenue-stack breakage.
- Create one evergreen recovery/checklist page instead of adding many incident pages.

## Current live validation assets

Primary assets:

- Homepage: `/`
- Recovery guide: `/payment-recovery/`
- Revenue breakage tracker: `/woocommerce-payment-issues/`
- Alert product test: `/woocommerce-payment-alerts/`

Existing issue records kept live:

- WooCommerce Stripe 10.8.x payment status not updating.
- WooCommerce Stripe 10.8.3 checkout error after update.
- WooCommerce PayPal 4.0.4 discount applied twice / amount mismatch.
- Stripe shipping cost not charged.
- Stripe WPML Multi-Currency 1/100 amount.
- PayPal shipping not included total.
- PayPal OrderProcessor.php:109 intermittent failures.
- Mollie cancelled payment order note loop.
- Mollie Payconiq removed.
- WooCommerce PayPal Pay with Crypto enabled by default for eligible merchants.

Secondary archive:

- API changes hub and five API records remain live, but they are no longer the main build direction.

## Evidence model

Every revenue-breakage record should use one of these labels:

### Confirmed fix

A vendor changelog, official issue, or official source explicitly identifies the defect and fix.

Use this when the page can safely say a fix exists or a version boundary is confirmed.

### Vendor acknowledged

An official support channel, official GitHub issue, or vendor response recognizes the behavior, but the final fix or complete affected-version range may still be unclear.

Use this when the issue is real but the safest action is to preserve evidence and follow official updates.

### Diagnostic match

Symptoms match a known pattern, but causality is not fully confirmed.

Use this when the page should help users verify their own order/gateway/webhook/amount evidence before taking action.

## Validation timeline

- WooCommerce payment test start: June 18, 2026
- WooCommerce payment test paused as broad content wedge: August 10, 2026
- API changes pivot launched: August 10, 2026
- API pivot judged weak: September 7, 2026
- Revenue-stack breakage pivot launched: September 7, 2026
- Next review: September 21, 2026

## What changed on September 7

Implemented the first foundation step:

- Repositioned homepage from API changes to revenue-stack breakage.
- Created `/payment-recovery/` as an evergreen WooCommerce payment recovery and reconciliation checklist.
- Reframed `/woocommerce-payment-issues/` as a revenue breakage tracker.
- Reframed `/woocommerce-payment-alerts/` as a saved-stack alert product test.
- Added evidence status labels: Confirmed fix, Vendor acknowledged, Diagnostic match.
- Updated sitemap lastmod values for the changed pages.

## Current hypothesis

The best surviving hypothesis is:

> People searching after a revenue-impacting software change will consume a precise diagnostic/recovery record, save their payment stack, and some will pay to be warned before or immediately after the next damaging change.

This is more product-like than the original content site because the content, lead magnet, alerts, and future scanner all solve the same recurring problem.

## What to measure next

For the next review, measure:

- GSC impressions for `/payment-recovery/`.
- GSC impressions and clicks for `/woocommerce-payment-issues/`.
- GSC clicks on the three already-proven Stripe/WooCommerce pages.
- Vercel visits to `/payment-recovery/`.
- Vercel visits to `/woocommerce-payment-alerts/`.
- Custom events:
  - `RecoveryGuideClick`
  - `PaymentHubClick`
  - `AlertInterestClick`
  - `AlertSignupClick`
  - `ReportIssueClick`
- Any email asking for stack alerts.

## Continue / refine / stop rules

### Continue

Continue if the revenue-breakage direction shows at least one of:

- Recovery guide impressions within 2 weeks.
- New clicks to recovery, pending-payment, checkout-error, or amount-mismatch pages.
- Alert page visits from issue/recovery pages.
- AlertSignupClick or real email interest.
- Better trailing 28-day organic clicks than the API pivot.

### Refine

Refine if pages get impressions but no clicks:

- Tighten titles around actual queries.
- Make snippets more symptom-led.
- Improve recovery sections on pages already getting impressions.
- Add clearer CTAs to save a payment stack.

### Stop or force a channel test

Stop the passive-only build if the new recovery page and repositioned hub get indexed but produce no clicks, no alert interest, and no visit lift after another review cycle.

At that point the next honest test is small paid search or a different project, not more passive waiting.

## Guardrails

- Do not add 20 pages immediately.
- Do not mass-generate plugin/version pages.
- Do not delete WooCommerce pages with existing clicks.
- Do not delete API pages yet; archive them quietly.
- Do not imply official affiliation with WooCommerce, Stripe, PayPal, Mollie, Automattic, or Shopify.
- Do not claim a vendor update caused an issue unless the source support is strong.
- Do not give irreversible payment/accounting advice; always tell users to preserve evidence and verify official gateway records.
- Do not rely on broad product news, feature hype, or generic changelog summaries.
