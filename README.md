# Essentio

Invoice from a conversation with your AI assistant. This plugin pairs the Essentio connector —
Essentio's MCP server at `https://mcp.essentio.pro` — with two skills that teach the assistant the
order Essentio's work is done in.

## Skills

- **draft-and-send-invoice** — finds or creates the Client, creates a Draft, shows it as a card with
  its Client, Lines, VAT and Total, checks the figures and which Actions are open, and issues and sends
  it only when you say so. A refusal stops the workflow, and the assistant tells you what it means and
  what to do.
- **close-vat-month** — reads a month's Reported VAT and Income from Essentio's own reports, lists the
  Drafts left and the documents still awaiting payment, and says what is done and what is not. It files
  nothing with a tax authority.

## Use it

In Claude, add the plugin and connect Essentio from its Connectors tab.
Connecting Essentio's server sends you to Essentio: you sign in, choose one of your Businesses and the
Role the assistant acts with there. Then ask, for example, "Invoice ACME 500 euros for consulting
and send it" or "Close March's VAT". The skills tell the assistant to ask you before it creates a
Client, issues or sends; your assistant's own tool permissions decide whether it has to. Try it
first in a Test business: its documents are marked as samples and what it sends reaches you, never a
Client.

## Data

The plugin holds no key or password. The connector sends what you ask for — Clients, documents, their
Lines, Payments and report periods — to the Business you connected, through `mcp.essentio.pro`, and
Essentio answers from that Business's records. The plugin stores nothing itself.

## Support

Write to support@essentio.pro; we answer within two working days, Cyprus time. How to disconnect the
assistant, and where the privacy policy and terms are: https://developers.essentio.pro/support.
Developer documentation: https://developers.essentio.pro.
