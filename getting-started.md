---
layout: default
title: Getting Started
---

# Getting Started

<p class="lead">Get up and running with Ask AI - Data Connector in a few steps.</p>

## Step 1: Install the App

Install Ask AI - Data Connector from the Shopify App Store. Once installed, your Shopify store data (orders, products, customers, and inventory) begins syncing automatically.

## Step 2: Connect Additional Data Sources (Optional)

Navigate to **Data Sources** in the app to connect third-party platforms. Each integration requires an API key from the respective platform. See the [Data Sources]({{ '/data-sources/' | relative_url }}) page for details on each provider and how to obtain API keys.

## Step 3: Set Up Your AI Client

Ask AI - Data Connector uses the Model Context Protocol (MCP) to connect AI tools to your data. You'll need to configure your AI client with your MCP endpoint and API key.

1. Go to **Integrations** in the app
2. Click **Create API Key** to generate your key
3. Copy your MCP endpoint URL and API key
4. Follow the [MCP Setup Guide]({{ '/mcp-setup/' | relative_url }}) for your specific AI client

## Step 4: Start Asking Questions

Once connected, you can ask questions about your store data in plain English. Here are some examples to get you started:

- "How's my revenue this month compared to last month?"
- "What are my top selling products?"
- "Which customers have the highest lifetime value?"
- "What's my average order value trend?"
- "Show me orders by country"

## Supported AI Clients

| Client | Type | Setup Guide |
|--------|------|-------------|
| Claude Desktop | Desktop app (macOS/Windows) | [View guide]({{ '/mcp-setup/#claude-desktop' | relative_url }}) |
| Claude Code | CLI tool | [View guide]({{ '/mcp-setup/#claude-code-cli' | relative_url }}) |
| Cursor | IDE | [View guide]({{ '/mcp-setup/#cursor' | relative_url }}) |
| VS Code | IDE | [View guide]({{ '/mcp-setup/#vs-code' | relative_url }}) |

## Need Help?

- Check the [FAQ]({{ '/faq/' | relative_url }}) for common questions
- See the [MCP Setup Guide]({{ '/mcp-setup/' | relative_url }}) for troubleshooting connection issues
- Review [Data Sources]({{ '/data-sources/' | relative_url }}) for integration-specific help
