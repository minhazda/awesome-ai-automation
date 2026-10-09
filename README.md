# Awesome AI & Workflow Automation [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated, opinionated map of the best open-source tools for automating work — from no-code workflow builders to AI browser agents to code-first orchestrators. Every tool is self-hostable and free to start.

Most "automation tool" lists are undifferentiated dumps. This one is organized by **the decision you're actually making** and says *when to reach for each*, so you can go from "I need to automate X" to the right tool in under a minute. Star counts are live badges — they update themselves.

Maintained by [MD Minhazur Rahman](https://github.com/minhazda) — an automation & ML engineer. PRs welcome (see [Contributing](CONTRIBUTING.md)).

## Contents

- [Pick the right tool in 30 seconds](#pick-the-right-tool-in-30-seconds)
- [No-code / low-code workflow builders](#no-code--low-code-workflow-builders)
- [AI agents & LLM automation](#ai-agents--llm-automation)
- [AI browser agents](#ai-browser-agents)
- [Code-first data & workflow orchestration](#code-first-data--workflow-orchestration)
- [Web scraping & data extraction](#web-scraping--data-extraction)
- [Browser automation & RPA libraries](#browser-automation--rpa-libraries)
- [How to self-host any of these for free](#how-to-self-host-any-of-these-for-free)

---

## Pick the right tool in 30 seconds

| If you want to… | Reach for | Why |
|---|---|---|
| Wire SaaS apps together with a visual editor | **n8n**, **Activepieces** | Fastest path; hundreds of integrations, self-hostable |
| Turn scripts into scheduled workflows + auto UIs | **Windmill**, **Trigger.dev** | Code-first, developer-oriented |
| Build an LLM app / agent with a visual canvas | **Dify**, **Flowise** | RAG + agents without gluing frameworks by hand |
| Have an AI *use a real website* for you | **browser-use**, **Skyvern** | Vision/DOM agents that click and type |
| Orchestrate data pipelines with dependencies & retries | **Airflow**, **Dagster**, **Prefect** | Battle-tested DAG schedulers |
| Guarantee a long-running process never loses state | **Temporal** | Durable execution / sagas |
| Scrape or crawl sites into clean data | **Firecrawl**, **Crawlee**, **Scrapy** | Purpose-built extraction |
| Drive a browser from code (RPA) | **Playwright**, **Puppeteer** | Reliable, headless, CI-friendly |

---

## No-code / low-code workflow builders

The Zapier/Make replacements. Reach for these first when the job is "when X happens in app A, do Y in app B."

- **[n8n](https://github.com/n8n-io/n8n)** ![](https://img.shields.io/github/stars/n8n-io/n8n?style=flat&label=%E2%AD%90&color=444) — Visual, fair-code workflow builder with 400+ integrations and inline code nodes. The default self-hosted Zapier alternative, and the tool most frequently named in European automation job posts.
- **[Activepieces](https://github.com/activepieces/activepieces)** ![](https://img.shields.io/github/stars/activepieces/activepieces?style=flat&label=%E2%AD%90&color=444) — MIT-licensed, AI-first, no-code automation. Cleanest "pieces" model if you want to publish your own reusable integrations.
- **[Windmill](https://github.com/windmill-labs/windmill)** ![](https://img.shields.io/github/stars/windmill-labs/windmill?style=flat&label=%E2%AD%90&color=444) — Turn Python/TypeScript/Go scripts into production workflows with auto-generated UIs and APIs. The pick when you want code, not just boxes.
- **[Node-RED](https://github.com/node-red/node-red)** ![](https://img.shields.io/github/stars/node-red/node-red?style=flat&label=%E2%AD%90&color=444) — Flow-based programming born in IoT; still excellent for event wiring and hardware.
- **[Kestra](https://github.com/kestra-io/kestra)** ![](https://img.shields.io/github/stars/kestra-io/kestra?style=flat&label=%E2%AD%90&color=444) — Declarative, YAML-defined orchestration that scales from simple flows to data pipelines.
- **[Huginn](https://github.com/huginn/huginn)** ![](https://img.shields.io/github/stars/huginn/huginn?style=flat&label=%E2%AD%90&color=444) — The original self-hosted "agents that watch and act on the web." Venerable and dependency-light.
- **[Automatisch](https://github.com/automatisch/automatisch)** ![](https://img.shields.io/github/stars/automatisch/automatisch?style=flat&label=%E2%AD%90&color=444) — Open-source Zapier alternative focused on data staying on your servers.
- **[Trigger.dev](https://github.com/triggerdotdev/trigger.dev)** ![](https://img.shields.io/github/stars/triggerdotdev/trigger.dev?style=flat&label=%E2%AD%90&color=444) — Write long-running background jobs and workflows as TypeScript, with retries and observability built in.

## AI agents & LLM automation

For automations where the "logic" is a language model — routing, drafting, extracting, deciding.

- **[Dify](https://github.com/langgenius/dify)** ![](https://img.shields.io/github/stars/langgenius/dify?style=flat&label=%E2%AD%90&color=444) — Production LLM app platform: RAG pipelines, agents, and workflows on a visual canvas with observability.
- **[CrewAI](https://github.com/crewAIInc/crewAI)** ![](https://img.shields.io/github/stars/crewAIInc/crewAI?style=flat&label=%E2%AD%90&color=444) — Framework for orchestrating role-playing, collaborating AI agents. Popular for multi-agent task automation.
- **[Flowise](https://github.com/FlowiseAI/Flowise)** ![](https://img.shields.io/github/stars/FlowiseAI/Flowise?style=flat&label=%E2%AD%90&color=444) — Drag-and-drop builder for LLM chains and agents; the visual counterpart to writing LangChain by hand.
- **[OpenLeo](https://github.com/ancs21/openleo)** ![](https://img.shields.io/github/stars/ancs21/openleo?style=flat&label=%E2%AD%90&color=444) — A to-do board where agents do the cards on the board's own Linux computer, running on your ChatGPT plan; reach for it when you'd rather write a task than build a workflow.

## AI browser agents

The hottest corner of automation: agents that operate real web pages via vision and/or the DOM.

- **[browser-use](https://github.com/browser-use/browser-use)** ![](https://img.shields.io/github/stars/browser-use/browser-use?style=flat&label=%E2%AD%90&color=444) — Make any website usable by an AI agent. Currently the most-starred AI browser-automation project and a top-100 GitHub repo.
- **[Skyvern](https://github.com/Skyvern-AI/skyvern)** ![](https://img.shields.io/github/stars/Skyvern-AI/skyvern?style=flat&label=%E2%AD%90&color=444) — Vision-first browser automation that navigates portals it has never seen; strong on forms and workflows.
- **[Stagehand](https://github.com/browserbase/stagehand)** ![](https://img.shields.io/github/stars/browserbase/stagehand?style=flat&label=%E2%AD%90&color=444) — Add a few AI-driven `act`/`extract` calls on top of Playwright without giving up deterministic control.

## Code-first data & workflow orchestration

When you need dependencies, backfills, retries, and scheduling for data or ML pipelines.

- **[Apache Airflow](https://github.com/apache/airflow)** ![](https://img.shields.io/github/stars/apache/airflow?style=flat&label=%E2%AD%90&color=444) — The industry-standard DAG scheduler. Ubiquitous in data engineering job descriptions.
- **[Prefect](https://github.com/PrefectHQ/prefect)** ![](https://img.shields.io/github/stars/PrefectHQ/prefect?style=flat&label=%E2%AD%90&color=444) — Pythonic orchestration with a gentler learning curve than Airflow; dynamic, code-native flows.
- **[Dagster](https://github.com/dagster-io/dagster)** ![](https://img.shields.io/github/stars/dagster-io/dagster?style=flat&label=%E2%AD%90&color=444) — Asset-oriented orchestrator with typed, testable pipelines and great local dev ergonomics.
- **[Temporal](https://github.com/temporalio/temporal)** ![](https://img.shields.io/github/stars/temporalio/temporal?style=flat&label=%E2%AD%90&color=444) — Durable execution: workflows that survive crashes and run for days without losing state.

## Web scraping & data extraction

- **[Firecrawl](https://github.com/firecrawl/firecrawl)** ![](https://img.shields.io/github/stars/firecrawl/firecrawl?style=flat&label=%E2%AD%90&color=444) — Turn any website into clean, LLM-ready markdown/JSON. The go-to for feeding sites into AI pipelines.
- **[Crawlee](https://github.com/apify/crawlee)** ![](https://img.shields.io/github/stars/apify/crawlee?style=flat&label=%E2%AD%90&color=444) — Node/Python scraping and crawling library with anti-blocking, queues, and headless browser support.
- **[Scrapy](https://github.com/scrapy/scrapy)** ![](https://img.shields.io/github/stars/scrapy/scrapy?style=flat&label=%E2%AD%90&color=444) — The mature, high-throughput Python scraping framework. Still unmatched for large structured crawls.

## Browser automation & RPA libraries

Drive browsers deterministically from code — the foundation under most RPA.

- **[Playwright](https://github.com/microsoft/playwright)** ![](https://img.shields.io/github/stars/microsoft/playwright?style=flat&label=%E2%AD%90&color=444) — Modern cross-browser automation with auto-waiting and great CI support. The current default for reliable browser RPA.
- **[Puppeteer](https://github.com/puppeteer/puppeteer)** ![](https://img.shields.io/github/stars/puppeteer/puppeteer?style=flat&label=%E2%AD%90&color=444) — Chrome/Chromium automation via the DevTools Protocol; battle-tested for scraping and PDF/render tasks.
- **[Selenium](https://github.com/SeleniumHQ/selenium)** ![](https://img.shields.io/github/stars/SeleniumHQ/selenium?style=flat&label=%E2%AD%90&color=444) — The long-standing cross-language, cross-browser standard; widest ecosystem and grid support.
- **[Robot Framework](https://github.com/robotframework/robotframework)** ![](https://img.shields.io/github/stars/robotframework/robotframework?style=flat&label=%E2%AD%90&color=444) — Keyword-driven automation popular for RPA and acceptance testing; readable by non-developers.

---

## How to self-host any of these for free

You don't need a paid cloud to run or demo these:

- **Docker on a free-tier VM** — [Oracle Cloud Always Free](https://www.oracle.com/cloud/free/) gives 4 ARM cores/24 GB RAM indefinitely; enough for n8n, Activepieces, or Windmill via their official `docker-compose`.
- **GitHub Actions** as a scheduler — free minutes for public repos make Actions a zero-cost cron for scripts and scrapers.
- **Hugging Face Spaces / Streamlit Community Cloud** — free hosting for a UI on top of any of the Python tools here.

---

## Contributing

Suggestions and additions welcome — the bar is: open-source, self-hostable, actively maintained, and genuinely useful for automation. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/80x15.png)](LICENSE) — released under CC0 (public domain). Tool names and trademarks belong to their respective owners; this list only links to and describes them.
