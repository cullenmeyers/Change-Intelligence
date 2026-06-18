# What Just Changed

Evidence-backed change records that explain what changed, who is affected, and the smallest justified action.

The product category is change intelligence. The first wedge is WordPress plugins; the broader destination is fast-changing software and vendor markets.

## Live validation site

- https://whatjustchanged.com/
- WooCommerce Stripe 10.8.x payment-status incident
- Mollie Payconiq removal
- WooCommerce PayPal Pay with Crypto default change
- WP Super Cache WordPress 6.8 requirement

The initial public validation cohort is now complete at four records. See [`VALIDATION.md`](./VALIDATION.md) for the measurement plan, review cadence, and scope lock.

## Deployment

This is a dependency-free static site deployed through Vercel from the `main` branch.

Current production setup includes:

- permanent custom domain
- absolute canonical URLs
- `mainEntityOfPage` in TechArticle schema
- production sitemap
- sitemap reference in `robots.txt`
- permanent redirect from the former Vercel production hostname
- favicon support

## Current stage

Do not add more public records yet. The next step is to enable page-level analytics, collect Search Console and referral evidence, test whether the recommendations help real users choose an action, and review the four-record cohort before expanding.
