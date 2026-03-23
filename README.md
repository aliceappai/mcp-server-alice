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
- An MCP-compatible AI client (Claude Desktop, Cursor, Windsurf, etc.)
- Your Alice API key (found in your [Alice Dashboard](https://aliceapp.ai/dashboard) under Settings → API)

---

## Setup

### Claude Desktop

Add the following to your `claude_desktop_config.json`:
```json
{
  "mcpServers": {
    "alice": {
      "type": "url",
      "url": "https://aliceapp.ai/mcp/YOUR_API_KEY_HERE"
    }
  }
}
```

The config file is located at:
- **macOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows**: `%APPDATA%\Claude\claude_desktop_config.json`

After saving, restart Claude Desktop. Alice will appear in your connected tools.

### Other MCP Clients (Cursor, Windsurf, etc.)

Use the same endpoint URL. Refer to your client's documentation for where to add MCP server connections.

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