# Change Intelligence

Evidence-backed change records that explain what changed, who is affected, and the smallest justified action.

The first wedge is WordPress plugins. The broader destination is change intelligence across fast-changing software and vendor markets.

## Current validation page

- WooCommerce Stripe 10.8.x payment-status incident

## Deployment

This is a dependency-free static site. Import the repository into Vercel with the framework preset set to **Other**.

After Vercel provides the production URL or a custom domain is connected:

1. Add an absolute canonical URL to the decision page.
2. Add the production URL to the `mainEntityOfPage` field in its TechArticle schema.
3. Create `sitemap.xml` using the production domain.
4. Add the sitemap URL to `robots.txt`.

Do not expand the site until the first page is live, indexed, and tested for impressions and useful referrals.
