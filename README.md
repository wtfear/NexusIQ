<p align="center">
  <img src="./public/sirius-logo.svg" alt="SiriusIQ Logo" width="320" />
</p>

<h1 align="center">SiriusIQ</h1>
<h3 align="center">Enterprise AI Context Layer & Autonomous Workplace RAG Platform</h3>

<p align="center">
  <strong>The Brightest Star of Enterprise Search, Cited Retrieval & Workplace Intelligence</strong><br />
  Production-Grade, Air-Gapped Context Engine Indexing 50+ Enterprise Connectors with Absolute Data Sovereignty
</p>

<p align="center">
  <a href="https://github.com/wtfear"><img src="https://img.shields.io/badge/Agency-WTFear-blue.svg?style=flat-square" alt="WTFear Agency" /></a>
  <a href="https://github.com/wtfear/SiriusIQ/actions"><img src="https://img.shields.io/badge/CI%2FCD-Passing-emerald.svg?style=flat-square" alt="CI/CD" /></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg?style=flat-square" alt="MIT License" /></a>
  <a href="https://nextjs.org"><img src="https://img.shields.io/badge/Next.js-15-black.svg?style=flat-square" alt="Next.js" /></a>
  <a href="https://fastapi.tiangolo.com"><img src="https://img.shields.io/badge/FastAPI-0.115-009688.svg?style=flat-square" alt="FastAPI" /></a>
  <a href="https://vespa.ai"><img src="https://img.shields.io/badge/Index-Vespa%20%7C%20Qdrant-FF6B6B.svg?style=flat-square" alt="Vespa" /></a>
</p>

---

## 🌟 Executive Overview

**SiriusIQ** (named after Alpha Canis Majoris, the brightest star in the entire night sky) is an enterprise-grade Autonomous RAG (Retrieval-Augmented Generation) and workplace knowledge orchestration platform. Built on **Next.js, FastAPI, Vespa/Qdrant, and PostgreSQL**, it indexes, permission-gates, and surfaces organizational intelligence across **50+ enterprise SaaS connectors** (Slack, Google Drive, Notion, Confluence, Jira, Zendesk, Salesforce) while ensuring 100% private cloud or on-premise data sovereignty.

---

## ⚡ Core Capabilities

- **🔍 Agentic RAG:** Hybrid vector + BM25 keyword search with an agent harness fine-tuned for high-precision citation and zero hallucinations.
- **🔬 Deep Research Engine:** Multi-step autonomous research flows with automated summary report generation.
- **🤖 Custom AI Personas:** Build dedicated AI coworkers with custom system prompts, document subsets, and role-based access controls.
- **🌐 Live Web Search Integration:** Augment private data with real-time web search (Google PSE, SearXNG, Serper, Brave) and in-house web crawling.
- **🔌 50+ Enterprise Connectors:** Native zero-setup connectors for Slack, Google Drive, Notion, GitHub, Jira, Confluence, Zendesk, Postgres, S3, and local document stores.
- **🔒 Private & Air-Gapped:** Run 100% locally with Ollama/vLLM or connect to frontier models (Claude 3.5, OpenAI GPT-4o, Google Gemini).
- **📊 Drop-in JavaScript Chat Widget:** Embeddable client widget for agency portals and intranet deployments.

---

## 🚀 Quickstart with Docker Compose

Deploy the complete SiriusIQ stack in under 5 minutes:

### 1. Prerequisites
* [Docker](https://docs.docker.com/get-docker/) & Docker Compose
* Git

### 2. Launch
```bash
# 1. Clone repository
git clone https://github.com/wtfear/SiriusIQ.git
cd SiriusIQ/deployment/docker_compose

# 2. Run via Docker Compose
docker compose -f docker-compose.dev.yml up -d --build
```

Access the SiriusIQ operations cockpit at: `http://localhost:3000`

---

## 🏗️ Architecture

```
                               ┌────────────────────────────────┐
                               │   Next.js Enterprise Web UI    │
                               │    (Chat, Search & Admin)      │
                               └───────────────┬────────────────┘
                                               │
                                               ▼
                               ┌────────────────────────────────┐
                               │      FastAPI Core Engine       │
                               │   (RAG Routing & Agent Logic)  │
                               └───────────────┬────────────────┘
                                               │
               ┌───────────────────────────────┼───────────────────────────────┐
               ▼                               ▼                               ▼
 ┌───────────────────────────┐   ┌───────────────────────────┐   ┌───────────────────────────┐
 │   Vespa / Qdrant Index    │   │    PostgreSQL Database    │   │     Enterprise Connectors │
 │ (Hybrid Vector + Lexical) │   │  (Users, RBAC, Metadata)  │   │   (Drive, Slack, Notion)  │
 └───────────────────────────┘   └───────────────────────────┘   └───────────────────────────┘
```

---

## 🛡️ Security & Enterprise Access Control

* **Role-Based Access Control (RBAC):** Restrict sensitive documents by team, department, or individual user credentials.
* **Air-Gap Capability:** Fully functional in disconnected on-prem environments with local embedding models and local LLM runners.
* **Audit Logging:** Enterprise-grade logs of query history, citation sources, and permission enforcement.

---

## 🌌 The WTFear Celestial Enterprise Portfolio

SiriusIQ serves as the central cognitive brain of the **WTFear Celestial AI Suite**:

| Star | Flagship Platform | Category | Stack |
|---|---|---|---|
| 🌟 **Sirius** | **`SiriusIQ`** | Enterprise Workplace Knowledge OS & RAG | Next.js, FastAPI, Vespa, PostgreSQL |
| 🌟 **Capella** | **`CapellaBI`** | BI-as-Code & Unit Economics Cockpit | DuckDB-WASM, Svelte, SQL |
| 🌟 **Polaris** | **`PolarisERP`** | Autonomous Enterprise ERP, CRM & WMS | Next.js 15, PostgreSQL, TurboRepo |
| 🌟 **Aldebaran** | **`AldebaranCRM`** | Enterprise Sales Pipeline & Quotation CRM | Laravel, Vue.js, MySQL |
| 🌟 **Altair** | **`AltairCommerce`** | Headless B2B/D2C Commerce Engine | Laravel 11/12, Vue.js, MySQL |
| 🌟 **Vega** | **`VegaDocs`** | Air-Gapped Document Intelligence & RAG | React, Node.js, Vector DBs |

---

## 📄 License & Attribution

- **Core License:** [MIT License](./LICENSE) — 100% Free for commercial, agency, and enterprise client white-label deployments.
- **Upstream Engine:** Built on the battle-tested [Onyx](https://github.com/onyx-dot-app/onyx) enterprise core (formerly Danswer).
- **Maintained & Enhanced by:** [WTFear Agency](https://github.com/wtfear) & **Pavan Kumar Kunukuntla**.
