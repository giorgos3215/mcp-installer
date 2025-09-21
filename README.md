# mcp-installer - A MCP Server to install MCP Servers

This server is a server that installs other MCP servers for you. Install it, and you can ask the Codex CLI to install MCP servers hosted in npm or PyPi for you. Requires `npx` and `uv` to be installed for node and Python servers respectively.

![image](https://github.com/user-attachments/assets/d082e614-b4bc-485c-a7c5-f80680348793)

### How to install:

You can register the server with the Codex CLI by running:

```bash
codex mcp add mcp-installer --command npx --args @anaisbetts/mcp-installer
```

If you prefer to edit the configuration manually, add the following to your `~/.codex/config.toml` file:

```toml
[mcp_servers."mcp-installer"]
command = "npx"
args = ["@anaisbetts/mcp-installer"]
```

### Example prompts

These are sample prompts you can issue through the Codex CLI:

> Codex, install the MCP server named mcp-server-fetch.

> Codex, install the @modelcontextprotocol/server-filesystem package as an MCP server. Use ['/Users/anibetts/Desktop'] for the arguments.

> Codex, please install the MCP server at /Users/anibetts/code/mcp-youtube; I'm too lazy to do it myself.

> Codex, install the server @modelcontextprotocol/server-github and set the environment variable GITHUB_PERSONAL_ACCESS_TOKEN to '1234567890'.
