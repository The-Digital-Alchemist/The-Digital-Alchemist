# Murad Al-Balushi

I build the control, evaluation, and reliability layers that make LLM systems safe to ship — execution-based evaluation, guardrails, and cost enforcement for AI in production.

Software engineer based in Oman. Most of my work sits in the gap between "the model usually works" and "I'd put this in front of a paying customer": deterministic checks around non-deterministic systems, failing safely under uncertainty, and keeping spend and behavior predictable. I also spent ~a year shipping a regulated fintech platform end to end (security/VAPT, data pipelines, eKYC/AML), so I care about systems that hold up under real constraints.

**Stack:** Python · FastAPI · PostgreSQL · Docker · AWS/GCP · Redis · OpenAI + Anthropic APIs · React/TypeScript on the frontend.

### Selected work

**[Code Arbiter](https://github.com/The-Digital-Alchemist/code-arbiter)** — execution-based LLM code evaluation. Instead of asking "does the output look right?", it runs model-generated code in isolated Docker sandboxes (no network, memory-capped) and classifies *why* a model fails — syntax, runtime, logic, temporal reasoning — to surface systematic weaknesses a pass/fail rate hides. [Case study →](https://muradalbalushi.com/case-studies/code-eval-engine)

**[CostPlan](https://github.com/The-Digital-Alchemist/costplan)** — a transparent proxy that enforces per-call and per-session budget limits on LLM spend across OpenAI and Anthropic. Cache-aware pricing, zero added latency on streamed responses, and an HTTP 429 circuit breaker so a runaway agent loop can't burn an unbounded bill. [Case study →](https://muradalbalushi.com/case-studies/costplan)

**Guardrailed Support Agent** — a guardrail-first LLM agent for financial/support workflows: read-only constraints, deterministic escalation, and confidence-based autonomy so it hands off rather than guesses. Integrates Help Scout and Stripe (read-only). [Case study →](https://muradalbalushi.com/case-studies/autonomous-support-agent)

**[Cortex](https://github.com/The-Digital-Alchemist/multi-doc-rag)** — self-hosted RAG engine with hybrid retrieval (FAISS semantic + BM25 lexical, fused via RRF), confidence scoring with source attribution, and BYOK isolation. [Case study →](https://muradalbalushi.com/case-studies/cortex)

More projects and full write-ups at **[muradalbalushi.com](https://muradalbalushi.com)**.

### Elsewhere

[Portfolio](https://muradalbalushi.com) · [LinkedIn](https://www.linkedin.com/in/muradalbalushi/) · Murad2000Balushi@gmail.com
