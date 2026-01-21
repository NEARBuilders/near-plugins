# NEAR Intents Plugin

Cross-chain token swaps via the 1Click API for Claude Code.

## Install

```bash
# Local development
claude --plugin-dir ./near-intents-plugin

# From marketplace
/plugin marketplace add NEARBuilders/near-intents-plugin
/plugin install near-intents@near-plugins
```

## Usage

Claude automatically uses this skill when building swap widgets, bridge interfaces, or multi-chain transfers.

```
"Build a React swap widget using NEAR Intents"
"Create a cross-chain bridge from Ethereum to NEAR"
"Implement a token swap server using the 1Click API"
```

## Structure

```
near-intents-plugin/
├── .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── skills/
│   └── near-intents/
│       ├── SKILL.md          # Index - start here
│       ├── AGENTS.md         # Full compiled rules
│       └── rules/
│           ├── api-*.md      # API endpoints
│           ├── deposit-*.md  # Chain deposits
│           └── react-*.md    # React patterns
└── README.md
```

## Resources

- [Official Docs](https://docs.near-intents.org/near-intents/integration/distribution-channels/1click-api)
- [API Keys](https://partners.near-intents.org/)
- [OpenAPI Spec](https://1click.chaindefuser.com/docs/v0/openapi.yaml)

## Credits

`near-intents` [skill](https://github.com/SurgeCode/near-intents-skill) by SurgeCode

More info: https://skills.sh/surgecode/near-intents-skill/near-intents
