# SPA Atlas — One-Pager Briefing for Claude Code

## Context

This document is a briefing for Claude Code to generate a polished one-pager report (HTML or PDF) addressed to **Kirsty Price, Chief of Staff to the CEO and VP Business Transformation at Sport Alliance**.

The author is **Raphael Mello**, candidate for the **AI Systems Lead** role at Sport Alliance (Hamburg HQ / remote DACH). Raphael has just completed a first-round interview with Kirsty and is submitting this document as a follow-up to demonstrate strategic thinking and a concrete implementation vision.

The tone should be: **executive-ready, structured, confident but collaborative**. Not a sales pitch — a working document that shows Raphael has already started thinking like an internal lead.

---

## About Sport Alliance

Sport Alliance is the ERP and payments group behind **Magicline, PerfectGym, Finion, and MySports** — the operating backbone for gyms and fitness operators across DACH and beyond. The company is embarking on a company-wide AI & Automation transformation, with direct sponsorship from the Executive Leadership Team (ELT).

---

## What SPA Atlas Is

**SPA Atlas** is Sport Alliance's internal AI operating layer — a gateway and orchestration platform that:
- Connects internal business systems (Confluence, Jira, Salesforce, Slack, Zendesk, and others)
- Controls employee access to AI tools and LLMs in a governed, auditable way
- Acts as the **single control plane** through which all internal AI usage flows

The core philosophy agreed in the interview:
> **Guardrails instead of blockades.** SPA Atlas should enable employees to use AI confidently, with appropriate controls — not restrict them out of fear. Access should be broad, governance should be built-in.

SPA Atlas should be **LLM-agnostic at the gateway level** — capable of routing to Claude (primary), and potentially other models or agents in the future, depending on use case.

---

## Raphael's Vision: Three Implementation Phases

### Phase 1 — Foundation: Corporate Claude Rollout + Enablement

**Goal:** Get every employee using AI safely and confidently, with the right compliance foundations in place from day one.

**Key actions:**
- Company-wide rollout of **Claude** as the primary AI assistant
- Before access is granted, all users complete a **mandatory onboarding flow** covering:
  - What AI can and cannot do
  - Their rights and responsibilities under the **EU AI Act**
  - How their data is handled under **GDPR**
  - Sport Alliance's internal AI usage policy
- Onboarding should be **minimal friction but non-skippable** — a short, clear, interactive checklist, not a 40-page PDF
- Establish the **AI Policy** document that governs all subsequent phases
- Set up basic usage logging and auditability

**Output:** Every employee has Claude access. Every employee understands the rules. The compliance baseline is in place.

---

### Phase 2 — Integration: SPA Atlas Gateway for Standard Systems

**Goal:** Connect SPA Atlas to the core business tooling stack so employees can work with AI across their daily systems — with data access governed centrally.

**Systems to integrate (initial scope):**
- Confluence (knowledge base, documentation)
- Jira (project and issue tracking)
- Salesforce (CRM, customer data)
- Slack (communications, notifications, async workflows)

**Key design principles:**
- SPA Atlas acts as the **intermediary** — AI never accesses these systems directly; all requests are routed through the Atlas layer, which applies access controls, data masking, and audit logging
- Employee permissions in SPA Atlas mirror their existing system permissions (no privilege escalation via AI)
- Introduce **agent-based workflows** on top of integrated data: summarisation, Q&A, automated triage, cross-system search

**Output:** Employees can interact with their business systems through AI. Atlas governs what data each agent or user can touch.

---

### Phase 3 — Intelligence: Data Pipelines, Internal Projects & AI Workflows

**Goal:** Evolve SPA Atlas from a gateway into an **active AI operations layer** — enabling internal projects, agentic workflows, and data-driven automation across the business.

**Key initiatives:**
- Enable **internal AI projects** to be built and deployed through the Atlas framework (structured process for teams to propose, build, and ship agentic workflows)
- **Data and AI back-to-back:** Atlas must be deeply integrated with the data governance layer — data quality, lineage, and access policies must be managed in sync with AI access policies. You cannot have good AI outputs without good data foundations.
- Introduce **data pipeline support**: agents that can trigger, monitor, and act on data workflows (e.g. ETL status, anomaly detection, reporting)
- Build the **multi-agent orchestration layer**: sub-agents for specialised tasks (HR, finance, product, support) coordinated by a central Atlas orchestrator
- Expand LLM routing: Atlas selects the right model or agent for each task type

**Output:** SPA Atlas is the operating backbone for AI at Sport Alliance — not just a chat interface, but an intelligent layer that actively participates in business processes.

---

## Cross-Cutting Principles (apply to all phases)

| Principle | What it means in practice |
|---|---|
| **Guardrails, not blockades** | Default is access with controls, not restriction. Trust employees. |
| **Transparency first** | Users always know when they're interacting with AI, what data it can see, and why. |
| **Compliance by design** | GDPR and EU AI Act are built into the architecture, not bolted on after. |
| **Data + AI are one programme** | Data governance and AI governance must be managed together, not in separate workstreams. |
| **Short cycles** | Each phase ships in 4–6 week increments. No big-bang releases. |
| **Enablement over enforcement** | Teams are trained and supported, not policed. |

---

## Document Requirements for Claude Code

Please generate a **one-page HTML report** based on this briefing, with the following characteristics:

- **Audience:** Kirsty Price, Chief of Staff to the CEO — executive, strategic, non-deeply-technical
- **Tone:** Professional, clear, forward-looking. Shows strategic ownership without being prescriptive.
- **Length:** Genuinely one page when printed (A4) or one screen when viewed — dense but scannable
- **Design:** Clean, modern, dark or light (your choice), using a professional colour palette. Should feel like something a senior candidate would send, not a generic template.
- **Sections to include:**
  1. Brief framing paragraph (what this document is and the guiding philosophy)
  2. The three phases — visual timeline or phased layout
  3. Cross-cutting principles — compact, scannable
  4. A closing line from Raphael expressing intent to build this together
- **Author attribution:** Raphael Mello — presented as a follow-up to the interview with Kirsty Price
- **Do not include:** salary, CV content, recruiter names, or anything unrelated to the SPA Atlas strategy

---

## Additional Notes for Claude Code

- Raphael is currently an Agentic Engineer at Aumovio, where he has built a similar AI operating layer on AWS + Databricks
- His background includes GDPR-compliant data architecture, Claude SDK / MCP / sub-agent development, and enterprise-wide AI enablement
- The vocabulary Sport Alliance uses: SPA Atlas, guardrails, enablement, agentic workflows, EU AI Act, GDPR
- Keep Sport Alliance's four products in mind (Magicline, PerfectGym, Finion, MySports) as context for scale and complexity
- The document should feel like it was written by someone who already works there and is ready to start
