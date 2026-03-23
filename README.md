# Alice MCP Server

Connect your Alice recordings and transcripts to the AI tools you already use — Claude, ChatGPT, Gemini, Grok, Perplexity, and any other MCP-compatible client.

The Alice MCP Server turns your secure voice archive into a queryable knowledge base. Search across hundreds of hours of recordings, retrieve full transcripts, surface insights, and automate workflows — all with natural language.

---

## What You Can Do

- **Search recordings** — find any transcript, quote, or moment using natural-language queries
- **Retrieve transcripts** — pull full transcripts or specific segments by recording ID
- **List and browse recordings** — filter by date, title, language, speaker, or metadata
- **Ask questions** — get precise answers sourced directly from your real conversations
- **Build workflows** — automate drafting, summarizing, tagging, CRM notes, and enrichment

---

## Requirements

- An Alice account — [sign up free at aliceapp.ai](https://aliceapp.ai/signup) (includes 60 free minutes)
- An MCP-compatible AI client (Claude Desktop, Claude.ai, ChatGPT, Grok, etc.)
- Your Alice connection URL (found in your [Alice Dashboard](https://aliceapp.ai/mcp) under AI → MCP Server)

---

## Setup

### Get Your Connection URL

1. Go to [aliceapp.ai/mcp](https://aliceapp.ai/mcp)
2. Click **Generate connection URL**
3. Copy the URL — you'll paste it into your AI client below

### Claude Desktop

1. Open Claude Desktop → Settings (⌘ + ,)
2. Go to **Connectors**
3. Click **Add custom connector**
4. Name: `Alice`
5. URL: Paste the URL from above
6. Click **Save**

Claude will now know to ask Alice when you have questions about your recordings.

### Claude.ai Web

1. Open Claude.ai Settings
2. Go to **Connectors**
3. Click **Add custom connector**
4. Name: `Alice`
5. URL: Paste the URL from above
6. Click **Save**

Claude will now know to ask Alice when you have questions about your recordings.

### ChatGPT

1. Open ChatGPT settings
2. Navigate to **Integrations** or **MCP Servers**
3. Click **Add Server** or **Connect**
4. Name: `Alice`
5. URL: Paste the copied URL

ChatGPT will now know to ask Alice when you have questions about your recordings.

### Grok

1. Open [grok.com](https://grok.com) or your Grok-enabled application
2. Go to **Settings → Integrations** or **MCP Tools**
3. Click **Add Remote MCP Server**
4. Name: `Alice`
5. Server URL: Paste the URL from above
6. Click **Save**

Grok will now know to ask Alice when you have questions about your recordings.

For more details, see the [Grok Remote MCP Tools Documentation](https://docs.x.ai/docs/guides/tools/remote-mcp-tools).

### Other MCP Clients (Cursor, Windsurf, etc.)

Use the same connection URL. Refer to your client's documentation for where to add MCP server connections.

### Tips

- Set permissions to **Always Allow** so your AI can reach out to Alice as needed
- Create a project named **Alice** to keep chats organized and set specific instructions

---

## Available Tools

Once connected, your AI client has access to the following tools:

| Tool | Description |
|------|-------------|
| `list_recordings` | List recordings with optional filters (date range, title, language) |
| `get_transcript` | Retrieve the full transcript for a specific recording |
| `search_recordings` | Natural-language search across recordings, transcripts, and metadata |
| `get_recording_metadata` | Get metadata for a recording (duration, speakers, language, date, location) |

---

## Example Prompts

Once Alice is connected to your AI client, try:

> *"Search my Alice recordings for everything I captured about the Johnson interview"*

> *"Get the transcript from my recording on March 15th"*

> *"Summarize the last 5 recordings tagged as sales calls"*

> *"Draft a LinkedIn post from my most recent podcast recording"*

> *"What were the key themes across all my recordings from Q1?"*

---

## Privacy & Security

Alice is built on a foundational commitment to privacy — not as a feature, but as a moral baseline.

- No data mining, no third-party trackers, no ad networks
- All data encrypted in transit and at rest
- True hard-deletion — deleted files are permanently and unrecoverably erased
- HIPAA, SOC 2, GDPR, and CCPA compliant
- Deployable in your own cloud or data center for enterprise use
- Your recordings are never used to train AI models
- You retain full ownership and intellectual property rights

---

## Supported AI Clients

| Client | Status |
|--------|--------|
| Claude Desktop | ✅ Supported |
| ChatGPT | ✅ Supported |
| Gemini | ✅ Supported |
| Grok | ✅ Supported |
| Perplexity | ✅ Supported |
| Cursor | ✅ Supported |
| Windsurf | ✅ Supported |

---

## Support

- 📧 Email: [alice@aliceapp.ai](mailto:alice@aliceapp.ai)
- 🌐 Website: [aliceapp.ai](https://aliceapp.ai)
- 📖 MCP Server page: [aliceapp.ai/mcp-server](https://aliceapp.ai/mcp-server)

---

## License

MIT License — see [LICENSE](./LICENSE) for details.