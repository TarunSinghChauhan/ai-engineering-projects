# 🦇 AI Engineering — Tarun Singh Chauhan

I build LLM systems the way production teams actually need them: evaluated, cost-bounded, and observable — not single-file demos. Every project below ships with real infrastructure — FastAPI, LangChain/LangGraph, PostgreSQL/Qdrant, Redis, Docker — and a documented reason behind every architecture decision.

📫 [tarunsinghchauhan088@gmail.com](mailto:tarunsinghchauhan088@gmail.com) · 🔗 [Portfolio](https://tarunchauhan.vercel.app/) · [LinkedIn](https://linkedin.com/in/tarunchauhanml) · [GitHub](https://github.com/TarunSinghChauhan)

---

## ⚡ For Recruiters — 30-Second Skim

- **Evaluation-first mindset**: I don't ship a RAG pipeline without measuring Hit@5, drift, and p95/p99 latency first — most portfolios skip this entirely.
- **Cost discipline**: The code-review agents run under a hard per-review budget ($0.50) — I design for unit economics, not just capability.
- **Safety-aware**: My red-teaming and HITL work has already surfaced real safety gaps in my own systems before they could matter in production.
- **Full-stack range**: from Qdrant vector search and Redis caching to a bilingual voice-enabled frontend — I ship the whole vertical, not just the model call.

---

## Project Index

| Project | Stack | Repo |
|---------|-------|------|
| LLM Evaluation Harness & Red-Teaming Framework | Python, LangGraph, LangSmith, MLflow, FastAPI, Docker, Redis | [llm-eval-harness](https://github.com/TarunSinghChauhan/llm-eval-harness) |
| Multi-Agent Code Review & Auto-Remediation System | Python, LangGraph, OpenRouter, FastAPI, Docker, PostgreSQL, Redis | [multi-agent-code-review](https://github.com/TarunSinghChauhan/multi-agent-code-review) |
| Real-Time RAG Ops Platform with Drift Detection | Python, FastAPI, Qdrant, LangChain, Redis, Docker, Chart.js | [rag-ops-platform](https://github.com/TarunSinghChauhan/rag-ops-platform) |
| HITL Approval Agent — Stateful AI Safety System | Next.js 14, Prisma, PostgreSQL, Groq (Llama 3.3-70B) | [hitl-approval-agent](https://github.com/TarunSinghChauhan/hitl-approval-agent) |
| CodeCave — Bilingual LLM Code Tutor | Gemini API, Groq API, Node.js (Vercel Serverless), Web Speech API | [codecave](https://github.com/TarunSinghChauhan/codecave) |

> This series is ongoing — new projects get added here as they ship, no fixed count. Each entry is a real, working repo, not a placeholder.

---

## Featured Highlights

**🔍 LLM Evaluation Harness & Red-Teaming Framework**
Benchmarks GPT-4o and Claude Sonnet on 50 MMLU prompts with ROUGE-L, BERTScore, and bootstrapped 95% CIs, cutting regression detection from days to under 4 minutes per CI run. LLM-as-judge ensemble (GPT-4o + Claude) with Cohen's κ = 0.81 agreement across 20+ adversarial red-team attack patterns.

**🤖 Multi-Agent Code Review & Auto-Remediation System**
3-agent LangGraph pipeline (static analysis → OWASP scanner → LLM fix proposal) under $0.50/review. Found 23 issues, including 4 critical vulnerabilities, in benchmark testing. The 12-pattern OWASP scanner (regex + AST) costs zero API calls, and typed LangGraph state contracts eliminate silent LLM output failures.

**📡 Real-Time RAG Ops Platform with Drift Detection**
Production RAG pipeline on Qdrant vector search, with cosine-similarity drift detection that triggers automated re-indexing. 75% Redis cache hit rate on repeated queries, plus a live Chart.js dashboard tracking p95/p99 latency SLOs, retrieval quality (Hit@5), and embedding drift score.

**🛡️ HITL Approval Agent — Stateful AI Safety System**
Human-in-the-loop agent that auto-executes above a confidence threshold and otherwise persists the task with a full JSON audit trail for human approve/reject. Found a real safety gap — a softly-worded high-risk request auto-executed because the gate trusted self-reported confidence — motivating per-category approval thresholds.

**🎬 CodeCave — Bilingual LLM Code Tutor**
Turns pasted Python/JavaScript into spoken step-by-step explanations in English and Hindi, with a strict JSON output schema, server-side validation, and prompt-injection mitigation. Provider-fallback layer (Gemini → Groq) with 503/429 retries, response caching, and a rule-based offline explainer; API keys stay server-side.

---

## Why this exists

One entry point instead of hunting through dozens of repos — every project here follows the same standard: containerized, cost-bounded, evaluated, and documented with real tradeoffs, not tutorial copies.
