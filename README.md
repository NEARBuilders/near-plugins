# NEAR Plugins

Claude Code plugins for building on NEAR.

## Quick Start

```
/plugin marketplace add NEARBuilders/near-plugins
/plugin install near-intents@near-plugins
```

Then restart Claude Code.

### Example Prompts (NEAR Intents Plugin)

```
Build a React swap widget using NEAR Intents
Create a cross-chain bridge from Ethereum to NEAR
Implement a token swap server using the 1Click API
```

## Available Plugins

| Plugin                                        | Description                      | Install                                     |
| --------------------------------------------- | -------------------------------- | ------------------------------------------- |
| [near-intents](./plugins/near-intents-plugin) | Cross-chain swaps via 1Click API | `/plugin install near-intents@near-plugins` |

### Soon

- `near-ai` — NEAR AI Cloud
- `near-social` — Graph Database
- `near-kit` — Developer Tools

Other ideas? Create an issue [here](https://github.com/NEARBuilders/near-plugins/issues) to request a plugin.

## Contributing

To add a plugin:

1. Fork or clone this repo: https://github.com/NEARBuilders/near-plugins.git
2. Create `plugins/your-plugin/` with `.claude-plugin/plugin.json`
3. Add skills in `plugins/your-plugin/skills/`
4. Add entry to `.claude-plugin/marketplace.json`
5. Submit pull request

## Resources

- [NEAR Protocol Docs](https://docs.near.org)
- [Claude Code Plugins](https://docs.anthropic.com/claude-code/plugins)
