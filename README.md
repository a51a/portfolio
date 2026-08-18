# Sergei Mikhaltsov — AI Automation Portfolio

Belfast, UK · mikhaltsov@outlook.com · [linkedin.com/in/mikhaltsov](https://www.linkedin.com/in/mikhaltsov/)

Selected AI projects I've designed, built and shipped. Everything here follows the same rule: measure the baseline, automate, prove the result.

---

## 1. Financial report validation — days of manual checking → minutes

**Pain.** Every quarter, a grants programme validated partner financial reports by hand: cross-checking expense registers against dozens of supporting PDF documents. Days of manual effort per cycle, error-prone, unloved by everyone.

**Solution.** An OCR + LLM pipeline that reads supporting documents, matches them line-by-line against the expense register and flags mismatches for human review. Rolled out controls-first: written baseline, shadow-run against human decisions, go-live only after hitting the quality gate.

**Stack.** OCR, LLM document analysis, low-code orchestration (n8n), cloud storage APIs.

**Result.** −50% manual effort across the quarterly cycle; validation that took days now takes minutes per report, with humans reviewing only flagged lines.

## 2. Multi-agent research — mapping where an AI assistant needs live routing

**Pain.** A voice-assistant service needed to route users asking about serious health conditions (stroke, dementia, cancer and other heavy diagnoses) to verified support organisations. But nobody knew *where* routing was actually needed versus where the assistant already answered well — and manual review of thousands of real user queries wasn't feasible.

**Solution.** A multi-agent LLM pipeline I designed and ran with a colleague: agents classified real user queries across six health topics into "navigational" (needs live, local, up-to-date data) versus "reference" (stable knowledge), while independent fact-checking agents graded answer reliability on a 0–5 scale with web verification. Human review focused only on disagreements and edge cases.

**Stack.** Multi-agent LLM orchestration, query taxonomy design, independent LLM-as-judge evaluation with web-grounded fact-checking.

**Result.** The analysis showed routing demand varies dramatically by topic — from marginal to dominant — which turned a "roll it out everywhere" plan into a targeted rollout where navigation demand is real. The methodology was documented and is reusable for any answer-quality evaluation.

## 3. AI enablement — external programme and internal adoption

**Pain.** Teams around me — nonprofit partners outside, colleagues inside — wanted to use AI but didn't know where to start.

**Solution & results, external:** a full enablement programme built from user research (survey of 44 organisations): 13-session hands-on AI sprints for 66 nonprofit organisations (146 applications), curated and fact-checked prompt libraries, a practical AI guide (88k+ views) and a co-produced online course (567k+ views). Partner-trainer model so the programme scales beyond me.

**Solution & results, internal:** regular internal sessions on applied AI; hands-on training for colleagues on Claude Code and agentic workflows; built custom skills and automations that colleagues now run themselves — adoption measured by tools actually used, not attendance.

**Stack.** Curriculum design, workshops, prompt engineering, train-the-trainer, Claude Code / agent skills.

## 4. Grant application processing — 30–60 minutes per case → minutes

**Pain.** Each incoming grant application needed 30–60 minutes of manual eligibility checks before a decision.

**Solution.** An LLM-based checker that runs the eligibility rules and drafts the response; shipped with a strict quality gate — automated responses went live only after the system matched human decisions with 90% no-edit accuracy on a large case sample.

**Stack.** LLM pipelines, ticketing/CRM integration, structured prompts with fact-checking.

**Result.** Checks reduced to minutes per case; the team reviews exceptions instead of processing every application by hand.

---

## How I measure

Every project above used the same benefits methodology: **hours saved → FTE equivalent → money saved**, with a written baseline before automation and adoption tracked after launch. If it can't be measured, it doesn't ship.

*Full CV and references available on request.*
