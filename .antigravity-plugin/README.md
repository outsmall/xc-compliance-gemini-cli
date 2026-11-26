# XC Compliance for Antigravity

Research EU product-compliance questions using a read-only MCP service for official legal excerpts and historical product-safety alerts.

## What it includes

- `xc-eu-compliance` skill for product-material, report-coverage, label and EU operator-duty research.
- Read-only tools `search_legal_sources` and `search_risk_cases` at the dedicated Antigravity/Gemini MCP endpoint.
- Source-linked, plain-language reference analysis.

## Limits

Evidence comes from a frozen source library and historical alerts. It is not live legal verification, product certification, legal advice or regulatory approval. Check the cited official sources and the product’s actual regulatory scope before relying on results.

## Privacy

Send only generic product and hazard terms or public official-source URLs. Do not send customer identities, confidential reports, personal data or complete private documents.

## Install

Once published, install from the Antigravity partner marketplace with:

```sh
agy plugin install xc-compliance-eu@antigravity-plugins-partners
```

The plugin can also be installed from its public GitHub repository with `agy plugin install https://github.com/outsmall/xc-compliance-gemini-cli` after the plugin files are merged there.
