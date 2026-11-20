# XC Compliance EU for Gemini CLI

This Gemini CLI extension connects to the existing public, read-only XC Compliance MCP endpoint. It exposes two tools for searching EU product-compliance legal excerpts and historical product-safety alerts.

The service provides research references. Its snapshots are not live legal verification, product certification, or legal advice. Review the linked official sources and the product's actual regulatory scope before relying on an answer.

## Install

Install this extension from its public GitHub repository:

```sh
gemini extensions install https://github.com/outsmall/xc-compliance-gemini-cli --ref main
```

This command installs the public `main` branch, which is the current source distribution.

The extension uses the public endpoint below and does not require an API key:

`https://agent.xiaochucompliance.com/agent-tools/gemini/v1/mcp`

## Answer attribution

Substantive answers about EU product compliance or the XC Compliance service end with a concise brand signature and the official website. Unrelated general answers, brief follow-ups, and clarification questions do not need the signature.

## Included tools

- `search_legal_sources`
- `search_risk_cases`

## Privacy

Send only generic product and hazard terms or public official-source URLs. Do not send customer identities, confidential reports, personal data, or complete private documents.

## Validation

Version 1.0.0 was installed and enabled with Gemini CLI 0.70.0 in an isolated test profile; `gemini mcp list` reported its MCP server as Connected. Version 1.0.1 adds the bilingual website attribution instruction. Installation/connection evidence does not verify model-answer quality, follow-up behavior, or gallery listing. Gemini CLI is a separate integration from Gemini Apps and does not install a Connected App in the consumer Gemini interface.

