# EOR pricing 2026

Published Employer of Record (EOR) prices for 11 plans from 10 providers, collected by hand from each provider's own pricing page. Checked on 2026-11-18. Maintained by [eorcalculator.com](https://eorcalculator.com).

| File | What it is |
|---|---|
| `eor_pricing_2026-11.csv` | One row per plan, cheapest first |
| `eor_pricing_2026-11.json` | Same data as JSON |

## What the data says
- The same service, one employee on an EOR, is listed from **$199 to $699 per employee per month**: up to 3.5x depending on the provider.
- Two providers publish a **required refundable deposit**: Playroll (one month of salary) and Oyster (for every EOR employee). On both, the pricing page cannot be indexed by search engines (`noindex`).
- Most providers do not publish setup fees or deposit terms. "not published" means exactly that: the information is not on the public pricing page.

## Fields
`eor_usd_per_employee_month` is the published EOR fee in USD. `price_basis` says whether it is a "from" price, a list price or an annual-billing price, so the figures are not always like for like. `source` is the page the figure was read from, and `checked` is the date it was read.

## Rules
- Only figures shown on the provider's public page. No quotes, no estimates.
- Rows are sorted by published price and never reordered for commercial reasons. If eorcalculator.com earns a referral fee from any provider, the site says so before its table.
- Prices are reviewed every month, and each change is logged with its date.

Corrections are welcome: open an issue with the provider's page that shows the figure.

License: CC BY 4.0. Cite as "EOR pricing 2026, eorcalculator.com".
