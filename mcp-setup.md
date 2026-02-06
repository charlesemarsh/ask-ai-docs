---
layout: default
title: MCP Setup Guide
---

# MCP Setup Guide

<p class="lead">Ask AI - Data Connector uses the Model Context Protocol (MCP) to connect AI tools to your e-commerce data. Follow the guide below for your preferred AI client.</p>

## Server Details

Before configuring your client, gather the following from your app's **Integrations** page:

| Setting | Value |
|---------|-------|
| **Endpoint** | `https://your-app-url/mcp` (shown on Integrations page) |
| **Transport** | Streamable HTTP |
| **Authentication** | Bearer token via Authorization header |
| **Protocol Version** | 2024-11-05 |

<div class="callout callout-info">
Get your MCP endpoint URL and API key from <strong>Integrations > Claude</strong> in the Ask AI - Data Connector app.
</div>

---

## Claude Desktop

**macOS / Windows**

### 1. Locate your config file

- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

### 2. Add the server configuration

```json
{
  "mcpServers": {
    "ask-ai": {
      "url": "https://your-app-url/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

### 3. Restart Claude Desktop

Close and reopen Claude Desktop for the changes to take effect.

---

## Claude Code (CLI)

### Option 1: Add via command

```bash
claude mcp add --transport http ask-ai https://your-app-url/mcp \
  --header "Authorization: Bearer YOUR_API_KEY"
```

### Option 2: Edit settings file

Add to `~/.claude/settings.json`:

```json
{
  "mcpServers": {
    "ask-ai": {
      "url": "https://your-app-url/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

### 3. Verify connection

Run `/mcp` in Claude Code to check that Ask AI - Data Connector is connected.

---

## Cursor

### 1. Open Cursor Settings

Go to **Settings > Cursor Settings > Tools & MCP**.

### 2. Add the MCP server configuration

```json
{
  "mcpServers": {
    "ask-ai": {
      "url": "https://your-app-url/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

### 3. Save and restart

Save your settings and restart Cursor to apply changes.

---

## VS Code

### 1. Create the MCP config file

Create `.vscode/mcp.json` in your workspace.

### 2. Add the configuration

```json
{
  "servers": {
    "ask-ai": {
      "type": "http",
      "url": "https://your-app-url/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

### 3. Reload VS Code

Reload the window or restart VS Code for the MCP server to connect.

---

## Troubleshooting

### Connection Failed

- Verify the endpoint URL is correct (check **Integrations > Claude** page)
- Ensure your API key is valid and hasn't been revoked
- Check that `Bearer ` prefix is included before the API key in the Authorization header

### Authentication Errors (401/403)

- Regenerate your API key from the Integrations page
- Make sure you're using the `Authorization` header, not `X-API-Key`

### No Data Returned

- Ensure your Shopify data has been synced (check the Data Sources page in the app)
- Wait for the initial sync to complete after first setup

### Tools Not Showing

- Restart your AI client after configuration changes
- Check that the JSON configuration is valid (no trailing commas, correct syntax)
