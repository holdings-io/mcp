# Holdings — MCP server

**Software your AI can run.** Let Claude, ChatGPT, or Cursor send invoices and take payment — card or ACH. You approve every send. No monthly fee.

Tell the AI you already use who to bill and how much: it drafts the invoice, shows you a preview, and sends it the moment you confirm. Your client gets a payment link; you get paid by card or ACH, and you're told when the money lands. Quotes, clients, and recurring invoices included.

## Quick start

1. **Get a free key** — Holdings workspace → **Settings → API keys**.
2. **Add the server** to your MCP client:

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

3. **Ask your AI:** *"Send Acme the December retainer — $8,400, net 30."*

## What you can do

- **Invoices** — draft, preview, send, and track; get paid by card or ACH.
- **Quotes** — send estimates; turn accepted quotes into invoices.
- **Clients** — keep the people and businesses you bill.
- **Payments** — see what's paid and what's outstanding.

Every action is confirmable: `create_*` makes a draft, and nothing reaches a client until an explicit send. Amounts are recomputed server-side. You stay in control.

## Links
- Learn more: https://getholdings.com/invoicing
- npm: https://www.npmjs.com/package/@getholdings/mcp
- Privacy: https://getholdings.com/privacy · Terms: https://getholdings.com/terms

_Built by Holdings Financial Technologies. Payments via Stripe._
