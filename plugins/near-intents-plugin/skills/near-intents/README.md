# near-intents plugin

Cross-chain token swaps via the NEAR Intents 1Click API.

## Install

```
/plugin marketplace add NEARBuilders/near-plugins
/plugin install near-intents@near-plugins
```

Restart Claude Code after installing.

## What It Does

This skill teaches Claude Code how to build with the 1Click API:

- React swap widgets with wagmi
- Server-side swap scripts with viem
- Chain-specific deposit transactions (EVM, Solana, NEAR, TON, Tron, Stellar)
- Status polling and error handling

## Example Prompts

```
"Build a React swap widget using NEAR Intents"
"Create a Node.js script to swap USDC to wNEAR"
"Add cross-chain bridging from Ethereum to NEAR"
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

- [1Click API Docs](https://docs.near-intents.org/near-intents/integration/distribution-channels/1click-api)
- [API Keys](https://partners.near-intents.org/)
- [OpenAPI Spec](https://1click.chaindefuser.com/docs/v0/openapi.yaml)

## Credits

Based on [near-intents-skill](https://github.com/SurgeCode/near-intents-skill) by [SurgeCode](https://github.com/SurgeCode)

> More info via [skills.sh](https://skills.sh/surgecode/near-intents-skill/near-intents)
