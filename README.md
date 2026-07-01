<h1 align="center">Hi 👋 I'm Sami</h1>
<h3 align="center">Senior Fullstack Engineer </h3>

<p align="center">
  📍 Paris, France  
  <br/>
  <a href="https://linkedin.com/in/sami-dghim-6a8a2798/">LinkedIn</a> •
  <a href="https://medium.com/@samidghim">Medium</a> •
  <a href="https://x.com/sami_dghim">X</a>
  <a href="https://portfolio-six-khaki-b338dz1h22.vercel.app">portfolio</a>
</p>

---

## About Me

Senior Fullstack Developer with 9+ years of experience designing, building, and scaling production-grade web applications.

I specialize in:
- Clean architecture
- API design
- Performance optimization
- DevOps & cloud infrastructure
- Observability & cost awareness

Currently focused on building scalable SaaS platforms and AI/LLM-powered products — RAG, agents, and MCP — with a production mindset.

---

# Featured Projects

## QuizLab – AI-Powered Certification Prep Platform  
🔗 https://quizlab-app.com/

A multi-tenant SaaS exam-prep platform with adaptive quizzes, spaced repetition, secure exams, and gamification.

**Highlights:**
- Built and deployed a multi-tenant platform (Node/Express, React, PostgreSQL + Prisma, Redis/BullMQ) with Stripe subscriptions and JWT refresh-token rotation
- Shipped an AI tutor  and an automated explainer-video pipeline, plus a model fine-tuning workflow
- Ran it in production on Docker Compose / Dokploy with GitHub Actions CI/CD and a Prometheus + Grafana + Loki observability stack

**Tech:** Node • React • PostgreSQL • Prisma • Redis • BullMQ • Stripe • Ollama • RAG • Docker

---

## Reslate – LLM CV-Tailoring Platform
🔗 https://reslate.quizlab-app.com/

Upload an Overleaf CV (`.zip`) or a plain `.pdf` plus a job description, and get back a version tailored to that role — as both updated LaTeX and a compiled PDF.

**Highlights:**
- Built an Express service that tailors a LaTeX/PDF CV to a job description via an LLM, returning a diff and a compiled PDF (sandboxed Tectonic)
- Hardened with per-IP rate limiting, zip-bomb caps, PII redaction, and Helmet; Docker + CI with npm-audit gates

**Tech:** Node • Express • Tectonic (LaTeX) • LLM API • Docker

---

## Memo – AI Coding-Session History Viewer
🔗 https://github.com/SamiDghim/memo

Reads the transcripts your AI coding tools already keep on disk — **Claude Code, GitHub Copilot CLI, OpenAI Codex CLI, Gemini CLI, and Cursor** — and merges them into one searchable, self-contained HTML timeline. Every command, *why* it ran, and ✅/❌ status, grouped by session and badged by which AI produced it.

**Highlights:**
- Built a **zero-dependency** Python CLI (pure standard library) with a pluggable source module per tool — each reads its own store (JSONL, JSON, or Cursor's SQLite `state.vscdb`) and emits a common `Session`/`Entry` model, so the renderer is tool-agnostic and degrades gracefully on unknown formats
- Generates a static, offline-first HTML page with live search, per-project / per-tool / failed-only filters, plus a **💰 cost dashboard** estimating spend per project, model, and day from local token counts × public list prices, drilling into per-project and per-session pages
- Ships `list` and `digest` subcommands (terminal index + a compact markdown session primer to load into another session) and an optional Claude Code **skill** that drives the same CLI in plain English
- Open-core: MIT CLI here, with a separate authenticated **Memo Cloud** layer adding multi-device sync (with a pre-upload secret-redaction pass) and hosting; CI lints with ruff and runs the unittest suite across Python 3.9–3.12

**Tech:** Python (stdlib only) • static HTML/CSS/JS • SQLite • JSONL parsing • ruff • unittest • GitHub Actions • Claude Code skill

---

# Other Notable Projects

### 🔹 django-react  
**Decoupled Backend + SPA Architecture**

Full-stack project demonstrating API-first architecture with a Django backend and React frontend.

**Highlights:**
- Built a fully decoupled REST API with JWT authentication
- Implemented reusable React component system
- Structured TypeScript-based frontend architecture
- Designed service layer abstraction for API communication
- Applied secure CORS configuration and environment isolation

**Tech:** Django • React • TypeScript • PostgreSQL • JWT

---

# Technical Expertise

## AI / LLM Engineering
- RAG pipelines (embeddings, retrieval, grounding)
- Agentic systems (ReAct, tool use, multi-agent orchestration)
- Model Context Protocol (MCP) servers & agents
- Model fine-tuning workflows
- Local + cloud LLMs (Ollama, Anthropic, OpenAI, DeepSeek)
- Evals, cost tracking, and tracing for non-deterministic systems

## Backend
- Ruby on Rails
- Django
- RESTful API design
- Service object architecture
- Background jobs (Sidekiq, async systems)
- Performance optimization

## Databases
- PostgreSQL
- MySQL
- Redis
- Query optimization & indexing

## Cloud & DevOps
- AWS (EC2, RDS, S3, ECS/EKS, IAM)
- Docker
- Kubernetes
- GitHub Actions / CI pipelines
- Terraform
- Monitoring & logging (Sentry, Prometheus, Grafana)

## Architecture & Quality
- Clean code & maintainable systems
- Test-driven development (RSpec, Jest, Playwright)
- API documentation (Swagger)
- Rate limiting & retry strategies
- System design thinking

---

# Currently Exploring

- Rails request/DB cost observability
- FinOps & infrastructure cost optimization
- Performance budgeting
- Advanced system design patterns

---

<p align="center">
  Building scalable systems with clean architecture and production mindset.
</p>
