# Initial Site Validation

## Scope lock

The initial public validation set is complete at four decision records:

1. WooCommerce Stripe 10.8.x payment status not updating
2. Mollie Payconiq removal
3. WooCommerce PayPal Pay with Crypto enabled by default
4. WP Super Cache requiring WordPress 6.8

Do not add more public records until the first validation review. New changes may be researched and queued privately, but the public site stays at four records so results are attributable to a small, deliberate cohort rather than volume.

## Validation start

- Start date: June 18, 2026
- First review: 7 days after Web Analytics is enabled
- Second review: 14 days after Web Analytics is enabled
- Main decision review: 30 days after Web Analytics is enabled

## What to measure

### 1. Indexing

For each record, capture:

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

Examples of useful intent include questions about whether to update, migrate, disable, reconcile, or change configuration.

### 3. Visits and referrals

From Vercel Web Analytics, capture by page:

- visitors
- views
- referrer/source
- country only when useful for interpreting a region-specific change

The purpose is to distinguish Google discovery from direct links, support-thread referrals, and manual sharing.

### 4. Recommendation usefulness

For each record, ask at least one relevant WordPress user, developer, agency operator, or store owner:

- Can you identify whether the record applies to you?
- Is the recommended action clear?
- Is the safeguard specific enough to act on?
- What information is still missing before you would follow it?

Record the answer, not just a yes/no score.

### 5. Freshness

Recheck source evidence when the underlying change is still active:

- Stripe incident: recheck official releases and support status when a new release appears
- Mollie Payconiq: recheck if Payconiq is restored, replaced, or addressed in a later release
- PayPal Pay with Crypto: recheck when eligibility, defaults, or documentation changes
- WP Super Cache: recheck when requirements or the current release change

## Decision rules

### Continue and expand carefully

Continue when the pages are indexed and at least some records show relevant non-branded impressions, useful referrals, or clear user-action value. Add the next record only after identifying which page pattern produced the strongest signal.

### Refine before expanding

Refine when pages are indexed but the queries or referrals do not match the intended decision. Change the angle, title, summary, or decision framing before adding volume.

### Investigate distribution or technical problems

Investigate when pages are not indexed, Google selects a different canonical, analytics receives no real visits after distribution, or users cannot tell what action to take.

## Prohibited during the initial validation window

- Do not expand to 10–25 public pages.
- Do not redesign the site.
- Do not add broad comparison or affiliate content.
- Do not repeatedly request indexing every day.
- Do not change several variables at once.
- Do not judge the market from raw traffic alone; query intent and action usefulness matter more at this stage.
