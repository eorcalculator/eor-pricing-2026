# EOR pricing 2026

Published Employer of Record (EOR) prices for 11 plans from 10 providers, collected by hand from each provider's own pricing page. Checked on 2026-11-18. Maintained by [eorcalculator.com](https://eorcalculator.com).

| File | What it is |
|---|---|
| `eor_pricing_2026-11.csv` | One row per plan, cheapest first |
| `eor_pricing_2026-11.json` | Same data as JSON |

## What the data says
- The same service, one employee on an EOR, is listed from **$199 to $699 per employee per month**: up to 3.5x depending on the provider.
- Two providers publish a **required refundable deposit**: Playroll (one month of salary) and Oyster (for every EOR employee). The other nine do not publish deposit terms at all.
- The headline prices are not like for like. Of the 11 plans, **6 are "from" prices** that the country or the role can raise (RemoFirst, Skuad, Payoneer, Playroll, Papaya Global, G-P), **3 are annual-billing prices** that cost more month to month (Multiplier Core, Multiplier Growth, Remote), and only **2 publish a flat list price** (Deel at $599 and Oyster at $699). So $199 to $699 is a range between starting points, not between final bills.
- Most providers do not publish setup fees or deposit terms. "not published" means exactly that: the information is not on the public pricing page.

## Correction, 18 November 2026
An earlier version of this dataset said that the pricing pages of Oyster and Playroll were served with a `noindex`
tag and could not be indexed by search engines. We re-checked both on 18 November 2026: neither page carries a
`noindex` meta tag or an `X-Robots-Tag` header, with either a browser or a crawler user agent, and both are indexed
by Google. The claim was wrong. It has been removed and `pricing_page_indexable` is now `True` for every row.

## Fields
`eor_usd_per_employee_month` is the published EOR fee in USD. `price_basis` says whether it is a "from" price, a list price or an annual-billing price, so the figures are not always like for like. `source` is the page the figure was read from, and `checked` is the date it was read.

## Rules
- Only figures shown on the provider's public page. No quotes, no estimates.
- Rows are sorted by published price and never reordered for commercial reasons. If eorcalculator.com earns a referral fee from any provider, the site says so before its table.
- Prices are reviewed every month, and each change is logged with its date.

Corrections are welcome: open an issue with the provider's page that shows the figure.

License: CC BY 4.0. Cite as "EOR pricing 2026, eorcalculator.com".
