# AI Automation Workflows — Tony Wong / Zentorin

A collection of production n8n automation workflows built and deployed as part of real business systems. These are exported from live environments — not demos or templates.

> Built by [Tony Wong](https://zentorin.co.nz) · AI & Automation Specialist · New Zealand

---

## What's in here

These workflows are organised by system. Each folder contains the exported JSON and a README explaining what the workflow does, how it's connected, and what problem it solves.

---

### `/dalaikarma` — Personal AI Agent System

A modular multi-agent AI assistant with Telegram interface, persistent memory, and 20+ skills.

| Workflow | Description |
|---|---|
| `00-telegram-entry` | Telegram bot entry point — receives messages and routes to gateway |
| `01-gateway` | Central hub — dispatches incoming requests to the right handler |
| `02-router` | Routes between Gateway, DKB, and SSH execution paths |
| `03-ai-agent-executor` | Core AI execution layer — runs LLM-powered tasks |
| `06-memory-integration` | Persistent memory integration — reads/writes long-term context |
| `07-memory-manager-api` | Memory Manager API — CRUD interface for agent memory |
| `21-gmail-skill` | Gmail integration skill |
| `22-web-search-skill` | Live web search capability |
| `23-web-scraper-skill` | Web scraping skill with structured output |
| `25-calendar-skill` | Google Calendar read/write skill |
| `27-notes-skill` | Notes creation and retrieval |
| `28-github-skill` | GitHub integration |
| `30-browser-automation` | Browser automation via CDP |
| `31-daily-briefing` | Automated daily briefing generation |
| `32-decision-framework` | Structured decision-making workflow |

---

### `/bos` — Business Operating System

Productised AI automation suite for SME clients via Zentorin.

| Workflow | Description |
|---|---|
| `central-hub` | Command and control API — central routing for all BOS modules |
| `lead-engine` | AI lead scoring and audit trigger |
| `audit-pipeline` | Score → report → deliver, fully automated |
| `rag-knowledge-system` | Document ingest and contextual query system |
| `follow-up-sequence` | Automated follow-up engine |
| `blog-automation` | AI-powered blog content pipeline |
| `daily-intelligence-briefing` | Daily AI-curated business intelligence report |
| `technical-discovery` | Stack audit and technical discovery for new clients |

---

### `/zentorin` — Consultancy Infrastructure

Powers zentorin.co.nz and client intake processes.

| Workflow | Description |
|---|---|
| `ai-audit-engine-v2` | Full AI readiness audit — intake to scored report |
| `tradie-audit-intake` | Specialised intake for trades/SME clients |
| `audit-self-review-loop` | Automated quality review of generated audit reports |
| `audit-commander` | Manual trigger mode for audit pipeline |
| `audit-log-api` | Audit logging and tracking API |
| `daily-9am-briefing` | Scheduled daily briefing for Zentorin ops |

---

### `/orbit` — Intelligence & Monitoring

| Workflow | Description |
|---|---|
| `orbit-ai-radar` | AI trend and signal monitoring |
| `orbit-daily-digest` | Automated daily digest compilation |
| `orbit-job-hunter` | Automated job opportunity scanning and Telegram notification |

---

### `/nexus` — Market Intelligence

| Workflow | Description |
|---|---|
| `nexus-live-price-feed` | Real-time market data ingestion |
| `nexus-ai-market-analysis` | AI-powered market analysis and reporting |

---

### `/openswarm-intel` — AI Research Pipeline

| Workflow | Description |
|---|---|
| `ai-auto-research` | Dual-LLM research pipeline (Claude + GPT) feeding OpenSwarm knowledge base |

---

## How to use these

1. Import any JSON file into your n8n instance via **Settings → Import Workflow**
2. Review and update credential references (all sensitive credentials have been removed — you'll need to reconnect your own)
3. Check the inline notes on each workflow for setup requirements

---

## About

These workflows are part of a larger AI automation ecosystem including:

- **DalaiKarma** — multi-agent personal AI assistant
- **OpenSwarm** — autonomous AI agent platform (Rust + React + SQLite)
- **BOS** — Business Operating System for SME clients
- **Zentorin** — AI consultancy platform

More at [zentorin.co.nz](https://zentorin.co.nz)
