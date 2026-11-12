# Microcommerce plugin

The Microcommerce connector and its skills, for working on your brand's visibility in AI answers:

- **weekly-review**: what changed since the last cycle, and what to do next.
- **triage-recommendations**: proposes a decision for each open recommendation and records only the ones you agree to.
- **reading-the-reports**: explains the reports in plain language.

You sign in with your Microcommerce admin login. MCP access must be turned on for your membership; ask your Microcommerce contact.

## Install

**Claude** (chat, desktop app, Cowork): Customize > Plugins > Add marketplace, enter `microcasting/microcommerce-plugin`, then install Microcommerce. On Team and Enterprise plans an owner adds it for the organization in the organization's plugin settings.

**Claude Code**:

```
/plugin marketplace add microcasting/microcommerce-plugin
/plugin install microcommerce@microcommerce
```

Then run `/mcp`, choose `microcommerce` and sign in.

**Codex**: `codex plugin marketplace add microcasting/microcommerce-plugin`, then open `/plugins` and install Microcommerce.

**ChatGPT** (Business, Enterprise and Edu): a workspace admin adds the plugin and publishes it to the workspace from ChatGPT Plugins; members then install it and sign in.

## Layout

This folder is both the plugin and a one-plugin marketplace.

| File | For |
|---|---|
| `.claude-plugin/plugin.json`, `.mcp.json` | Claude |
| `plugin.json`, `mcp.json` | ChatGPT and Codex |
| `.claude-plugin/marketplace.json`, `.agents/plugins/marketplace.json` | adding this repository as a marketplace |
| `skills/` | the skills, shared by all |

The source lives in the Microcommerce platform repository under `plugins/microcommerce/`; change it there.
