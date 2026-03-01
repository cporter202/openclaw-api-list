# OpenClaw API List — Focus & Criteria

This repository curates **APIs that are productive for tying into [OpenClaw](https://openclaw.ai)** — the open-source, local-first personal AI assistant that runs on your own devices and connects to WhatsApp, Telegram, Slack, Discord, and more.

---

## What is OpenClaw?

- **Multi-channel** — One assistant across WhatsApp, Telegram, Slack, Discord, Google Chat, Signal, iMessage, Microsoft Teams, Matrix, WebChat, etc.
- **Agentic** — It can *do* things: run shell commands, use the browser, manage files, run cron jobs, call webhooks, and use skills/tools.
- **Skills** — Capabilities are added via **skills** (AgentSkills-compatible): a folder with `SKILL.md` that teaches the agent when and how to call tools. Skills can use API keys via `skills.entries.<name>.apiKey` or env vars.
- **Tools** — Built-in: browser, canvas, nodes, cron, webhooks, sessions. Custom APIs are typically exposed via **skills** (HTTP/API calls from a skill’s tool) or **MCP**.
- **ClawHub** — Public skill registry; install skills with `clawhub install` / `clawhub sync`.

**Productive APIs** = APIs the OpenClaw agent can actually call to *do* something: search, book, send, fetch, analyze, automate — via **skills**, **webhooks**, or **MCP**.

---

## Inclusion Criteria

An API belongs in this list if it is **useful for an OpenClaw assistant** and at least one of:

1. **Callable by a skill** — REST/HTTP API (or Apify-style run) that a skill can invoke with an API key or token.
2. **MCP-compatible** — MCP servers that OpenClaw (or its ecosystem) can connect to.
3. **Webhook-friendly** — Can trigger or be triggered by OpenClaw’s webhook/cron automation.
4. **Integration-ready** — Calendar, email, messaging, storage, search, or productivity APIs the assistant can use on behalf of the user.

We **exclude** or deprioritize:

- APIs that are not agent-callable (e.g. SDK-only, no HTTP/API surface).
- APIs that are purely for human-only dashboards with no automation/API use case.
- Duplicate entries (e.g. "Rental" variants) unless they offer a distinct integration path.

---

## Category Relevance for OpenClaw

| Category | Relevance | How it ties in |
|----------|-----------|-----------------|
| **MCP Servers** | ⭐⭐⭐ Direct | MCP is a first-class integration path for OpenClaw; these are ready to connect. |
| **Automation** | ⭐⭐⭐ High | Workflows, triggers, webhooks; the agent can start or react to automations. |
| **Integrations** | ⭐⭐⭐ High | Calendar, email, messaging, storage — natural “do this for me” APIs for skills. |
| **AI** | ⭐⭐⭐ High | Models/agents the assistant can call; API keys go in `skills.entries.*.apiKey`. |
| **Agents** | ⭐⭐ Medium–High | Agent-to-agent or task APIs; wrap as skills for research, content, jobs, etc. |
| **Travel** | ⭐⭐ Medium | Book, search, compare — ideal for “plan my trip” / “find accommodation” skills. |
| **Jobs** | ⭐⭐ Medium | Job search, applications, alerts — useful for “find jobs” / “apply” skills. |
| **News** | ⭐⭐ Medium | Headlines, summaries, feeds — “what’s the news” / digest skills. |
| **Ecommerce** | ⭐⭐ Medium | Price checks, product search, reviews — “find product” / “compare prices” skills. |
| **Lead Generation** | ⭐⭐ Medium | Contacts, outreach; use with care via skills (privacy/compliance). |
| **Social Media** | ⭐⭐ Medium | Post, analyze, monitor — skills for “post to X” / “summarize engagement”. |
| **Real Estate** | ⭐⭐ Medium | Listings, market data — “find properties” skills. |
| **SEO Tools** | ⭐⭐ Medium | Keywords, rankings — “SEO report” / “keyword ideas” skills. |
| **Videos** | ⭐⭐ Medium | Transcripts, search, metadata — “summarize video” / “find clip” skills. |
| **Developer Tools** | ⭐ Low–Medium | Include only scriptable/HTTP-callable tools useful for an assistant (e.g. deploy, docs). |
| **Open Source** | ⭐ Low–Medium | Same as developer tools; prefer APIs that expose clear “do X” actions. |
| **Business** | ⭐ Low | Keep if they expose automation/API use cases. |
| **Other** | ⭐ Low | Audit case-by-case; keep only those that clearly support skills/webhooks/MCP. |

---

## How to Use This List with OpenClaw

1. **Pick an API** from a category that fits your use case (e.g. [MCP Servers](./mcp-servers-apis-131/), [Integrations](./integrations-apis-890/), [Automation](./automation-apis-4825/)).
2. **Create a skill** — In `~/.openclaw/workspace/skills/` or `~/.openclaw/skills/`, add a folder with a `SKILL.md` that:
   - Describes when the agent should use the API.
   - Declares `metadata.openclaw.primaryEnv` (or `requires.env`) for the API key.
   - Instructs the agent to call your tool (e.g. HTTP request to the API).
3. **Configure the key** — In `~/.openclaw/openclaw.json`, under `skills.entries.<skillName>`, set `apiKey` or `env` so the key is injected at runtime.
4. **Optional: Publish to ClawHub** — Share your skill so others can `clawhub install <skill>`.

For **MCP servers**, use OpenClaw’s MCP integration to attach the server; no skill is required for basic tool exposure.

---

## Links

- [OpenClaw](https://openclaw.ai) · [Docs](https://docs.openclaw.ai) · [Skills](https://docs.openclaw.ai/tools/skills) · [ClawHub](https://clawhub.com)
