# Zomato MCP Server

An mcp server for your food ordering needs.

Disclaimer : This is only for testing purposes and Zomato disclaims any and all liabilities that may arise due to erroneous / non-functionality of the MCP integration.

## Supported Features

- 🔎 **Restaurant Discovery** - Find nearby restaurants based on your location and preferences.
- 📒 **Menu Browsing** - Browse through detailed menus with prices, descriptions, and ratings.
- 🛒 **Cart Creation** - Add items to your cart and customize orders with ease.
- 🥗 **Food Ordering** - Place orders seamlessly with order tracking support.
- 💳 **QR code payment** - Complete secure payments using QR code integration.

## Installation Guide

> ⚠️ **OAuth Redirect URI Warning**: Currently, we have only whitelisted the following redirect URIs for OAuth authentication. Please reach out to us to enable your client:
> - `claude://claude.ai/settings/connectors`
> - `https://chatgpt.com/connector_platform_oauth_redirect`
> - `https://claude.ai/api/mcp/auth_callback`
> - `https://insiders.vscode.dev/redirect`
> - `https://oauth.pstmn.io/v1/callback`
> - `https://vscode.dev/redirect`

### Install in VsCode

<b>One Click Installation</b>

[<img src="https://code.visualstudio.com/assets/apple-touch-icon.png" alt="Install in VS Code" height="32" />](https://insiders.vscode.dev/redirect?url=vscode:mcp/install?%7B%22type%22%3A%22http%22%2C%22name%22%3A%22zomato-mcp%22%2C%22version%22%3A%220.0.1%22%2C%22description%22%3A%22MCP%20server%20to%20interact%20with%20Zomato%20services%22%2C%22url%22%3A%22https%3A%2F%2Fmcp-server.zomato.com%2Fmcp%22%2C%22author%22%3A%22Zomato%22%2C%22tags%22%3A%5B%22zomato-mcp%22%2C%22mcp%22%2C%22server%22%5D%2C%22categories%22%3A%5B%22mcp%22%5D%7D)

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

<b>Disclaimer</b>
We are not allowing any third party apps to be built right now due to security and legal consideration, please watch out the space due to this
