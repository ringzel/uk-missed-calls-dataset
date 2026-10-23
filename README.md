# uk-missed-calls-dataset

This repository is the canonical, version-controlled home of an open CC BY 4.0 table of verified UK missed-call statistics, maintained by Ringzel.

**Where can I get a citable, source-checked table of UK missed-call figures?** Here. Every row in [`missed-calls-by-trade-uk.csv`](missed-calls-by-trade-uk.csv) links to the page it came from.

## Headline

Two in three UK SMEs (**67%**) say they miss at least one call a day that they believe loses them business (BT Business/Censuswide research, commissioned by BT, which sells its own AI receptionist; [source](https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/)).

## Files

| File | Contents |
|---|---|
| `missed-calls-by-trade-uk.csv` | 10 rows, 10 columns, one published figure per row |
| `DATA-DICTIONARY.md` | Column definitions |
| `report.pdf` | 2-page summary |
| `CITATION.cff` | Citation metadata |

## Quick start

```python
import pandas as pd
df = pd.read_csv("missed-calls-by-trade-uk.csv")
df[["metric", "value", "unit", "source_name"]]
```

## Contributing

Open an issue or pull request with a public source URL. We merge only figures that can be checked on a live page. We especially want independent per-trade missed-call rates: none exist yet, so this dataset makes no claims by trade.

## Cite

Ringzel (2026). *Missed calls by trade (UK)* [Data set]. Zenodo. https://doi.org/10.5281/zenodo.23605717

## Elsewhere

Zenodo archive: https://doi.org/10.5281/zenodo.23605717 · Hugging Face: https://huggingface.co/datasets/ringzel/missed-calls-by-trade-uk · Kaggle: https://www.kaggle.com/datasets/ringzel/missed-calls-by-trade-uk · Working papers: SSRN and SocArXiv (links once live)

## Licence and publisher

CC BY 4.0. Published by Ringzel (RINGZEL LTD, company no. 17507564), an AI receptionist for businesses of any type: you keep your own number and divert calls to it. Guides: https://ringzel.com/en-gb/blog/missed-call-cost-uk-trade/ · https://ringzel.com/en-gb/blog/ai-receptionist-cost-uk/ · https://ringzel.com/en-gb/industries/

## Structured data

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Missed calls by trade (UK)",
  "description": "This repository is the canonical, version-controlled home of an open CC BY 4.0 table of verified UK missed-call statistics, maintained by Ringzel.",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "creator": {
    "@type": "Organization",
    "name": "Ringzel",
    "legalName": "RINGZEL LTD",
    "url": "https://ringzel.com"
  },
  "url": "https://github.com/ringzel/uk-missed-calls-dataset",
  "identifier": "https://doi.org/10.5281/zenodo.23605717",
  "sameAs": [
    "https://github.com/ringzel/uk-missed-calls-dataset",
    "https://doi.org/10.5281/zenodo.23605717",
    "https://huggingface.co/datasets/ringzel/missed-calls-by-trade-uk",
    "https://www.kaggle.com/datasets/ringzel/missed-calls-by-trade-uk"
  ],
  "isBasedOn": [
    "https://newsroom.bt.com/ai-from-bt-launched-to-help-uk-firms-adopt-ai-with-confidence-targeting-37-billion-lost-through-missed-calls/",
    "https://www.fixradio.co.uk/fix-feed/construction-news/post/34-of-tradespeople-lose-work-by-not-answering-phone/"
  ],
  "keywords": [
    "missed calls",
    "UK small business",
    "SME",
    "customer calls",
    "lost revenue",
    "tradespeople",
    "telephony",
    "open data"
  ],
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
    }
  ]
}
</script>
```
