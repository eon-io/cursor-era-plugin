# Era Cursor Plugin

Connect Cursor to [Era](https://console.era.eon.io) via this plugin. Bundles the Era MCP server so an agent can sign in, provision a synthetic design partner, and manage its connector fleet.

## Capabilities

- **Era MCP server** — sign in (or complete OAuth), list the connectors a design partner can be built across, provision one, add systems to it, watch its build, rotate or scope its tokens, check usage, and remove it — all as MCP tools.

This plugin currently ships the MCP server only. Guided skills are not included yet.

## Installation

Copy the plugin into Cursor's local plugin directory and reload Cursor:

```bash
mkdir -p ~/.cursor/plugins/local
cp -R . ~/.cursor/plugins/local/era
```

## MCP Server

The plugin connects to `https://console.era.eon.io/mcp` via HTTP. Authentication is handled by Era's own sign-in flow.

## Local Development

Copy the plugin to Cursor's local plugin directory, then run `/reload-plugins` inside Cursor after making local edits.

## Links

- [Era](https://console.era.eon.io)
- [Eon](https://eon.io)

## License

Licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE) for details. Use of the Era service and API is governed separately by the Era by Eon design partner program terms of service.
