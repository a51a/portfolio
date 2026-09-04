# Sergei Mikhaltsov — AI Automation Portfolio

Belfast, UK · mikhaltsov@outlook.com · [linkedin.com/in/mikhaltsov](https://www.linkedin.com/in/mikhaltsov/)

AI automation projects I designed and shipped at a major tech company, 2025–2026. Each project had a written baseline before launch, so the numbers below are measured, not estimated.

---

## 1. Financial report validation

**Pain.** A grants programme validated partner financial reports by hand every quarter: each expense register cross-checked against dozens of supporting PDF documents. Days of manual work per cycle.

**Solution.** An OCR + LLM pipeline: reads the supporting documents, matches them line-by-line against the expense register, flags mismatches for human review. Before go-live it ran in shadow mode against human decisions until it passed the quality bar.

**Stack.** OCR, LLM document analysis, low-code orchestration (n8n), cloud storage APIs.

**Result.** Manual effort down ~50% per quarter. A report now takes minutes instead of days; humans review only flagged lines.

## 2. Multi-agent evaluation of assistant answers

**Pain.** A voice-assistant service needed to decide where to route users asking about serious health conditions to verified support organisations — and where its own answers were already good enough. Thousands of real user queries; no capacity to review them manually.

**Solution.** A multi-agent LLM pipeline, built with a colleague. Classifier agents split real queries across six health topics into "navigational" (needs live, local data) vs "reference" (stable knowledge). Separate fact-checking agents scored answer reliability on a 0–5 scale with web verification. Humans reviewed only disagreements and edge cases.

**Stack.** Multi-agent orchestration, query taxonomy design, LLM-as-judge evaluation with web-grounded fact-checking.

**Result.** A reusable evaluation method — taxonomy, reliability scale, independent fact-checking — that the team used as the evidence base for rollout decisions. The product itself is confidential; the method is not.

## 3. AI enablement — external programme and internal adoption

**Pain.** Nonprofit partners and colleagues wanted to use AI and didn't know where to start.

**External.** Built the programme from a survey of 44 organisations: 13 hands-on sprint sessions for 66 nonprofits (146 applications), fact-checked prompt libraries, a practical AI guide (88k+ views), a co-produced online course (567k+ views). Partner trainers now run it without me.

**Internal.** Regular sessions on applied AI for colleagues; hands-on training on Claude Code and agent workflows; custom skills and automations that colleagues run themselves. I track adoption by tools in use, not attendance.

**Public coverage (official Yandex announcements, in Russian):** [the AI guide launch](https://yandex.ru/company/news/11-08-2025-02) · [the pilot AI training programme](https://yandex.ru/company/news/31-10-2025-02) · [the free AI course on Yandex Practicum](https://yandex.ru/company/news/22-07-2026-01)

## 4. Grant application processing

**Pain.** Every incoming grant application needed 30–60 minutes of manual eligibility checks.

**Solution.** An LLM checker that runs the eligibility rules and drafts the response. Automated responses were enabled only after the system matched human decisions with 90% no-edit accuracy on a large case sample.

**Stack.** LLM pipelines, ticketing/CRM integration, structured prompts with fact-checking.

**Result.** Minutes per case instead of 30–60; the team reviews exceptions, not every application.

---

## Method

The same measurement approach in every project: a written baseline before automation (hours per task), then hours saved → FTE equivalent → money saved. Adoption tracked after launch.

*Full CV and references available on request.*
