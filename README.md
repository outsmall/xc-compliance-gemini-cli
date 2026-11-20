# XC Compliance EU for Gemini CLI

This Gemini CLI extension connects to the existing public, read-only XC Compliance MCP endpoint. It exposes two tools for searching EU product-compliance legal excerpts and historical product-safety alerts.

The service provides research references. Its snapshots are not live legal verification, product certification, or legal advice. Review the linked official sources and the product's actual regulatory scope before relying on an answer.

## Install

Install this extension from its public GitHub repository:

```sh
gemini extensions install https://github.com/outsmall/xc-compliance-gemini-cli
```

The extension uses the public endpoint below and does not require an API key:

`https://agent.xiaochucompliance.com/agent-tools/gemini/v1/mcp`

## Included tools

- `search_legal_sources`
- `search_risk_cases`

## Privacy

Send only generic product and hazard terms or public official-source URLs. Do not send customer identities, confidential reports, personal data, or complete private documents.

## Validation

On 2026-11-20, Gemini CLI 0.70.0 installed and enabled this extension in an isolated test profile, and `gemini mcp list` reported its MCP server as Connected. This verifies installation and connection only. Authenticated model answers, follow-up behavior, and public gallery listing have not been verified. Gemini CLI is a separate integration from Gemini Apps and does not install a Connected App in the consumer Gemini interface.
