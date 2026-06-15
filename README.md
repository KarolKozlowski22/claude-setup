# claude-setup

My Claude Code MCP servers configuration.

## MCP Servers

### GitHub MCP Server

Enables Claude Code to interact with GitHub — create PRs, manage issues, read repos, etc.

**Requirements:**
- Docker

**Setup:**

1. Copy `settings.json` to `~/.claude/settings.json`
2. Replace `YOUR_GITHUB_PAT_HERE` with a [GitHub fine-grained personal access token](https://github.com/settings/tokens?type=beta)

**Required token permissions:**
- `Contents` — Read & Write
- `Issues` — Read & Write
- `Pull requests` — Read & Write
- `Discussions` — Read & Write
- `Metadata` — Read (mandatory)

3. Restart Claude Code — the GitHub MCP server will be available automatically.
