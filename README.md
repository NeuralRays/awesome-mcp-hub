# Awesome MCP Hub

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/NeuralRays/awesome-mcp-hub/pulls)
[![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-8B5CF6)](https://modelcontextprotocol.io/)
[![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/NeuralRays/awesome-mcp-hub/commits/main)

> The curated, comprehensive directory of MCP servers and clients — with quality reviews, compatibility info, and difficulty ratings.

**Model Context Protocol (MCP)** is an open standard that lets AI assistants connect to external tools, data sources, and services. This hub helps you find the right MCP servers for your workflow.

---

## What Makes This Different

| Feature | Other Lists | Awesome MCP Hub |
|---------|------------|-----------------|
| Quality reviews | No — everything listed equally | **Editor's Picks** with pros/cons |
| Client compatibility | No — "does it work with Cursor?" unknown | **Compatibility matrix** for every server |
| Setup difficulty | No — beginners can't tell easy from hard | **Difficulty ratings** (Easy/Medium/Advanced) |
| Comparison tables | No — hard to choose between similar servers | **Side-by-side comparisons** within categories |
| Maintenance status | No — abandoned servers mixed with active ones | **Active/Maintained/Stale** indicators |

---

## Legend

**Difficulty:**
| Badge | Meaning |
|-------|---------|
| ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | One command setup, no API keys needed |
| ![Medium](https://img.shields.io/badge/-Medium-yellow) | Requires API keys or configuration |
| ![Advanced](https://img.shields.io/badge/-Advanced-red) | Requires infrastructure (Docker, databases, cloud) |

**Language:**
| Icon | Language |
|------|----------|
| TS | TypeScript/JavaScript |
| PY | Python |
| GO | Go |
| RS | Rust |
| JV | Java/Kotlin |
| CS | C# |

**Client Compatibility:**
| Icon | Client |
|------|--------|
| CD | Claude Desktop |
| CC | Claude Code |
| CU | Cursor |
| WS | Windsurf |
| CN | Continue |
| CL | Cline |

---

## Table of Contents

- [Editor's Picks (Curated)](#-editors-picks)
- [Community Directory](#-community-directory)
  - [Code Analysis & Intelligence](#code-analysis--intelligence)
  - [Version Control & Git](#version-control--git)
  - [Code Execution & Sandboxes](#code-execution--sandboxes)
  - [Databases (SQL)](#databases-sql)
  - [Databases (NoSQL & Key-Value)](#databases-nosql--key-value)
  - [Vector Databases & RAG](#vector-databases--rag)
  - [Web Browsing & Scraping](#web-browsing--scraping)
  - [Search Engines](#search-engines)
  - [API Integration](#api-integration)
  - [Cloud Platforms (AWS)](#cloud-platforms-aws)
  - [Cloud Platforms (GCP)](#cloud-platforms-gcp)
  - [Cloud Platforms (Azure)](#cloud-platforms-azure)
  - [Containers & Orchestration](#containers--orchestration)
  - [CI/CD & DevOps](#cicd--devops)
  - [Messaging & Communication](#messaging--communication)
  - [Project Management](#project-management)
  - [Documents & Notes](#documents--notes)
  - [Email & Calendar](#email--calendar)
  - [AI & LLM Tools](#ai--llm-tools)
  - [Knowledge & Memory](#knowledge--memory)
  - [Shell & Terminal](#shell--terminal)
  - [System Monitoring](#system-monitoring)
  - [Desktop Automation](#desktop-automation)
  - [Finance & Crypto](#finance--crypto)
  - [Social Media](#social-media)
  - [CMS & Publishing](#cms--publishing)
  - [Design & Visualization](#design--visualization)
  - [Security](#security)
  - [Maps & Location](#maps--location)
  - [Science & Research](#science--research)
  - [Media & Entertainment](#media--entertainment)
  - [Translation & Language](#translation--language)
  - [Other Tools](#other-tools)
- [MCP Clients](#-mcp-clients)
- [Getting Started Guide](#-getting-started)
- [Contributing](#-contributing)

---

## :star2: Editor's Picks

Hand-picked servers tested for quality, reliability, and usefulness. Each has been personally reviewed.

### :trophy: Best Overall

| Server | What It Does | Install | Difficulty | Clients | Why It's Picked |
|--------|-------------|---------|------------|---------|----------------|
| [**filesystem**](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | Read/write local files with security boundaries | `npx @modelcontextprotocol/server-filesystem` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN CL | Universal — every AI workflow needs file access. Official reference server. |
| [**GitHub**](https://github.com/modelcontextprotocol/servers/tree/main/src/github) | Repos, issues, PRs, code search | `npx @modelcontextprotocol/server-github` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Essential for any dev workflow. Needs `GITHUB_TOKEN`. |
| [**Brave Search**](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) | Web + local search via Brave API | `npx @modelcontextprotocol/server-brave-search` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Best free web search MCP. 2000 free queries/month. |
| [**PostgreSQL**](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) | Query PostgreSQL databases | `npx @modelcontextprotocol/server-postgres` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Rock-solid database access. Read-only by default (safe). |
| [**memory**](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | Persistent knowledge graph for context | `npx @modelcontextprotocol/server-memory` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN CL | AI agents that remember across sessions. Zero config. |

### :fire: Best for Developers

| Server | What It Does | Install | Difficulty | Clients | Why It's Picked |
|--------|-------------|---------|------------|---------|----------------|
| [**CodeXRay**](https://github.com/NeuralRays/codexray) | 16-tool semantic code intelligence — knowledge graph, TF-IDF search, call graphs, dead code, impact analysis | `npx codexray` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS | Saves 30%+ tokens. One `codexray_context` call replaces 5-10 file reads. 15 languages. |
| [**Context7**](https://github.com/upstash/context7) | Up-to-date library docs for any framework | `npx context7` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN CL | No more outdated docs. AI gets current React/Next.js/etc docs on demand. |
| [**Puppeteer**](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) | Browser automation, screenshots, scraping | `npx @modelcontextprotocol/server-puppeteer` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN CL | Official reference server. Headless Chrome for AI agents. |
| [**Sequential Thinking**](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) | Step-by-step reasoning and thought chains | `npx @modelcontextprotocol/server-sequential-thinking` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN CL | Makes AI reason more carefully through complex problems. |
| [**E2B Code Interpreter**](https://github.com/e2b-dev/mcp-server) | Sandboxed code execution in cloud | `npx @e2b/mcp-server` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN | Safe code execution without touching your machine. Needs API key. |

### :zap: Best for Productivity

| Server | What It Does | Install | Difficulty | Clients | Why It's Picked |
|--------|-------------|---------|------------|---------|----------------|
| [**Notion**](https://github.com/makenotion/notion-mcp-server) | Read/write Notion pages, databases | `npx @notionhq/notion-mcp-server` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Official server from Notion. Full workspace access. |
| [**Slack**](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) | Channel management, messaging, search | `npx @modelcontextprotocol/server-slack` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Official reference. Full Slack workspace integration. |
| [**Linear**](https://github.com/linear/linear-mcp-server) | Issue tracking, project management | `npx @linear/mcp-server` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN | Official server. Manage issues and projects with AI. |
| [**Google Drive**](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) | Search and access Google Drive files | `npx @modelcontextprotocol/server-gdrive` | ![Medium](https://img.shields.io/badge/-Medium-yellow) | CD CC CU WS CN CL | Official reference. OAuth setup required. |
| [**Obsidian**](https://github.com/smithery-ai/mcp-obsidian) | Read/search Obsidian vault notes | `npx mcp-obsidian` | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) | CD CC CU WS CN | Bridge your knowledge base to AI. Local vault access. |

---

## :books: Community Directory

Open to all submissions via [pull request](CONTRIBUTING.md). Sorted alphabetically within each category.

---

### Code Analysis & Intelligence

Tools for understanding, searching, and analyzing codebases.

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [code-context-provider-mcp](https://github.com/AB498/code-context-provider-mcp) | Code context and analysis via WebAssembly tree-sitter | `npx code-context-provider-mcp` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [CodeLogic](https://github.com/CodeLogicIncEngineering/codelogic-mcp-server) | Code dependency analytics and architectural risk analysis | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [**CodeXRay**](https://github.com/NeuralRays/codexray) | 16-tool semantic code intelligence with knowledge graph, TF-IDF, call graphs, dead code, impact analysis | `npx codexray` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [FileScopeMCP](https://github.com/admica/FileScopeMCP) | Codebase analysis via dependency relationships and importance scoring | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [javalens-mcp](https://github.com/pzalutski-pixel/javalens-mcp) | 56 semantic Java analysis tools via Eclipse JDT | See repo | JV | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [mcp-gopls](https://github.com/hloiseaufcms/mcp-gopls) | Go Language Server Protocol (gopls) integration | See repo | GO | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [react-analyzer-mcp](https://github.com/azer/react-analyzer-mcp) | Analyze React code, generate docs/llm.txt for whole projects | `npx react-analyzer-mcp` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [sharplens-mcp](https://github.com/pzalutski-pixel/sharplens-mcp) | 58 semantic C#/.NET analysis tools via Roslyn | See repo | CS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |

### Version Control & Git

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [git-mcp](https://github.com/idosal/git-mcp) | Connect to ANY GitHub repo for documentation via gitmcp.io | Remote URL | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [GitHub](https://github.com/modelcontextprotocol/servers/tree/main/src/github) | Official — repos, issues, PRs, code search | `npx @modelcontextprotocol/server-github` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [GitLab](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) | Official — GitLab API integration | `npx @modelcontextprotocol/server-gitlab` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [gitingest-mcp](https://github.com/narumiruna/gitingest-mcp) | Convert any Git repo into a text digest | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [GitKraken](https://github.com/gitkraken/gk-cli) | Official — GitKraken, Jira, GitHub, GitLab integration via `gk mcp` | `gk mcp` | GO | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [mcp-gitlab-jira](https://github.com/HainanZhao/mcp-gitlab-jira) | Unified GitLab and Jira server | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Code Execution & Sandboxes

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [code-sandbox-mcp](https://github.com/Automata-Labs-team/code-sandbox-mcp) | Secure code execution in Docker containers | See repo | TS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [E2B Code Interpreter](https://github.com/e2b-dev/mcp-server) | Sandboxed code execution in cloud | `npx @e2b/mcp-server` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [mcp-code-runner](https://github.com/axliupore/mcp-code-runner) | Run code locally via Docker, multiple languages | See repo | TS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [mcp_code_executor](https://github.com/bazinga012/mcp_code_executor) | Execute Python in Conda environments | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Databases (SQL)

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [CockroachDB](https://github.com/amineelkouhen/mcp-cockroachdb) | CockroachDB management and querying | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [dbhub](https://github.com/bytebase/dbhub) | Universal database server supporting mainstream databases | `npx dbhub` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [MySQL](https://github.com/benborla/mcp-server-mysql) | MySQL database integration | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Neon](https://github.com/neondatabase/mcp-server-neon) | Serverless Postgres via Neon | `npx @neondatabase/mcp-server-neon` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [PostgreSQL](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) | Official — PostgreSQL querying | `npx @modelcontextprotocol/server-postgres` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [SQLite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) | Official — Local SQLite database | `npx @modelcontextprotocol/server-sqlite` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Databases (NoSQL & Key-Value)

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [ArangoDB](https://github.com/ravenwits/mcp-server-arangodb) | ArangoDB graph database interaction | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [MongoDB](https://github.com/kiliczsh/mcp-mongo-server) | MongoDB database interaction | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Neo4j](https://github.com/neo4j-contrib/mcp-neo4j) | Neo4j graph database with knowledge graph memory | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [Redis / Upstash](https://github.com/upstash/mcp-server-upstash) | Serverless Redis via Upstash | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Vector Databases & RAG

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [ChromaDB](https://github.com/chroma-core/chroma-mcp) | ChromaDB vector database | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [local-faiss-mcp](https://github.com/nonatofabio/local_faiss_mcp) | Local FAISS vector DB with document ingestion and semantic search | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Pinecone](https://github.com/pinecone-io/pinecone-mcp) | Pinecone vector database | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Qdrant](https://github.com/qdrant/mcp-server-qdrant) | Qdrant vector database search | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Web Browsing & Scraping

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Browser MCP](https://github.com/browsermcp/mcp) | Automate your local browser | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Browserbase](https://github.com/browserbase/mcp-server-browserbase) | Cloud browser automation | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) | Official — HTTP requests and web content fetching | `npx @modelcontextprotocol/server-fetch` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [Firecrawl](https://github.com/mendableai/firecrawl-mcp-server) | Advanced web scraping with LLM-ready markdown output | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Playwright](https://github.com/executeautomation/mcp-playwright) | Browser automation via Playwright | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) | Official — Headless Chrome browser automation | `npx @modelcontextprotocol/server-puppeteer` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Search Engines

**Comparison:**

| Feature | Brave Search | Tavily | Exa | SearXNG |
|---------|-------------|--------|-----|---------|
| Free tier | 2,000/mo | 1,000/mo | 1,000/mo | Unlimited (self-host) |
| API key needed | Yes | Yes | Yes | No (self-host) |
| AI-optimized results | No | Yes | Yes | No |
| Local search | Yes | No | No | Configurable |
| Setup difficulty | Medium | Medium | Medium | Advanced |

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Brave Search](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) | Official — Web and local search via Brave API | `npx @modelcontextprotocol/server-brave-search` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Exa](https://github.com/exa-labs/exa-mcp-server) | AI-native search engine | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [SearXNG](https://github.com/ihor-sokoliuk/mcp-searxng) | Self-hosted meta search engine | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [Tavily](https://github.com/tavily-ai/tavily-mcp) | AI-optimized search with real-time results | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### API Integration

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [APIWeaver](https://github.com/GongRzhe/APIWeaver) | Dynamically create MCP servers from web API configs | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [mcp-openapi](https://github.com/ReAPI-com/mcp-openapi) | Let LLMs know everything about your OpenAPI specs | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [openapi-to-mcp](https://github.com/bbonnin/openapi-to-mcp) | Auto-convert any OpenAPI/Swagger spec into MCP tools | See repo | JV | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [postmancer](https://github.com/hijaz/postmancer) | Postman/Insomnia replacement — manage API collections via MCP | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Cloud Platforms (AWS)

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [AWS KB Retrieval](https://github.com/modelcontextprotocol/servers/tree/main/src/aws-kb-retrieval-server) | Official — AWS Knowledge Base retrieval | See repo | TS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [AWS EC2 Pricing](https://github.com/trilogy-group/aws-pricing-mcp) | Up-to-date EC2 pricing info | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Cloud Platforms (GCP)

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [BigQuery](https://github.com/LucasHild/mcp-server-bigquery) | Google BigQuery integration | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Google Drive](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) | Official — Google Drive file access | `npx @modelcontextprotocol/server-gdrive` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Google Maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) | Official — Google Maps API | `npx @modelcontextprotocol/server-google-maps` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Cloud Platforms (Azure)

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Azure](https://github.com/Azure/azure-mcp) | Official — Azure resource management | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |

### Containers & Orchestration

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Docker](https://github.com/ckreiling/mcp-server-docker) | Manage containers, images, volumes, networks | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Docker Hub](https://github.com/docker/hub-mcp) | Official — Docker Hub repos, search, hardened images | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Kubernetes](https://github.com/QuantGeekDev/docker-mcp) | Container management and operations | See repo | GO | ![Advanced](https://img.shields.io/badge/-Advanced-red) |

### CI/CD & DevOps

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Buildkite](https://github.com/buildkite/buildkite-mcp-server) | Official — pipelines, builds, diagnostics | See repo | GO | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [CircleCI](https://github.com/CircleCI-Public/mcp-server-circleci) | Fix build failures from CircleCI | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Jenkins](https://github.com/avisangle/jenkins-mcp-server) | 21 tools for Jenkins CI/CD management | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [Terraform](https://github.com/nwiizo/tfmcp) | Manage Terraform environments via AI | See repo | RS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |

### Messaging & Communication

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Discord](https://github.com/v-3/discordmcp) | Discord server interaction | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) | Official — channels, messaging, search | `npx @modelcontextprotocol/server-slack` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Telegram](https://github.com/nicobailey/mcp-telegram) | Telegram bot interaction | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Project Management

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Jira](https://github.com/aashari/mcp-server-atlassian-jira) | Atlassian Jira Cloud integration | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Linear](https://github.com/linear/linear-mcp-server) | Official — issue tracking, project management | `npx @linear/mcp-server` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Sentry](https://github.com/getsentry/sentry-mcp) | Error tracking and debugging | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Todoist](https://github.com/abhiz123/todoist-mcp-server) | Todoist task management | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Documents & Notes

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Confluence](https://github.com/aashari/mcp-server-atlassian-confluence) | Atlassian Confluence spaces and pages | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Notion](https://github.com/makenotion/notion-mcp-server) | Official — Notion pages and databases | `npx @notionhq/notion-mcp-server` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Obsidian](https://github.com/smithery-ai/mcp-obsidian) | Read and search Obsidian vault | `npx mcp-obsidian` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Email & Calendar

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Apple Calendar](https://github.com/Omar-v2/mcp-ical) | macOS Calendar interaction via natural language | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [CalDAV](https://github.com/dominik1001/caldav-mcp) | CalDAV calendar operations | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Commune MCP](https://github.com/commune-sh/commune-mcp) | Agent email infrastructure — provision inboxes, send/receive email, threads, custom domains, structured extraction, SMS | `uvx commune-mcp` | PY | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [Gmail / Google](https://github.com/nicobailey/mcp-gmail) | Gmail integration | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### AI & LLM Tools

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [any-chat-completions](https://github.com/pyroprompts/any-chat-completions-mcp) | Chat with any OpenAI-compatible API | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Context7](https://github.com/upstash/context7) | Up-to-date library documentation for AI | `npx context7` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [Sequential Thinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) | Official — step-by-step reasoning chains | `npx @modelcontextprotocol/server-sequential-thinking` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Knowledge & Memory

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [cognee-mcp](https://github.com/topoteretes/cognee/tree/main/cognee-mcp) | GraphRAG memory with customizable ingestion | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | Official — persistent knowledge graph | `npx @modelcontextprotocol/server-memory` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [memora](https://github.com/agentic-mcp-tools/memora) | Persistent memory with graph visualization and cloud sync | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Shell & Terminal

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [commands](https://github.com/g0t4/mcp-server-commands) | Run commands and scripts, just like in a terminal | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [Console Automation](https://github.com/ooples/mcp-console-automation) | AI-driven console automation with 40 tools | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### System Monitoring

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Netdata](https://github.com/netdata/netdata) | Full observability — metrics, logs, containers, processes | See repo | — | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [PostHog](https://github.com/posthog/mcp) | Official — analytics, feature flags, error tracking | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Desktop Automation

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Apple Script](https://github.com/peakmojo/applescript-mcp) | Run AppleScript to control anything on Mac | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [DroidMind](https://github.com/hyperb1iss/droidmind) | Android device control, debugging, UI automation | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [iOS Simulator](https://github.com/InditexTech/mcp-server-simulator-ios-idb) | Control iOS simulators via natural language | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Finance & Crypto

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Algorand](https://github.com/GoPlausible/algorand-mcp) | 40+ tools for Algorand blockchain | See repo | TS | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [CoinMarketCap](https://github.com/shinzo-labs/coinmarketcap-mcp) | Complete CoinMarketCap API | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [yfinance-mcp](https://github.com/narumiruna/yfinance-mcp) | Yahoo Finance data | See repo | PY | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Social Media

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Bluesky](https://github.com/keturiosakys/bluesky-context-server) | Query and search Bluesky feeds and posts | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Reddit](https://github.com/amidvidy/mcp-server-reddit) | Reddit browsing and search | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [Twitter/X](https://github.com/EnesCinr/twitter-mcp) | Twitter/X interaction | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### CMS & Publishing

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Contentful](https://github.com/ivo-toby/contentful-mcp) | Read/update/publish Contentful content | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [WordPress](https://github.com/developerdavid2/wordpress-mcp-server) | WordPress site management | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Design & Visualization

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [AntV Chart](https://github.com/antvis/mcp-server-chart) | Generate 15+ chart types | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [Figma](https://github.com/GLips/Figma-Context-MCP) | Direct Figma data access for coding agents | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [mindpilot-mcp](https://github.com/abrinsmead/mindpilot-mcp) | Visualize code/architecture as Mermaid diagrams | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Security

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [BloodHound-MCP](https://github.com/MorDavid/BloodHound-MCP-AI) | Active Directory attack path analysis | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [Conan](https://github.com/conan-io/conan-mcp) | Official — C/C++ dependency management, vulnerability scanning | See repo | PY | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [mcp-recon](https://github.com/nickpending/mcp-recon) | Domain reconnaissance and security header inspection | See repo | GO | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Maps & Location

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Google Maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) | Official — Google Maps places, directions, geocoding | `npx @modelcontextprotocol/server-google-maps` | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Science & Research

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [arXiv API](https://github.com/prashalruchiranga/arxiv-mcp-server) | Interact with arXiv API for papers | See repo | PY | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [arxiv-latex-mcp](https://github.com/takashiishida/arxiv-latex-mcp) | Fetch arXiv LaTeX sources for precise math | See repo | PY | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

### Media & Entertainment

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [Ableton Live](https://github.com/Simon-Kansara/ableton-live-mcp-server) | Control Ableton Live music production | See repo | PY | ![Advanced](https://img.shields.io/badge/-Advanced-red) |
| [Audius](https://github.com/glassBead-tc/audius-mcp-atris) | Stream music, interact with fans on Audius | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |
| [YouTube](https://github.com/nicobailey/mcp-youtube) | YouTube video data and transcripts | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Translation & Language

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [DeepL](https://github.com/nicobailey/mcp-deepl) | DeepL translation API | See repo | TS | ![Medium](https://img.shields.io/badge/-Medium-yellow) |

### Other Tools

| Server | Description | Install | Lang | Difficulty |
|--------|------------|---------|------|------------|
| [filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | Official — local file read/write with security boundaries | `npx @modelcontextprotocol/server-filesystem` | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [time-node-mcp](https://github.com/davidan90/time-node-mcp) | Timezone-aware date and time operations | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |
| [website-downloader](https://github.com/pskill9/website-downloader) | Download entire websites using wget | See repo | TS | ![Easy](https://img.shields.io/badge/-Easy-brightgreen) |

---

## :computer: MCP Clients

### Major Clients

| Client | Type | Platform | Transport | MCP Support |
|--------|------|----------|-----------|-------------|
| [**Claude Desktop**](https://claude.ai/download) | Desktop App | macOS, Windows | stdio | Full (native) |
| [**Claude Code**](https://docs.anthropic.com/en/docs/claude-code) | CLI Agent | Cross-platform | stdio | Full (native) |
| [**Cursor**](https://cursor.com) | IDE | macOS, Windows, Linux | stdio | Full |
| [**Windsurf**](https://codeium.com/windsurf) | IDE | macOS, Windows, Linux | stdio | Full |
| [**Continue**](https://continue.dev) | IDE Extension | VS Code, JetBrains | stdio | Full |
| [**Cline**](https://github.com/cline/cline) | VS Code Extension | VS Code | stdio | Full |
| [**Zed**](https://zed.dev) | Editor | macOS, Linux | stdio | Growing |
| [**Roo Code**](https://github.com/roo-code/roo-code) | VS Code Extension | VS Code | stdio | Full |
| [**GitHub Copilot**](https://github.com/features/copilot) | IDE Extension | VS Code | stdio | Growing |
| [**Augment Code**](https://augmentcode.com) | IDE Extension | VS Code | stdio | Growing |
| [**Trae**](https://trae.ai) | IDE | macOS, Windows | stdio | Growing |

### Development & Testing

| Client | Type | Description |
|--------|------|-------------|
| [**MCP Inspector**](https://github.com/modelcontextprotocol/inspector) | Dev Tool | Official debugging and testing tool for MCP servers |
| [**Smithery**](https://smithery.ai) | Web Platform | MCP server registry + testing playground |
| [**Glama**](https://glama.ai) | Web Platform | MCP server directory and playground |
| [**ChatMCP**](https://github.com/daodao97/chatmcp) | Desktop App | Purpose-built MCP chat client |

---

## :rocket: Getting Started

### New to MCP? Start here:

1. **Pick a client** — [Claude Desktop](https://claude.ai/download) or [Claude Code](https://docs.anthropic.com/en/docs/claude-code) are the easiest to start with
2. **Install a server** — Start with `filesystem` (universal) or `memory` (persistent context):
   ```bash
   npx @modelcontextprotocol/server-filesystem
   ```
3. **Configure** — Add the server to your client's config file
4. **Use it** — The AI agent now has access to the server's tools

### Recommended First Servers

| If you want to... | Install this | Command |
|-------------------|-------------|---------|
| Let AI read/write files | filesystem | `npx @modelcontextprotocol/server-filesystem` |
| Let AI search the web | Brave Search | `npx @modelcontextprotocol/server-brave-search` |
| Let AI remember things | memory | `npx @modelcontextprotocol/server-memory` |
| Let AI understand your code | CodeXRay | `npx codexray` |
| Let AI use GitHub | GitHub | `npx @modelcontextprotocol/server-github` |
| Let AI browse websites | Puppeteer | `npx @modelcontextprotocol/server-puppeteer` |

### Configuration Example (Claude Desktop)

Add to `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) or `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/allowed/dir"]
    },
    "memory": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-memory"]
    },
    "brave-search": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-brave-search"],
      "env": {
        "BRAVE_API_KEY": "your-api-key-here"
      }
    }
  }
}
```

---

## :handshake: Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

- **Add a server** — Submit a [pull request](../../pulls) to the Community Directory
- **Nominate for Editor's Picks** — Open an [issue](../../issues/new?template=curated-nomination.md)
- **Report problems** — [Report broken links or outdated info](../../issues/new?template=report-issue.md)
- **Improve descriptions** — PRs welcome for better/accurate descriptions

---

## Contributors

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/NeuralRays">
        <img src="https://github.com/NeuralRays.png" width="80" style="border-radius:50%" alt="NeuralRays"/>
        <br />
        <sub><b>NeuralRays</b></sub>
      </a>
      <br />
      <sub>Creator & Curator</sub>
    </td>
  </tr>
</table>

## License

MIT

---

<p align="center">
  <a href="../../issues"><b>Report a Problem</b></a>
  &nbsp;&middot;&nbsp;
  <a href="../../issues/new?template=add-server.md"><b>Submit a Server</b></a>
  &nbsp;&middot;&nbsp;
  <a href="../../issues/new?template=curated-nomination.md"><b>Nominate for Editor's Picks</b></a>
  &nbsp;&middot;&nbsp;
  <a href="../../pulls"><b>Contribute</b></a>
</p>

<p align="center">
  If you find this useful, please consider giving it a <a href="https://github.com/NeuralRays/awesome-mcp-hub">star</a>!
</p>
