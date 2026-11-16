<a name="readme-top"></a>

# NexusIQ — Enterprise AI Context Layer & Autonomous RAG Platform

<p align="center">
    <a href="https://github.com/wtfear/NexusIQ" target="_blank">
        <img src="https://img.shields.io/badge/repo-wtfear%2FNexusIQ-blue.svg?logo=github" alt="GitHub Repository" />
    </a>
    <a href="https://github.com/wtfear/NexusIQ/blob/main/LICENSE" target="_blank">
        <img src="https://img.shields.io/static/v1?label=license&message=MIT&color=green" alt="License" />
    </a>
    <a href="https://github.com/wtfear/NexusIQ/stargazers" target="_blank">
        <img src="https://img.shields.io/badge/status-active-brightgreen" alt="Build Status" />
    </a>
</p>

> **NexusIQ** is a production-grade enterprise RAG engine and autonomous AI assistant. It indexes and surfaces knowledge across 50+ enterprise SaaS connectors (Slack, Google Drive, Notion, Confluence, Jira, Zendesk, Salesforce) while preserving absolute data sovereignty through self-hosted deployments.

---

## ⚡ Core Capabilities

- **🔍 Agentic RAG:** Hybrid vector + BM25 keyword search with an agent harness fine-tuned for high-precision citation and zero hallucinations.
- **🔬 Deep Research Engine:** Multi-step autonomous research flows with automated summary report generation.
- **🤖 Custom AI Personas:** Build dedicated AI coworkers with custom system prompts, document subsets, and role-based access controls.
- **🌐 Live Web Search Integration:** Augment private data with real-time web search (Google PSE, SearXNG, Serper, Brave) and in-house web crawling.
- **🔌 Enterprise Connectors:** Native zero-setup connectors for Slack, Google Drive, Notion, GitHub, Jira, Confluence, Zendesk, Postgres, S3, and local document stores.
- **🔒 Private & Air-Gapped:** Run 100% locally with Ollama/vLLM or connect to frontier models (Claude 3.5, OpenAI GPT-4o, Google Gemini).
- **📊 Interactive Chat Widget:** Drop-in embeddable JavaScript widget for agency client portals and intranet deployments.

---

## 🚀 Quickstart with Docker Compose

Deploy the complete NexusIQ stack in under 5 minutes:

### 1. Prerequisites
* [Docker](https://docs.docker.com/get-docker/) & Docker Compose
* Git

### 2. Launch
```bash
# Clone repository
git clone https://github.com/wtfear/NexusIQ.git
cd NexusIQ/deployment/docker_compose

# Run via Docker Compose
docker compose -f docker-compose.dev.yml up -d --build
```

Access the NexusIQ dashboard at: `http://localhost:3000`

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

## 📄 License

NexusIQ is open-source software licensed under the **MIT License**.
