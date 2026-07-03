# 🦞 OpenClaw — Start Here (Curated List)

**~100 APIs** that are the best fit for OpenClaw. Use this list first; only browse the [full list](./README.md#-table-of-contents) when you need something specific.

---

## How to use

1. Pick an API below (MCP = plug in directly; others = wrap as a [skill](https://docs.openclaw.ai/tools/skills)).
2. Add your API key in `~/.openclaw/openclaw.json` under `skills.entries.<name>` if the API needs one.
3. For **MCP** servers, use OpenClaw’s MCP integration — no skill required for basic tools.

---

## MCP servers (plug in directly)

| API | What it does | OpenClaw use |
|-----|--------------|--------------|
| [Brave Search MCP Server](https://apify.com/agentify/brave-search-mcp-server?fpr=p2hrc6) | Private search via Brave | Web search from the assistant |
| [Google Search MCP Server](https://apify.com/datascoutapi/google-search-mcp-server?fpr=p2hrc6) | Real-time Google SERPs | Search from the assistant |
| [Tavily MCP Server](https://apify.com/agentify/tavily-mcp-server?fpr=p2hrc6) | Web search + extraction via Tavily | Research, citations |
| [Exa MCP Server](https://apify.com/agentify/exa-mcp-server?fpr=p2hrc6) | Semantic search (mcp.exa.ai) | Deep search for the assistant |
| [Firecrawl MCP Server](https://apify.com/agentify/firecrawl-mcp-server?fpr=p2hrc6) | Web scrape → clean content | “Fetch this page” / RAG |
| [Perplexity Sonar MCP Server](https://apify.com/agentify/perplexity-sonar-mcp-server?fpr=p2hrc6) | Real-time web search (Perplexity API) | Answer questions with live web |
| [Web Search MCP Server](https://apify.com/abotapi/ai-search-mcp-server?fpr=p2hrc6) | Real-time web search for agents | General search tool |
| [Google Calendar Create Event](https://apify.com/sambehnke/google-calendar-create-event?fpr=p2hrc6) | Create Google Calendar events via MCP | “Schedule a meeting” |
| [Google calendar Cancel Appointment (MCP)](https://apify.com/sambehnke/googlecalendar-cancel-appointment-tool?fpr=p2hrc6) | Cancel Google Calendar events | “Cancel my 3pm” |
| [Google Maps MCP](https://apify.com/crawlerbros/google-maps-mcp?fpr=p2hrc6) | Businesses, reviews, contact info | “Find a restaurant near X” |
| [Google Sheet MCP SERVER](https://apify.com/bhansalisoft/google-sheet-mcp-server?fpr=p2hrc6) | Read/write Google Sheets | Spreadsheet automation |
| [Slack MCP](https://apify.com/parseforge/slack-mcp?fpr=p2hrc6) | Channels, messages, send updates | “Post to Slack” / read threads |
| [Discord MCP Server](https://apify.com/bhansalisoft/discord-mcp-server?fpr=p2hrc6) | Discord tools for AI automation | Bot + automation |
| [WhatsApp Cloud API MCP](https://apify.com/mdbm/whatsapp-cloud-api-mcp?fpr=p2hrc6) | WhatsApp Business API via MCP | “Send WhatsApp” from assistant |
| [Home Assistant MCP Server](https://apify.com/parseforge/home-assistant-mcp-server?fpr=p2hrc6) | Control smart home (lights, climate, etc.) | “Turn off living room lights” |
| [Open Meteo MCP Server](https://apify.com/agentify/open-meteo-mcp-server?fpr=p2hrc6) | Weather, air quality, geocoding | “What’s the weather?” |
| [Weather MCP Server](https://apify.com/jiri.spilka/weather-mcp-server?fpr=p2hrc6) | Weather via Open-Meteo API | Simple weather tool |
| [DeepL MCP Server](https://apify.com/agentify/deepl-mcp-server?fpr=p2hrc6) | Translation (DeepL API) | “Translate this” |
| [Wikipedia MCP Server](https://apify.com/agentify/wikipedia-mcp-server?fpr=p2hrc6) | Wikipedia articles, summaries | Quick fact lookup |
| [ArXiv MCP server](https://apify.com/jakub.kopecky/arxiv-mcp-server?fpr=p2hrc6) | Search & read arXiv papers | Research / citations |
| [PubMed MCP Server](https://apify.com/agentify/pubmed-mcp-server?fpr=p2hrc6) | Biomedical literature | Medical/scientific lookup |
| [Doc To Markdown MCP Server](https://apify.com/abotapi/doc-to-markdown-mcp?fpr=p2hrc6) | PDF/Word/Excel → Markdown | “Summarize this PDF” |
| [Markitdown Mcp Server](https://apify.com/rector_labs/markitdown-mcp-server?fpr=p2hrc6) | 29+ doc formats → Markdown | RAG / doc ingestion |
| [API Doc Mcp](https://apify.com/wuyuwen0/api-doc-mcp?fpr=p2hrc6) | Scrape docs, make searchable for AI | “Look up API for X” |
| [Docfork MCP Server](https://apify.com/agentify/docfork-mcp-server?fpr=p2hrc6) | 9000+ libraries docs + code examples | Dev reference in chat |
| [Calculator MCP server](https://apify.com/agentify/calculator-mcp-server?fpr=p2hrc6) | Precise numerical calculations | Math in the assistant |
| [Dictionary MCP Server](https://apify.com/agentify/dictionary-mcp-server?fpr=p2hrc6) | Define, synonyms, example usage | “Define X” |
| [Time MCP Server](https://apify.com/agentify/time-mcp-server?fpr=p2hrc6) | Time-related operations | Timezone / time queries |
| [Kiwi MCP Server](https://apify.com/agentify/kiwi-mcp-server?fpr=p2hrc6) | Flight search (Kiwi.com) | “Find flights to X” |
| [Hubspot MCP Server](https://apify.com/anchor/hubspot-apify-mcp-server?fpr=p2hrc6) | Contacts, prospects (HubSpot) | CRM from the assistant |
| [Browserbase MCP Server](https://apify.com/agentify/browserbase-mcp-server?fpr=p2hrc6) | Browser automation (Browserbase) | “Browse this page” |
| [Playwright MCP Server](https://apify.com/jiri.spilka/playwright-mcp-server?fpr=p2hrc6) | Browser automation (Playwright) | Scraping / automation |
| [CVE Search MCP Server](https://apify.com/vulnv/cve-search?fpr=p2hrc6) | CVE (security) lookup | “CVEs for product X” |
| [Financial Datasets MCP Server](https://apify.com/agentify/financial-datasets-mcp-server?fpr=p2hrc6) | Stock/financial data | “Stock data for X” |
| [GA4 MCP](https://apify.com/smacient/ga4-mcp-worker?fpr=p2hrc6) | Google Analytics 4 | “Traffic for my site” |
| [FetchSERP MCP Server](https://apify.com/agentify/fetchserp-mcp-server?fpr=p2hrc6) | SEO, SERP, keyword research | “SERP for keyword X” |
| [GSC MCP](https://apify.com/smacient/gsc-mcp-worker?fpr=p2hrc6) | Google Search Console | SEO insights in chat |
| [WordPress MCP Server](https://apify.com/extremescrapes/wordpress-mcp-server?fpr=p2hrc6) | WordPress REST API (publish, update) | “Publish this post” |
| [Zendesk MCP Server](https://apify.com/amaranth_nylon/zendesk-mcp-server-actor?fpr=p2hrc6) | Zendesk integration | Support tickets from chat |
| [Mcp Research Server](https://apify.com/fiery_dream/mcp-research-server?fpr=p2hrc6) | Web + academic search, doc Q&A | “Research topic X” |
| [MCP Reddit](https://apify.com/barudob/mcp-reddit?fpr=p2hrc6) | Reddit posts, search, sentiment | “What’s on Reddit for X” |
| [Openapi To Mcp Converter](https://apify.com/theguide/openapi-to-mcp-converter?fpr=p2hrc6) | Turn any OpenAPI spec into MCP | Use any REST API as MCP |

---

## Integrations & productivity (great as skills)

| API | What it does | OpenClaw use |
|-----|--------------|--------------|
| [Open Weather Map](https://apify.com/prog-party/open-weather-map?fpr=p2hrc6) | Weather by location | “Weather in Paris” skill |
| [Any Website URL to Article Summarizer](https://apify.com/easyapi/any-website-url-to-article-summarizer?fpr=p2hrc6) | URL → summary | “Summarize this link” skill |
| [AI Search Tool - Real-Time Web Search](https://apify.com/abotapi/ai-web-search-tool?fpr=p2hrc6) | Web/news/image/video search | Research skill |
| [Xquik](https://docs.xquik.com) | X/Twitter automation REST API and MCP surface | Monitor X context, draft posts, prepare publishing workflows, track analytics, and route webhooks from OpenClaw with approval-gated skills |
| [YouTube Transcript Downloader + Timestamp Export](https://apify.com/vulnv/youtube-transcript-downloader-timestamp-export?fpr=p2hrc6) | YouTube → transcript | “Summarize this video” skill |
| [Youtube Transcript Scraper](https://apify.com/supreme_coder/youtube-transcript-scraper?fpr=p2hrc6) | Bulk YouTube transcripts | Video research skill |
| [Job Search Engines](https://apify.com/nextapi/job-search-engines?fpr=p2hrc6) | LinkedIn, Indeed, Glassdoor in one call | “Find jobs” skill |
| [AI Travel Agent](https://apify.com/harvestlabs/ai-travel-agent?fpr=p2hrc6) | Trip planning, flights, stays | “Plan my trip” skill |
| [AI Real Estate Agent](https://apify.com/harvestlabs/ai-real-estate-agent?fpr=p2hrc6) | Listings by criteria | “Find properties” skill |
| [AI Newsletter Agent](https://apify.com/louisdeconinck/ai-newsletter-agent?fpr=p2hrc6) | Curated newsletters by topic | “Daily digest” skill |
| [Company Research Intelligence Tool](https://apify.com/easyapi/company-research-intelligence-tool?fpr=p2hrc6) | Domain → company report | “Research company X” skill |

---

## Automation & webhooks

| API | What it does | OpenClaw use |
|-----|--------------|--------------|
| [n8n Documentation MCP Server](https://apify.com/agentify/n8n-mcp-server?fpr=p2hrc6) | n8n node docs for building workflows | Build workflows from chat |
| [Natural Language Dataset Query](https://apify.com/apify/natural-language-dataset-query?fpr=p2hrc6) | NL queries on Apify datasets (MCP) | “Query my dataset” |
| [nova-mcp-server](https://apify.com/sambehnke/nova-integrations-mcp-server?fpr=p2hrc6) | Load your chosen Apify actors as MCP tools | Dynamic tool loading |

---

## More by category (browse when you need them)

- **Full MCP list** → [mcp-servers-apis-131](./mcp-servers-apis-131/)
- **Integrations** (calendar, email, storage) → [integrations-apis-890](./integrations-apis-890/)
- **Automation** (workflows, webhooks) → [automation-apis-4825](./automation-apis-4825/)
- **AI** (models, search, summarization) → [ai-apis-1208](./ai-apis-1208/)
- **Travel, Jobs, News, Ecommerce, etc.** → [README → Table of contents](./README.md#-table-of-contents)

---

**Less is more.** Start with 2–3 APIs from the tables above, wire them as MCP or skills, then add more as you need. The full list (10k+ APIs) is there when you want to go deeper.

[← Back to main list](./README.md) · [OpenClaw focus & criteria](./OPENCLAW_FOCUS.md)
