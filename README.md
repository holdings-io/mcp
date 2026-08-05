# Holdings — MCP server

[![smithery badge](https://smithery.ai/badge/holdings/invoicing)](https://smithery.ai/servers/holdings/invoicing)

**Software your AI can run.** Let Claude, ChatGPT, or Cursor send invoices and take payment — card or ACH. You approve every send. No monthly fee.

Tell the AI you already use who to bill and how much: it drafts the invoice, shows you a preview, and sends it the moment you confirm. Your client gets a payment link; you get paid by card or ACH, and you're told when the money lands. Quotes, clients, and recurring invoices included.

## Get a key

Create a free key in your Holdings workspace → **Settings → API keys**. No monthly fee.

## Connect

Pick whichever fits your client. All three use the same free key.

### 1. Local (npm / stdio) — Claude Desktop, Cursor, Cline, Windsurf

```json
{
  "mcpServers": {
    "holdings": {
      "command": "npx",
      "args": ["-y", "@getholdings/mcp"],
      "env": { "HOLDINGS_API_KEY": "hw_live_your_key_here" }
    }
  }
}
```

### 2. Hosted (remote / Streamable HTTP) — any client that supports remote MCP

```
https://mcp.getholdings.com/mcp
```

Authenticate with either an `Authorization: Bearer <your key>` header or a `?mcpKey=<your key>` query parameter. Nothing to install.

### 3. Smithery

One-click via the registry: **[smithery.ai/servers/holdings/invoicing](https://smithery.ai/servers/holdings/invoicing)** — paste your key when prompted.

Then just ask your AI: *"Send Acme the December retainer — $8,400, net 30."*

## What you can do

- **Invoices** — draft, preview, send, and track; get paid by card or ACH.
- **Quotes** — send estimates; turn accepted quotes into invoices.
- **Clients** — keep the people and businesses you bill.
- **Payments** — see what's paid and what's outstanding.

Every action is confirmable: a draft is created first, and nothing reaches a client until an explicit send. Amounts are recomputed server-side. You stay in control.

## Links

- Learn more: https://getholdings.com/invoicing
- npm: https://www.npmjs.com/package/@getholdings/mcp
- Registry: https://registry.modelcontextprotocol.io (`com.getholdings/mcp`)
- Privacy: https://getholdings.com/privacy · Terms: https://getholdings.com/terms

_Built by Holdings Financial Technologies. Payments via Stripe._
