# Agentia MCP Server

Run Copado DevOps tasks from MCP-capable AI agents through the Agentia CLI local MCP server.

This repository is a public landing page for the official MCP Registry listing `com.copado/agentia-cli` (version 1.16.0). The Agentia CLI is closed-source and is distributed through npm as [`@copado/agentia-cli`](https://www.npmjs.com/package/@copado/agentia-cli). Documentation: <https://developer.copado.com/docs>.

## Prerequisite: store credentials

The MCP server reads the same keychain-backed credentials as the CLI. Store them once before starting the server:

```sh
npx -y @copado/agentia-cli auth set
```

No credentials are passed through MCP client configuration or environment variables.

## Start the server

```sh
npx -y @copado/agentia-cli mcp start
```

### Cursor

```json
{
  "mcpServers": {
    "agentia": {
      "command": "npx",
      "args": ["-y", "@copado/agentia-cli", "mcp", "start"]
    }
  }
}
```

### Claude Code

```sh
claude mcp add agentia -- npx -y @copado/agentia-cli mcp start
```

## Tool categories

- auth
- credential
- data
- environment
- function
- job template
- job
- pipeline
- project
- repository
- user
- work
- promotion
- metadata
- testing

## Support and security

- Issues: <https://github.com/CopadoSolutions/agentia-cli-mcp/issues>
- Security reports: see [SECURITY.md](SECURITY.md)
- License: see [LICENSE.md](LICENSE.md)
