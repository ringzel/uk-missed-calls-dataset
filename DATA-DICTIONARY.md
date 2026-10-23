# Data dictionary — missed-calls-by-trade-uk.csv

One row per published statistic. 10 rows, UTF-8, comma-separated, header row.

| Column | Type | Description |
|---|---|---|
| trade | text | Trade or sector as named by the source (e.g. "Trades (construction)"). "All SMEs" = cross-sector figure. |
| metric | text | What the number measures, worded as closely to the source as possible. |
| value | number | The figure as published. No rounding or recalculation. |
| unit | text | Unit of `value` (percent, GBP billion per year, GBP per business per year, percent of inbound calls). |
| year | integer | Year the data was collected (fieldwork or observation period). |
| geography | text | Area covered. All rows are UK. |
| source_name | text | Publisher of the page the figure was verified on. |
| source_url | URL | Page where the figure appears. Each was opened and checked on 23 Oct 2026. |
| source_date | date (YYYY-MM-DD) | Publication date shown on the source page. |
| notes | text | Sample, method and caveats, including whether the source is a vendor. |

Comparability: figures come from different methods (an SME and consumer survey, and a trades media survey) and years. Don't compare rows from different sources directly.
