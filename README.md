# Hi, I'm Murad 👋

### I build the control, evaluation, and reliability layers that make LLM systems safe to ship.

Most AI demos work in the happy path. My work lives in the gap between *"the model usually works"* and *"I'd put this in front of a paying customer"* — execution-based evaluation, guardrails, cost enforcement, and observability for AI systems in production. Deterministic checks wrapped around non-deterministic models, systems that fail safely under uncertainty, and spend that stays predictable.

I also spent ~a year shipping a **regulated fintech platform** end to end — security/VAPT, large-scale data pipelines, and eKYC/AML integrations — so I build for the constraints real systems actually run under, not the demo.

🌐 **[muradalbalushi.com](https://muradalbalushi.com)** &nbsp;·&nbsp; 💼 **[LinkedIn](https://www.linkedin.com/in/muradalbalushi/)** &nbsp;·&nbsp; 📧 **MuradlBalushi@gmail.com** &nbsp;·&nbsp; 📍 Oman

---

## 🚀 Featured Work

### 🔬 [Code Arbiter](https://github.com/The-Digital-Alchemist/code-arbiter) — Execution-Based LLM Code Evaluation
Most coding benchmarks ask *"does the output look right?"* — a weak question. Code Arbiter asks *"does it pass the tests, and if not, **why**?"* It runs model-generated code inside isolated Docker sandboxes (network disabled, memory-capped, torn down per run) and classifies every failure — syntax, runtime, logic, temporal reasoning, edge case, performance — to surface systematic model weaknesses a pass/fail rate completely hides. Benchmarks cloud and local models under identical conditions and emits self-contained HTML comparison reports.

> The actionable insight isn't *which* model scores higher — it's *how* each one fails. A 7B local model and a frontier model can post near-identical pass rates while failing on completely different things.

`Python` · `Docker` · `OpenAI` · `Anthropic` · `LM Studio` · `pytest`
&nbsp;&nbsp;📖 **[Read the case study →](https://muradalbalushi.com/case-studies/code-eval-engine)**

### 💰 [CostPlan](https://github.com/The-Digital-Alchemist/costplan) — LLM Cost-Enforcement Proxy
An open-source circuit breaker for autonomous-agent API spend. A transparent proxy that enforces **per-call and per-session budget limits** across OpenAI and Anthropic — point your agent at it with one env var, no code changes. Cache-aware pricing across all four Anthropic token types (so cached reads aren't billed as full input), **zero added latency** on streamed SSE responses, and an HTTP 429 circuit breaker so a runaway agent loop can't burn an unbounded bill.

> It's the `ulimit` for LLM spend — boring, invisible, and exactly what you wish you'd had the morning after an agent burned $200 overnight.

`Python` · `asyncio` · `SSE Streaming` · `HTTP Proxy` · `Anthropic` · `OpenAI`
&nbsp;&nbsp;📖 **[Read the case study →](https://muradalbalushi.com/case-studies/costplan)**

### 🛡️ [Guardrailed Support Agent](https://muradalbalushi.com/case-studies/autonomous-support-agent) — Guardrail-First Agent for Financial Workflows
A support agent designed to **fail safely**. Strict read-only constraints, deterministic escalation logic, and confidence-based autonomy — when it isn't sure, it hands off to a human instead of guessing. Integrates Help Scout and Stripe (read-only via MCP) to resolve routine inquiries autonomously and enrich operator context on escalation, reducing support load without risking unsafe billing or account actions.

`Python` · `RAG` · `Stripe MCP` · `Help Scout API` · `Gemini` · `GCP`
&nbsp;&nbsp;📖 **[Read the case study →](https://muradalbalushi.com/case-studies/autonomous-support-agent)**

### 🧠 [Cortex](https://github.com/The-Digital-Alchemist/multi-doc-rag) — Self-Hosted RAG Engine
A privacy-first knowledge engine with **hybrid retrieval** — FAISS semantic search and BM25 lexical search fused via Reciprocal Rank Fusion — plus confidence scoring with source attribution and BYOK isolation so credentials and data never leave the user's control. Multi-format document pipeline, containerized deployment.

`Python` · `FastAPI` · `FAISS` · `Next.js` · `OpenAI` · `Docker` · `AWS`
&nbsp;&nbsp;📖 **[Read the case study →](https://muradalbalushi.com/case-studies/cortex)**

### 📊 [FinAI](https://muradalbalushi.com/case-studies/finai) — Compute-First Financial Analysis
A decision-support engine that computes deterministic portfolio metrics — returns, volatility, drawdowns, allocation weights, risk concentration — **before** any LLM is involved, then constrains the model to interpreting those grounded numbers. No speculation, no hallucinated figures: the math is the source of truth, the model just explains it.

`Python` · `Portfolio Analytics` · `Constrained LLM Interpretation`
&nbsp;&nbsp;📖 **[Read the case study →](https://muradalbalushi.com/case-studies/finai)**

---

## 💼 Experience

**Software Developer — 360Remit** *(regulated fintech)* · Jan 2025 – Mar 2026
- Owned end-to-end **VAPT** as the risk authority between security vendors and engineering — cut false positives 40%+, closed 100% of critical issues pre-launch, **zero security incidents at go-live**.
- Engineered a vendor sync pipeline for **500k+ records** (delta detection, conflict resolution, bidirectional sync) that cut manual processing from **3–5 days to under 5 minutes**.
- Delivered MTO, eKYC, and AML integrations and designed phased infra (DR, capacity, data residency) to launch within regulatory deadlines.

---

## 🛠️ Tech I Work With

**Languages** &nbsp;Python · TypeScript · JavaScript · SQL

**AI / LLM** &nbsp;LLM Evaluation · Guardrails · RAG · Hybrid Retrieval (BM25 + RRF) · Cost Enforcement · OpenAI · Anthropic · MCP · Whisper

**Backend & Infra** &nbsp;FastAPI · Node.js · Docker · AWS · GCP · Redis · CI/CD · Nginx

**Data** &nbsp;PostgreSQL · MySQL · FAISS · ETL Pipelines

**Frontend** &nbsp;React · Next.js · TypeScript · Tailwind CSS

---

<sub>⚡ More projects and full write-ups at **[muradalbalushi.com](https://muradalbalushi.com)**</sub>
