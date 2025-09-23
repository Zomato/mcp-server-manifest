# Zomato MCP Server

An mcp server to expose Zomato functionalities.

## Supported Features

- 🔎 Restaurant Discovery
- 📒 Menu Browsing
- 🛒 Cart Creation
- 🥗 Food Ordering
- 💳 QR code payment

## Installation Guide

#### Install in VsCode

<b>One Click Installation</b>

[<img src="https://code.visualstudio.com/assets/images/code-stable.png" alt="Click to install" height="32" />](https://insiders.vscode.dev/redirect?url=vscode:mcp/install?%7B%22type%22%3A%22http%22%2C%22name%22%3A%22zomato-mcp%22%2C%22version%22%3A%220.0.1%22%2C%22description%22%3A%22MCP%20server%20to%20interact%20with%20Zomato%20services%22%2C%22url%22%3A%22https%3A%2F%2Fmcp-server.zomato.com%2Fmcp%22%2C%22author%22%3A%22Zomato%22%2C%22tags%22%3A%5B%22zomato-mcp%22%2C%22mcp%22%2C%22server%22%5D%2C%22categories%22%3A%5B%22mcp%22%5D%7D)

<b>Manual Installation</b>

Add this to your `mcp.json` file.

```json
{
	"servers": {
		"zomato-mcp-server": {
			"url": "https://mcp-server.zomato.com/mcp",
			"type": "http"
		}
	},
}
```

#### Install in Claude Desktop

1. Make sure Node.js is installed

In your terminal, check if Node.js is installed on your system by running:

```bash
node -v
```

If Node.js isn't installed, download it from [nodejs.org](https://nodejs.org/en).

2. Configure Claude Desktop

- Go to Settings > Developer
- Click Edit config to open the claude_desktop_config.json file
- Add the MCP server configuration to the mcpServers section
- Paste the configuration below
- Save the file to apply the configuration
- Restart Claude Desktop

<b>Configuration:</b>
```json
{
  "mcpServers": {
    "zomato-mcp": {
      "command": "npx",
      "args": [
        "mcp-remote",
        "https://mcp-server.zomato.com/mcp"
      ]
    }
  }
}
```