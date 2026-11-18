# Guide page template

Copy this file to `guides/your-slug.md` when adding a guide. GitHub Pages publishes everything in `guides/` that has front matter. The home page lists a page automatically when `trade` is set. This file lives in `docs/` and is excluded from the site, so the instructions below are not published.

Write for one search: a specific trade, a specific size of company, and the products someone in that situation is comparing. No filler, no invented reviews, and no claim that we used the product unless we did. If a fact is not on a vendor's official page, leave it out or mark it **Unverified**. Pricing always carries a checked-on date and a link to the page the number came from.

```yaml
---
layout: guide
title: Product A vs Product B for a small [trade] company
description: One or two sentences a search result can show. Say who it is for and what is compared.
trade: HVAC
last_updated: YYYY-MM-DD
---
```

`title` is the H1 and the browser title. `description` is the meta description and the text on the home-page card. `trade` is the label on the card. `last_updated` is the date the page, and especially the prices, were checked. Use an ISO date.

## Intent

Say what decision the page answers, in a few sentences. Name the work week the reader is trying to run (the emergency call, the quote, the invoice, the repeat visit). Say, in the same breath, whether the page is a document comparison or a hands-on test.

## Who it's for

Say who should use the page and who should not. Be concrete about company size, who does the dispatching, and which neighboring products are out of scope.

## Quick answer

Give the fit in one short section, before the table. Name the plan, not just the brand, and the price the reader would actually pay at that size. Point at the pricing section for the date and the source. Do not save the answer for the end.

## Comparison table

One table. Rows are the jobs that matter for this trade, not a dump of every feature on the pricing page. Typical rows:

- Scheduling and dispatch
- Quotes
- Invoicing
- Payments, including the published processing rate
- Maintenance agreements or the equivalent repeat-work tool
- Accounting sync
- Mobile app

Each cell states the plan that includes the feature. If the plan is not named on the source, write that, and add the item under unverified claims.

## Per-tool notes

One subsection per product. Under each, cover only the differences that change the decision, in this order when they apply: scheduling and dispatch, quotes, invoicing, payments, maintenance agreements, accounting sync, mobile app. Describe what the vendor's docs say the tool does. Link the sentence that carries a price, a rate, or a plan gate.

## Pricing

Open with **Checked on YYYY-MM-DD** and link each vendor's pricing page.

Show the plans a company of this size would actually buy, including month-to-month and annual when both exist, what a "user" is, and what an extra user costs. Note contract terms: cancel anytime, a one-year commitment, a prepaid year. If a page shows an introductory discount, show the regular price as the number to budget, and show the discount separately with its length.

If two official numbers disagree, print both and say which page each came from.

## What to watch out for

The mistakes a buyer of this size will make: counting trucks instead of logins, signing up for the wrong industry package, comparing an annual price with a cancel-anytime price, and accounting sync that is one-way or desktop-unfriendly. State limits the docs are explicit about.

## FAQ

Four to six questions in the words an owner would search. Answer from the sections above. Do not introduce new, unsourced facts here.

## Sources

List every official page the guide relied on, grouped by vendor. Prefer pricing pages and help-center articles over blog posts and comparison pages the vendor wrote about a competitor. No affiliate parameters on the URLs.

## Claims we could not verify

A short list. Each item says what is uncertain and which two sources disagree, or that the plan tier was never named. Delete the section only when there is nothing in it. Do not fill it with guesses.
