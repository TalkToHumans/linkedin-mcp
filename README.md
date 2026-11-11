<a href="https://www.talktohumans.app/?utm_source=github&utm_medium=readme&utm_campaign=linkedin-mcp"><img src="assets/banner.png" alt="LinkedIn MCP server by TalkToHumans: connect Claude, ChatGPT, Codex, Cursor and n8n to your LinkedIn inbox, network, leads and activity" width="100%"/></a>

# LinkedIn MCP Server

**The safest LinkedIn MCP for your Agents.** 

Connect Claude, ChatGPT, Claude Code, Codex, Cursor, VS Code or any remote MCP client to your own LinkedIn account. 

Your agent reads your LinkedIn conversations, searches your network, enriches profiles with email and phone, and drafts the messages. You review them and hit send.

[![Website](https://img.shields.io/badge/Website-talktohumans.app-blue)](https://www.talktohumans.app/?utm_source=github&utm_medium=readme&utm_campaign=linkedin-mcp)
[![Docs](https://img.shields.io/badge/Docs-MCP%20setup-green)](https://www.talktohumans.app/docs/developers/mcp)
[![MCP Registry](https://img.shields.io/badge/MCP%20Registry-io.github.TalkToHumans%2Flinkedin--mcp-purple)](https://registry.modelcontextprotocol.io/v0.1/servers?search=io.github.TalkToHumans/linkedin-mcp)
[![Transport](https://img.shields.io/badge/Transport-Streamable%20HTTP%20%2B%20OAuth-black)](#connect-your-ai-client-to-linkedin)
[![smithery badge](https://smithery.ai/badge/talktohumans/linkedin-mcp)](https://smithery.ai/servers/talktohumans/linkedin-mcp)

[![LinkedIn MCP (by TalkToHumans) MCP connector – tool definition quality and endpoint health on Glama](https://glama.ai/mcp/connectors/io.github.TalkToHumans/linkedin-mcp/badges/score.svg)](https://glama.ai/mcp/connectors/io.github.TalkToHumans/linkedin-mcp)
[![M8ven Score](https://m8ven.ai/badge/mcp/coolsapiens-linkedin-mcp-h5hxkm?v=2305abce2be77fc7cb7031625c4c95ad)](https://m8ven.ai/mcp/coolsapiens-linkedin-mcp-h5hxkm?s=readme)

```txt
https://api.talktohumans.app/mcp
```

## Why this LinkedIn MCP is safer

LinkedIn has no official MCP server, and its public API doesn't give access to your private messages. Every LinkedIn MCP is third-party, and most fall into one of three groups:

| | Open-source scrapers | Cloud LinkedIn tools | TalkToHumans |
|---|---|---|---|
| Pace | Whatever pace your agent sets | Daily caps sized for campaigns | Human pace, enforced: daily limits plus a gap between every action, per LinkedIn account. Nobody can override them |
| What 100 agent calls do | 100 trips to LinkedIn | 100 trips to LinkedIn, from their servers | Read a synced cache, so no more LinkedIn activity than one call |
| Where LinkedIn actions run | A script driving a browser on your machine | Their servers, often behind proxy IPs | The browser you already use. No cloud automation, no proxy IP |
| Where you work | In your agent's chat | In your agent's chat | Wherever suits the task: your agent's chat, the TalkToHumans app, or right inside LinkedIn and Sales Navigator |
| Who presses send | Usually the agent | The agent or a campaign | You. The MCP only drafts |

No LinkedIn tool is completely risk-free. Here is how TalkToHumans keeps the risk down:

- **Human pace, enforced.** Every action type has its own conservative daily limit and a slightly random gap between actions, so nothing goes out in bursts. Limits belong to the LinkedIn account, so every teammate and every agent shares them. Nobody can raise them, not even your agent.
- **Cache-based sync.** Your agent reads a synced copy of your LinkedIn data, not LinkedIn itself. Ask it 100 questions about your inbox and your account sees the same activity as one, with no hopping from profile to profile. The background sync that fills that copy is paced the same way.
- **Posts and searches skip your account.** Posts, comments, the people engaging with them and people searches come from a data provider, never from your LinkedIn session.
- **Runs in your browser.** LinkedIn actions go through the browser you already use. No cloud automation, no proxy IPs and no virtual browsers acting on your behalf.
- **Work in the chat, the app or LinkedIn.** Everything your agent does also lands in the TalkToHumans app and in panels embedded in LinkedIn's own pages. Check conversations, see what's scheduled and take over by hand wherever you are.
- **Drafts only.** The MCP can write a reply or stage a full follow-up sequence. Nothing goes out until you hit send.

## What your agent can do on LinkedIn

Founders, consultants, sales teams and agencies use it for the same handful of jobs:

- **Find leads in your network.** Describe your ideal customer, and your agent scores your connections. They're already connected to you, so you can message them today.
- **Find the replies you owe.** Scan hundreds of LinkedIn, Sales Navigator and Recruiter threads for the ones where someone is waiting on you, every morning if you like.
- **Draft messages in your voice.** Your agent researches each person and writes a first message that sounds like you. You review every draft and send it yourself.
- **See what gets replies.** Analyze acceptance rates, reply rates and templates, from connection request to booked meeting.
- **Stage follow-up sequences.** Follow-ups that stop when the lead replies, written for each person, waiting for you to launch them.
- **Find new leads, warmest first.** Your agent starts with the people you already talk to and those who engaged with you, then checks the news and posts on your topic, and only then searches LinkedIn by role, company or location. Or bring in a list from an event or Sales Navigator, and get a ready-to-work view.
- **Mine post comments.** Find posts on a topic or by a competitor, and import the people who commented or reacted, each with a signal saying how.
- **Score and tag contacts.** Fill an ICP score for every contact, or backfill tags on hundreds of conversations the way your team already uses them.
- **Keep your CRM in sync.** Combine it with your CRM's MCP to log LinkedIn conversations, or use the native HubSpot integration.

Your agent also gets work email and mobile phone for the people you talk to, from 20+ providers in a waterfall.

## Connect your AI client to LinkedIn

### Claude

[**Click this link to add TalkToHumans to Claude**](https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=TalkToHumans&connectorUrl=https%3A%2F%2Fapi.talktohumans.app%2Fmcp)

Click **Add**, then **Connect**, and sign in to TalkToHumans.

_On Team and Enterprise plans, only an owner can add it: [add it as an owner](https://claude.ai/admin-settings/connectors?modal=add-custom-connector&connectorName=TalkToHumans&connectorUrl=https%3A%2F%2Fapi.talktohumans.app%2Fmcp)._

_Members then click **Connect** in **Customize** > **Connectors**._

_Not showing in a chat? Click **+** > **Connectors** and turn TalkToHumans on._

<details>
<summary>Add it by hand</summary>

1. Open **Customize** > **Connectors**, click **+ Add** > **Add custom connector**
2. Name it "TalkToHumans" and paste the URL:

```text
https://api.talktohumans.app/mcp
```

3. Click **Add**, then **Connect**, and sign in to TalkToHumans

</details>

### ChatGPT

1. Open [ChatGPT plugins](https://chatgpt.com/plugins), click **+** and choose **Add custom MCP server**
2. Name it "TalkToHumans" and paste the URL:

```text
https://api.talktohumans.app/mcp
```

3. Choose **OAuth**, click **Create**, then sign in to TalkToHumans

_Custom MCP servers depend on your ChatGPT plan. On Business, Enterprise and Edu, an admin may need to allow them._

### Claude Code

In a terminal, run:

```bash
claude mcp add --transport http --scope user talktohumans https://api.talktohumans.app/mcp
```

Then run `/mcp` in Claude Code, pick `talktohumans` and choose **Authenticate**.

Already connected Claude? It shows up in Claude Code with the same account.

### Codex

In a terminal, run:

```bash
codex mcp add talktohumans --url https://api.talktohumans.app/mcp
```

If no browser opened to sign in, run:

```bash
codex mcp login talktohumans
```

The Codex app and IDE extension share this setup. In the ChatGPT desktop app, add it in **Settings** > **MCP servers**.

### Cursor

[**Click this link to add TalkToHumans to Cursor**](https://cursor.com/install-mcp?name=TalkToHumans&config=eyJ1cmwiOiJodHRwczovL2FwaS50YWxrdG9odW1hbnMuYXBwL21jcCJ9)

<details>
<summary>Add it by hand</summary>

Add this to `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "talktohumans": {
      "url": "https://api.talktohumans.app/mcp"
    }
  }
}
```

</details>

### VS Code

[**Click this link to add TalkToHumans to VS Code**](https://vscode.dev/redirect/mcp/install?name=talktohumans&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.talktohumans.app%2Fmcp%22%7D)

<details>
<summary>Add it by hand</summary>

1. Open the Command Palette and run **MCP: Add Server**
2. Choose **HTTP** and paste the URL:

```text
https://api.talktohumans.app/mcp
```

3. Name it `talktohumans`, choose **Global**, and sign in when VS Code asks

</details>

### Gemini CLI

In a terminal, run:

```bash
gemini mcp add --transport http talktohumans https://api.talktohumans.app/mcp
```

Then run `/mcp auth talktohumans` in Gemini CLI.

### Grok

1. On [grok.com](https://grok.com), open **Connectors**, then **New Connector** > **Custom**
2. Paste the URL, then sign in to TalkToHumans:

```text
https://api.talktohumans.app/mcp
```

### Perplexity

1. On [Perplexity](https://www.perplexity.ai), open **Connectors**, then **Add custom** > **Remote MCP**
2. Paste the URL, choose **OAuth** and **Streamable HTTP**:

```text
https://api.talktohumans.app/mcp
```

3. Sign in to TalkToHumans

Custom connectors need Perplexity Pro, Max or Enterprise.

### Le Chat

1. In [Le Chat connections](https://chat.mistral.ai/connections), click **Add connector**, then **Custom MCP**
2. Paste the URL, then sign in to TalkToHumans:

```text
https://api.talktohumans.app/mcp
```

### Other

Add a custom MCP server (Streamable HTTP, OAuth) with this URL, then sign in:

```text
https://api.talktohumans.app/mcp
```

## LinkedIn MCP tools

| Area | Tools |
|---|---|
| Accounts | `list_accounts`, `get_credit_balance` |
| Conversations | `list_conversations`, `list_messages`, `write_message_draft`, `upload_file` |
| Contacts | `list_contacts`, `search_people`, `import_contacts`, `get_import_progress`, `update_contact`, `delete_contacts`, `list_field_definitions`, `create_field_definition`, `list_tags`, `update_tag`, `delete_tag`, `create_signals` |
| Companies | `list_companies` |
| Content | `list_content`, `search_posts`, `find_content`, `import_content`, `import_content_engagers`, `track_content`, `update_content` |
| Enrichment | `enrich_profile`, `find_email`, `find_phone` |
| Views | `list_views`, `create_view`, `update_view`, `delete_view` |
| Templates & sequences | `list_templates`, `create_template`, `update_template`, `update_sequence`, `delete_sequence` |
| Reporting | `list_activity`, `get_activity_summary` |
| Skills | `load_skill` |
| Feedback | `send_feedback` |

`write_message_draft` saves a draft, a sequence or a connection request for you to review, or clears one. It never sends. Imports, searches, enrichment and tracking use TalkToHumans credits. `list_accounts` also gives your agent your own LinkedIn profile, for free, so it knows who you are.

## FAQ

### What is a LinkedIn MCP server?

MCP (Model Context Protocol) is the open standard that lets AI assistants like Claude, ChatGPT and Cursor use outside tools. A LinkedIn MCP server connects your agent to your LinkedIn data. It can read your conversations, search your network and prepare messages, instead of you copying everything into a chat.

### Is there an official LinkedIn MCP?

No. LinkedIn doesn't offer an MCP server, and its public API doesn't cover private messages. Every LinkedIn MCP is third-party.

### Can my agent send LinkedIn messages on its own?

No, and that's on purpose. Your agent can read, sort and draft, down to a full follow-up sequence. Every message that carries your name still gets your approval.

### Do I have to give you my LinkedIn password?

No. TalkToHumans works through your logged-in browser session. Your AI client signs in to TalkToHumans, not to LinkedIn.

### How fresh is the data?

Your workspace syncs while your browser is open with the TalkToHumans extension on, newest conversations first. Older message history loads when you open a conversation in TalkToHumans.

### Is there a LinkedIn CLI?

Yes. The [LinkedIn CLI](https://github.com/TalkToHumans/linkedin-cli) (`tth`) is the same workspace from the terminal, for Claude Code, Codex, scripts and cron jobs. It only drafts too. See the [CLI docs](https://www.talktohumans.app/docs/developers/cli).

### Is there a LinkedIn API too?

Yes. Every paid plan also includes a REST API for contacts, companies, conversations, content, drafts, views and activity. See the [developer docs](https://www.talktohumans.app/docs/developers/overview).

### Which plan includes the MCP?

MCP, CLI and API access come with every paid plan, from [Starter](https://www.talktohumans.app/pricing?utm_source=github&utm_medium=readme&utm_campaign=linkedin-mcp). Pro adds sequences, post engagers, analytics and CRM integrations.

## About this repository

This repo holds the [MCP Registry](https://registry.modelcontextprotocol.io/) entry (`server.json`) and setup docs for the hosted TalkToHumans server. The server runs at `https://api.talktohumans.app/mcp`, and its code isn't in this repo.

Found a bug or a missing tool? [Open an issue](https://github.com/TalkToHumans/linkedin-mcp/issues).

---

Built by [TalkToHumans](https://www.talktohumans.app/?utm_source=github&utm_medium=readme&utm_campaign=linkedin-mcp).
