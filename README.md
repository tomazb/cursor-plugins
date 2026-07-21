# Tomazb Cursor plugins

My own Cursor plugin marketplace: developer tools, framework rules, MCP integrations, and agent skills. Each plugin is a standalone directory at the repository root with its own `.cursor-plugin/plugin.json` manifest.

## Plugins

| `name` | Plugin | Author | Category | `description` (from marketplace) |
|:-------|:-------|:-------|:---------|:-------------------------------------|
| `cursor-rubber-duck` | [Rubber Duck](cursor-rubber-duck/) | Tomazb | Developer Tools | Constructive second-opinion critic for plans, code, and tests on a contrasting model — Blocking / Non-blocking / Suggestions, read-only, with /rubber-duck. |

## Repository structure

This is a multi-plugin marketplace repository. The root `.cursor-plugin/marketplace.json` lists all plugins, and each plugin has its own manifest:

```
cursor-plugins/
├── .cursor-plugin/
│   └── marketplace.json       # Marketplace manifest (lists all plugins)
├── plugin-name/
│   ├── .cursor-plugin/
│   │   └── plugin.json        # Per-plugin manifest
│   ├── skills/                # Agent skills (SKILL.md with frontmatter)
│   ├── rules/                 # Cursor rules (.mdc files)
│   ├── agents/                # Custom agents
│   ├── commands/              # Slash commands
│   ├── mcp.json               # MCP server definitions (optional)
│   ├── README.md
│   ├── CHANGELOG.md
│   └── LICENSE
└── ...
```

## License

MIT (see each plugin directory for its license).
