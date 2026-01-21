# NEAR Plugins

Claude Code plugins for building on NEAR.

## Install

```bash
/plugin marketplace add NEARBuilders/near-plugins
/plugin install near-intents@near-plugins
```

## Plugins

### near-intents

Cross-chain token swaps via the 1Click API.

Claude automatically uses this skill when building swap widgets, bridge interfaces, or multi-chain transfers.

```
"Build a React swap widget using NEAR Intents"
"Create a cross-chain bridge from Ethereum to NEAR"
"Implement a token swap server using the 1Click API"
```

## Structure

```
near-plugins/
├── .claude-plugin/
│   └── marketplace.json
├── plugins/
│   └── near-intents-plugin/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           └── near-intents/
│               ├── SKILL.md
│               ├── AGENTS.md
│               └── rules/
│                   ├── api-*.md
│                   ├── deposit-*.md
│                   └── react-*.md
└── README.md
```

## Resources

- [NEAR Intents Docs](https://docs.near-intents.org/near-intents/integration/distribution-channels/1click-api)
- [API Keys](https://partners.near-intents.org/)
- [OpenAPI Spec](https://1click.chaindefuser.com/docs/v0/openapi.yaml)

## Credits

[`near-intents-skill`](https://github.com/SurgeCode/near-intents-skill) by SurgeCode

> more info via [skills.sh](https://skills.sh/surgecode/near-intents-skill/near-intents)
