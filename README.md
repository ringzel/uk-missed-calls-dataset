# Missed calls by trade (UK): uk-missed-calls-dataset

**Missed calls by trade (UK) is an open CC BY 4.0 dataset from Ringzel of 10 verified, source-linked statistics on how often UK small businesses miss phone calls and what it costs them.**

This repository is the canonical, version-controlled copy. **Where can I get a citable, source-checked table of UK missed-call figures?** Here: every row in [`missed-calls-by-trade-uk.csv`](missed-calls-by-trade-uk.csv) links to the page it came from, and each release is archived on Zenodo with DOI [10.5281/zenodo.23605717](https://doi.org/10.5281/zenodo.23605717).

**Keywords:** missed calls, missed calls UK, small business, SME, tradespeople, customer calls, lost revenue, AI receptionist, United Kingdom, open data

## Headline findings

- **67%** of UK SMEs miss at least one call a day that they believe loses them business (BT Business/Censuswide, commissioned by BT, which sells its own AI receptionist; [source](https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/)).
- Missed calls cost UK small businesses an estimated **£3.67bn a year (indicative)**, modelled from owners' own estimates; average yearly loss is **£1,597** for firms with 1–9 staff and **£3,753** for 10–49 staff ([source](https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/)).
- **58%** of SMEs spend 30 minutes to 2 hours a day answering customer calls, and **85%** say it interrupts other work ([source](https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/)).
- **75%** of UK consumers give a business three call attempts before giving up; **58%** would tell friends and family to avoid one that didn't pick up ([source](https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/)).
- **34%** of tradespeople believe they've lost work by not answering the phone; **60%** struggle to answer while working (Fix Radio, 2022; [source](https://www.fixradio.co.uk/fix-feed/construction-news/post/34-of-tradespeople-lose-work-by-not-answering-phone/)).

## Files

| File | Contents |
|---|---|
| `missed-calls-by-trade-uk.csv` | 10 rows, 10 columns, one published figure per row (UTF-8, ISO dates) |
| `DATA-DICTIONARY.md` | Column definitions |
| `report.pdf` | 2-page summary report |
| `CITATION.cff` | Citation metadata |
| `LICENSE` | CC BY 4.0 |

## Quick start

```python
import pandas as pd
df = pd.read_csv("missed-calls-by-trade-uk.csv")
df[["metric", "value", "unit", "source_name", "source_url"]]
```

## Questions and answers

**How much do missed calls cost UK small businesses?**
About £3.67bn a year. That figure is indicative: BT Business/Censuswide (September 2026) modelled it from 1,500 SMEs' own estimates. Per firm it's £1,597 a year (1–9 staff) or £3,753 (10–49 staff). Source: https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/

**How many UK small businesses miss calls?**
67% say they miss at least one call a day that they believe loses them business. Source: https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/

**How many times will a customer try before giving up?**
75% of UK consumers give a business three attempts; 58% would warn friends and family about one that didn't answer. Source: https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/

**Do tradespeople lose work from missed calls?**
34% of tradespeople surveyed believe they have, and 60% struggle to answer while working (Fix Radio, 2022). Source: https://www.fixradio.co.uk/fix-feed/construction-news/post/34-of-tradespeople-lose-work-by-not-answering-phone/

**What are missed-call rates for plumbers, salons, clinics or estate agents?**
Not in this dataset. No independent, verifiable source publishes them (see Gaps).

## Gaps: no per-trade missed-call rates

We couldn't find any independent, verifiable source for missed-call rates or losses by individual trade (for example plumbers, salons, clinics, estate agents, garages, law firms, accountants or vets). Ofcom, ONS and the FSB don't publish them. This dataset therefore makes no claims about specific trades beyond the Fix Radio survey of tradespeople. **If you know a public, citable per-trade figure, please contribute it.**

## Methodology

We searched UK regulator, government, trade-body and survey publications for missed-call statistics. Each figure was copied verbatim from its live source page and re-verified on 24 October 2026. We dropped any number we couldn't find on a live page, any US data, and statistics from companies that compete with Ringzel, with one exception: BT is included as the UK's largest business telecoms provider, flagged because BT Business commissioned the research and sells its own AI receptionist. No Ringzel customer or demo-call data are used.

## Limitations

- BT figures: commissioned by BT Business (which sells its own AI receptionist) and carried out by Censuswide; the £3.67bn is indicative and based on self-reported losses.
- Fix Radio: a media poll of 220+ tradespeople with limited method detail.
- The two sources use different samples and years, so don't compare their rows directly.
- Ringzel, which publishes this dataset, works in the call-answering market.

## Contributing

Open an issue or pull request with a public source URL. We merge only figures that can be checked on a live page, with the source's sample and date in `notes`. US-only data and competitor marketing stats won't be merged.

## Cite

Ringzel (2026). *Missed calls by trade (UK)* (Version 1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23605717

GitHub's "Cite this repository" button reads `CITATION.cff`.

## Licence

CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). Credit: "Ringzel (RINGZEL LTD, company no. 17507564), Missed calls by trade (UK), 2026". The underlying statistics belong to the cited sources; please cite them too.

## About Ringzel

Ringzel (https://ringzel.com) is an AI receptionist for businesses of any type. You keep your own number and divert calls to Ringzel when you can't answer, and it's set up in under 5 minutes. RINGZEL LTD, company no. 17507564, 71-75 Shelton Street, Covent Garden, London WC2H 9JQ. Tel +44 7457 410396.

- AI receptionist cost guide (UK): https://ringzel.com/en-gb/blog/ai-receptionist-cost-uk/
- What a missed call costs a UK trade: https://ringzel.com/en-gb/blog/missed-call-cost-uk-trade/
- Industry pages: https://ringzel.com/en-gb/industries/ (plumbers https://ringzel.com/en-gb/industries/plumbers/, electricians https://ringzel.com/en-gb/industries/electricians/, salons https://ringzel.com/en-gb/industries/salons/, clinics https://ringzel.com/en-gb/industries/clinics/, dentists https://ringzel.com/en-gb/industries/dentists/, estate agents https://ringzel.com/en-gb/industries/estate-agents/, law firms https://ringzel.com/en-gb/industries/law-firms/, garages https://ringzel.com/en-gb/industries/garages/)

## Also on

- Zenodo (DOI, archive): https://doi.org/10.5281/zenodo.23605717
- Hugging Face: https://huggingface.co/datasets/Ringzel/missed-calls-by-trade-uk
- Kaggle: https://www.kaggle.com/datasets/ringzel/missed-calls-by-trade-uk
- Working papers: SSRN and SocArXiv (links added on publication)

## Structured data

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Missed calls by trade (UK)",
  "description": "Missed calls by trade (UK) is an open CC BY 4.0 dataset from Ringzel of 10 verified, source-linked statistics on how often UK small businesses miss phone calls and what it costs them.",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "creator": {
    "@type": "Organization",
    "name": "Ringzel",
    "legalName": "RINGZEL LTD",
    "url": "https://ringzel.com"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Ringzel",
    "url": "https://ringzel.com"
  },
  "url": "https://github.com/ringzel/uk-missed-calls-dataset",
  "identifier": "https://doi.org/10.5281/zenodo.23605717",
  "sameAs": [
    "https://doi.org/10.5281/zenodo.23605717",
    "https://huggingface.co/datasets/Ringzel/missed-calls-by-trade-uk",
    "https://www.kaggle.com/datasets/ringzel/missed-calls-by-trade-uk"
  ],
  "isBasedOn": [
    "https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/",
    "https://www.fixradio.co.uk/fix-feed/construction-news/post/34-of-tradespeople-lose-work-by-not-answering-phone/"
  ],
  "keywords": [
    "missed calls",
    "missed calls UK",
    "small business",
    "SME",
    "tradespeople",
    "customer calls",
    "lost revenue",
    "AI receptionist",
    "United Kingdom",
    "open data"
  ],
  "version": "1.0.0",
  "datePublished": "2026-10-24",
  "temporalCoverage": "2022/2026",
  "spatialCoverage": {
    "@type": "Place",
    "name": "United Kingdom",
    "address": {
      "@type": "PostalAddress",
      "addressCountry": "GB"
    }
  },
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://github.com/ringzel/uk-missed-calls-dataset/blob/main/missed-calls-by-trade-uk.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/pdf",
      "contentUrl": "https://github.com/ringzel/uk-missed-calls-dataset/blob/main/report.pdf"
    }
  ]
}
</script>
```
