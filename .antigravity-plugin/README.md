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

## Windows quick start

Antigravity CLI (`agy`) is separate from Gemini CLI. In Windows PowerShell, launch Antigravity CLI with:

```powershell
& "$env:LOCALAPPDATA\agy\bin\agy.exe"
```

Complete the Google sign-in flow opened by Antigravity. Antigravity App and CLI share the local sign-in session. The path above is the standard per-user install path; if it is missing, install the CLI using Google's official instructions.

## Install

After this plugin has been published to the Antigravity partner marketplace, install it with:

```powershell
& "$env:LOCALAPPDATA\agy\bin\agy.exe" plugin install xc-compliance-eu@antigravity-plugins-partners
```

After the plugin files are merged into the public repository, it can also be installed from GitHub:

```powershell
& "$env:LOCALAPPDATA\agy\bin\agy.exe" plugin install https://github.com/outsmall/xc-compliance-gemini-cli
```
