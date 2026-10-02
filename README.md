# BIOS

BIOS is the workspace where an e-commerce founder's AI team does real work inside approvals. This plugin
brings your BIOS company into Claude, ChatGPT and Codex: your store's numbers, what your team is waiting for
you to approve, and a way to ask your team for work. Approving, sending and spending stay in the BIOS app.

## What it includes

- **The BIOS connector** (`https://api.usebios.com/mcp`), a remote MCP server run by Helion. You sign in with
  your BIOS email and password and choose Allow (OAuth 2.1 with PKCE). It has four tools:

  | Tool | What it does | Who can use it |
  |---|---|---|
  | Business snapshot | Revenue, orders, average order and Meta ad spend for today, 7 or 30 days, from BIOS Reports | Anyone in the company |
  | Waiting for your yes | What your BIOS team has proposed and is waiting for you to approve | Anyone in the company |
  | Ask BIOS | A plain question about your numbers, answered from BIOS Reports | Managers and owners |
  | Ask the team for work | Sends a request to your BIOS executive assistant | Managers and owners |

- **Two skills:** `weekly-business-review` (a short review of the last 7 days, then what waits for your yes) and
  `plan-a-campaign` (shape a campaign with your real numbers, then hand it to your team).

## What it sends and fetches

The plugin runs no code on your computer. Claude talks only to `https://api.usebios.com/mcp`, sending the
questions and requests you make with these tools, and receives your company's numbers and approval queue
from BIOS. BIOS never estimates a number it cannot read from your store; it says the number is unavailable.
Nothing is sent to customers, published or changed in your store from Claude. When you ask the team for
work, it plans the work in BIOS using the AI subscriptions connected there, and any send, publish or spend it
proposes waits for your yes in the BIOS app.

## Requirements

A BIOS account (usebios.com), with AI data sharing agreed by an owner of your company in the BIOS app.
Connect Shopify (and Meta for ad spend) in BIOS for real numbers.

Help: https://usebios.com/support · Privacy: https://usebios.com/privacy · Terms: https://usebios.com/terms

The same folder is also an OpenAI plugin package (`plugin.json` and `mcp.json` at the root, Agent Plugins
1.0.0); `.claude-plugin/plugin.json` and `.mcp.json` are the Claude plugin manifest and server config.
