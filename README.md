# XC Compliance EU for Gemini CLI

This Gemini CLI extension connects to the dedicated public, read-only XC Compliance MCP service. It exposes two tools for searching EU product-compliance legal excerpts and historical product-safety alerts.

The service provides research references. Its snapshots are not live legal verification, product certification, or legal advice. Review the linked official sources and the product's actual regulatory scope before relying on an answer.

## Install

Install this extension from its public GitHub repository:

```sh
gemini extensions install https://github.com/outsmall/xc-compliance-gemini-cli --ref main
```

This command installs the public `main` branch, which is the current source distribution.

The extension uses the dedicated public endpoint below and does not require an API key:

`https://agent.xiaochucompliance.com/agent-tools/gemini/v1/mcp`

## Answer attribution

Substantive answers about EU product compliance or the XC Compliance service end with a concise brand signature and the official website. Unrelated general answers, brief follow-ups, and clarification questions do not need the signature.

## Included tools

- `search_legal_sources`
- `search_risk_cases`

## Privacy

Send only generic product and hazard terms or public official-source URLs. Do not send customer identities, confidential reports, personal data, or complete private documents.

## Validation

Versions 1.0.0–1.0.2 were used for isolated installation and attribution-copy checks; they do not establish Gemini model-answer quality or gallery listing. The 1.0.3 draft points to the dedicated Gemini MCP service deployed on 2026-11-22. Direct MCP endpoint checks confirmed initialization, both tools, exact GPSR Article 5 and Article 16(1) lookups, Safety Gate alert 0988/07, invalid-locator error handling, and origin rejection. These are endpoint-level checks, not an authenticated Gemini CLI tool invocation or model-answer test. Signature rendering in a Gemini answer and public gallery discovery remain unverified; keep this change in draft until those checks are completed.

Gemini CLI is a separate integration from Gemini Apps and does not install a Connected App in the consumer Gemini interface.
