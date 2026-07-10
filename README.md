<!-- Profile README · lives in the repo named mlabenski/mlabenski -->

<div align="center">

# Hey, I'm Profile viewer 👋

**Cloud & security engineer building AI into the tools people actually use every day.**

*I spent years hardening infrastructure and certifying payment systems where failure isn't an option — now I bring that same rigor to shipping production LLM applications.*

<br/>

[![💬 Send me a message](https://img.shields.io/badge/💬_Send_me_a_message-direct_line-4FD6C4?style=for-the-badge&labelColor=0B1220)](https://mlabenski.github.io/chat/)

</div>

---

## 🏊 Now building — [swimpractices.com](https://swimpractices.com)

An AI swim-practice generator that coaches actually rely on. Not a demo — a production GenAI system:

- **Schema-guided prompting → structured JSON output**, holding **100% valid JSON across thousands of generations**
- **RAG pipeline** grounding every practice in real coaching methodology
- **Token-cost optimization** so the economics work at scale, not just in a notebook
- **Firestore** as the live data layer, **AWS** underneath

```mermaid
flowchart LR
    U[Coach] --> W[Web app]
    W --> P[Prompt layer<br/>schema-guided]
    P --> L[LLM]
    R[(RAG store<br/>coaching corpus)] --> P
    L --> V{JSON<br/>validator}
    V -->|valid| F[(Firestore)]
    V -->|retry| P
    F --> W
```

The interesting problem wasn't getting an LLM to write a swim practice — it was getting it to do so *reliably*, in a strict schema, thousands of times in a row, at a cost that makes sense. That's the difference between a prototype and a product.

---

## 💳 Payments-grade engineering

Before AI, I worked in one of the least forgiving corners of software: **card payment systems**.

- Completed **chip-card payment kernel certifications (EMV-family)** — the formal, test-lab-verified process behind every tap and dip at a terminal
- Working fluency in **financial messaging standards used by authorization networks (ISO 8583-class protocols)** — the binary, field-by-field messages that move money in milliseconds
- The lasting lesson: **specs are contracts.** Every bit is accounted for, every failure mode is defined, and "it usually works" is not a passing grade

That mindset — schema discipline, exhaustive validation, defensive defaults — is exactly what production LLM systems need. It's why my generators emit valid JSON every time.

---

## 🧭 The through-line

| | | |
|---|---|---|
| **2020** | Data + instinct | Built predictive models (Python/scikit-learn) as a student — and flagged a security gap in a public-facing system along the way. Analysis and privacy hygiene, from day one. |
| **2021** | Infrastructure | Designed and hardened AWS network architecture: OpenVPN, subnet segmentation, ACLs — enterprise-grade security at a $12–22/month budget. Constraints breed good architecture. |
| **Now** | Production AI | LLM application engineering: structured outputs, RAG, cost-aware design, Firestore/AWS backends. Security-first habits applied to a brand-new stack. |

---

## 💬 Talk to me

This profile has its own **self-hosted message line** — a static page on GitHub Pages wired to a serverless backend (swappable between Firestore and AWS Lambda, because of course it is).

**[→ Open the direct line](https://mlabenski.github.io/chat/)**

Messages land straight in my inbox. No forms-as-a-service, no trackers.

<div align="center">
<sub>⚡ This README is a living build — the chat backend architecture is documented <a href="https://github.com/mlabenski/chat">in its own repo</a>.</sub>
</div>
