# NEAR Intents Plugin

Enable cross-chain token swaps via the [NEAR Intents](https://near-intents.org).

## Install

```
/plugin marketplace add NEARBuilders/near-plugins
/plugin install near-intents@near-plugins
```

Restart Claude Code after installing.

## What It Does

This skill teaches Claude Code how to build with the [1Click Swap API](https://docs.near-intents.org/near-intents/integration/distribution-channels/1click-api):

- React swap widgets with wagmi
- Server-side swap scripts with viem
- Chain-specific deposit transactions (EVM, Solana, NEAR, TON, Tron, Stellar)
- Status polling and error handling

## Example Prompts

```
Build a React swap widget using NEAR Intents
Create a cross-chain bridge from Ethereum to NEAR
Implement a token swap server using the 1Click API
```

## Integration Flow

```
GET /v0/tokens → POST /v0/quote (dry) → POST /v0/quote (wet) → Deposit TX → POST /v0/deposit/submit → GET /v0/status
```

## Skill Structure

```
skills/near-intents/
├── SKILL.md          # Entry point
├── AGENTS.md         # Full reference doc
└── rules/
    ├── api-*.md      # API endpoints
    ├── deposit-*.md  # Chain-specific deposits
    ├── react-*.md    # React patterns
    └── *.md          # Advanced topics
```

## Resources

- [NEAR Intents Docs](https://docs.near-intents.org)
- [API Keys](https://partners.near-intents.org)
- [OpenAPI Spec](https://1click.chaindefuser.com/docs/v0/openapi.yaml)

## Credits

[near-intents-skill](https://github.com/SurgeCode/near-intents-skill) by [Surge](https://x.com/surgecodes)

> More info via [skills.sh](https://skills.sh/surgecode/near-intents-skill/near-intents)
