# 🦇 AI Engineering — Tarun Singh Chauhan

I build LLM systems the way production teams actually need them: evaluated, cost-bounded, and observable — not single-file demos. Every project below ships with real infrastructure — FastAPI, LangChain/LangGraph, PostgreSQL/Qdrant, Redis, Docker — and a documented reason behind every architecture decision.

📫 [tarunsinghchauhan088@gmail.com](mailto:tarunsinghchauhan088@gmail.com) · 🔗 [Portfolio](https://tarun-app.vercel.app) · [LinkedIn](https://linkedin.com/in/tarunchauhanml) · [GitHub](https://github.com/TarunSinghChauhan)

---

## ⚡ For Recruiters — 30-Second Skim

- **Evaluation-first mindset**: I don't ship a RAG pipeline without measuring Hit@k, drift, and latency SLOs first — most portfolios skip this entirely.
- **Cost discipline**: Every agent enforces a hard per-query LLM budget (e.g. $0.50/review, $0.50/report) — I design for unit economics, not just capability.
- **Safety-aware**: My red-teaming and HITL work has already surfaced real safety gaps in my own systems before they'd matter in production.
- **Full-stack range**: from zero-cost deterministic embeddings to animated frontend agent walkthroughs — I ship the whole vertical, not just the model call.

---

## Project Index

| Project | Stack | Repo |
|---------|-------|------|
| LLM Evaluation Harness & Red-Teaming Framework | Python, LangGraph, LangSmith, MLflow, FastAPI, Docker | [llm-eval-harness](https://github.com/TarunSinghChauhan/llm-eval-harness) |
| Multi-Agent Code Review & Auto-Remediation System | Python, LangGraph, OpenRouter, FastAPI, Docker | [multi-agent-code-review](https://github.com/TarunSinghChauhan/multi-agent-code-review) |
| Autonomous Financial Research Agent | FastAPI, OpenRouter, Yahoo Finance API, Redis | [finance-research-agent](https://github.com/TarunSinghChauhan/finance-research-agent) |
| CodePulse — AI Cinematic Code Walkthrough | Next.js 14, TypeScript, Groq (LLaMA 4), Framer Motion | [CodePulse](https://github.com/TarunSinghChauhan/CodePulse) |
| Multimodal Product Intelligence Platform | Docker, LLM Pipelines, Vector Search, Streamlit | [Multimodal-Product-Intelligence-Platform](https://github.com/TarunSinghChauhan/Multimodal-Product-Intelligence-Platform) |

> This series is ongoing — new projects get added here as they ship, no fixed count. Each entry is a real, working repo, not a placeholder.

---

## Featured Highlights

**🔍 LLM Evaluation Harness & Red-Teaming Framework**
Benchmarks GPT-4o and Claude Sonnet across MMLU prompts with ROUGE-L, BERTScore, and bootstrapped 95% CIs. LLM-as-judge ensemble with Cohen's κ = 0.81 agreement, 20+ adversarial red-team attack patterns.

**🤖 Multi-Agent Code Review & Auto-Remediation System**
3-agent LangGraph pipeline (static analysis → OWASP scanner → LLM fix proposal), cost-budgeted under $0.50/review, catches SQL injection, hardcoded secrets, insecure deserialization, and shell injection.

**📈 Autonomous Financial Research Agent**
4-step reasoning chain (Market Context → Financial Analysis → Risk Assessment → Investment Thesis), SHA-256 reproducibility hash per report, full company research in under 60 seconds.

**🎬 CodePulse — AI Cinematic Code Walkthrough**
LLaMA 4 via Groq generates structured execution traces powering an animated, line-by-line code walkthrough with voice narration and "Break Mode" AI-driven bug injection.

**🧩 Multimodal Product Intelligence Platform**
End-to-end pipeline combining embeddings, vector search, and LLM inference behind a Streamlit interface, containerized for reproducible deployment.

---

## Why this exists

One entry point instead of hunting through dozens of repos — every project here follows the same standard: containerized, cost-bounded, evaluated, and documented with real tradeoffs, not tutorial copies.
