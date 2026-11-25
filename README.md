# SaaSFrame for agents: plugin

Design from real SaaS references. This plugin connects your AI tool to the [SaaSFrame](https://www.saasframe.io) MCP: 2,000+ real SaaS website pages, product screens, user flows and isolated sections, with the fonts, sizes, colors and radii measured on each page.

- **MCP server**: `https://www.saasframe.io/api/mcp/pro` (streamable HTTP, OAuth sign-in with your SaaSFrame account)
- **Skill**: `design-from-references`, the method to go from references to a built screen
- **Requires**: a SaaSFrame Pro or Team plan ([pricing](https://www.saasframe.io/pricing))

## Install

**Claude Code**

```
claude mcp add --transport http saasframe https://www.saasframe.io/api/mcp/pro
```

**Claude (web and desktop)**: Settings → Connectors → Add custom connector → `https://www.saasframe.io/api/mcp/pro`

**Cursor**: add to `.cursor/mcp.json`

```json
{ "mcpServers": { "saasframe": { "url": "https://www.saasframe.io/api/mcp/pro" } } }
```

**ChatGPT, Codex, VS Code**: add a remote MCP server with the same URL. Sign-in opens in your browser.

## What you can ask

- "Show me pricing pages with a monthly and yearly toggle."
- "How do SaaS products onboard a new user? Show me a flow step by step."
- "I'm designing a settings page. What should I decide first?"
- "List the sections of https://linear.app and give me its hero as Tailwind code."

## Tools

`design_guide`, `search_screens`, `get_screen`, `search_sections`, `get_section`, `search_flows`, `get_saas`, `list_categories`, `list_patterns`, `list_collections`, `get_collection`, `get_clip`, `save_to_collection`, `inspect_url`, `export_section`, `remix`, `list_inspector_exports`, `get_inspector_export`.

All tools read data, except `save_to_collection`, which saves a page to your own SaaSFrame collections.

## Links

- Documentation: https://www.saasframe.io/agents/mcp
- Privacy policy: https://www.saasframe.io/privacy
- Terms: https://www.saasframe.io/terms
- Support: https://www.saasframe.io/contact

## License

MIT, for the files in this repository. The SaaSFrame library and service are covered by the [terms](https://www.saasframe.io/terms).
