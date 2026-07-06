# Databricks Deliverables

Claude Code plugin for Databricks branded deliverables

## Prerequisites

- Claude Code v2.1.49+
- Node.js 18+, Python 3.11+ with [uv](https://docs.astral.sh/uv/)
- GitHub access to this repo (`gh auth login`)

## Installation

Via marketplace:
```bash
/plugin marketplace add stromy-org/databricks-marketplace
/plugin install databricks
```

For local development:
```bash
git clone https://github.com/stromy-org/databricks.git
cd databricks
npm install
uv sync
claude --plugin-dir .
```

## Skills

Skills are split between MCP-hosted stubs (fetched at runtime via
`ReadMcpResourceTool`) and locally-authored skills (frontmatter `_local: true`).
See `skills/README.md` for the maintenance workflow. Maintaining this plugin is
an operator task driven by the `plugin-maintain` skill in stromy-org
(`/plugin-maintain`) — it is not shipped in this plugin.

## Updating

```bash
/plugin update databricks
```

## License

See [LICENSE](LICENSE) for terms.
