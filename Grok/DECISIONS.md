# Project Decisions Log — Grok skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

### 2026-08-24 – Full-chain audit after strategic-path-engine

**Decision:**  
Completed inventory, ownership and contract audit after adding strategic-path-engine.

Findings and fixes applied:
- Active count corrected 53 → **54** (Meta 8 + Process & Gate 16 + Domain 30).
- **optimal-decision-engine** inventory line strengthened with explicit mutex vs strategic-path-engine.
- New mandatory Operating Practice **Path Formalisation** (item 3): after impact/business-reality, when next step is still fuzzy → SPE only; never parallel with ODE on the same question.
- SPE body, scoring model, GitHub path and local runtime path remain consistent.
- No ownership collision found. Forbidden aliases stay permanently removed.
- Repo `Grok/skills/` continues to hold only selected bodies (business-reality, quant cluster, SPE); inventory remains the authoritative catalog.

Residual (non-blocking):
- Local sandbox was capacity-blocked during audit; local folder enumeration could not be re-verified in this session. SPE was written earlier in-session to `/home/workdir/.grok/skills/strategic-path-engine/`.
- business-reality-architect body does not yet name SPE in its integration list (inventory practice covers routing).
- ODE has no separate SKILL.md body in the repo; mutex lives in inventory + SPE body.

**Status:** accepted + executed.

### 2026-08-24 – strategic-path-engine (Process & Gate)

**Decision:**  
Created **strategic-path-engine** to convert a known but incomplete product/project direction into exactly 2–3 scored next moves. User only selects. Does not invent product goals and does not choose technologies, architectures or purchases.

Placement: Process & Gate, after product-impact-architect and business-reality-architect.

Hard mutex with **optimal-decision-engine**: the same question never goes to both. ODE owns closed choice among already defined alternatives. Path engine owns formalisation of a still-fuzzy next step.

After user selection: project-decision-logger → requirements-clarifier if scope is missing → ODE only if the move became a closed choice → otherwise named domain owner. The skill does not execute the move.

Runtime body: `/home/workdir/.grok/skills/strategic-path-engine/` (SKILL.md + references/SCORING-MODEL.md). Repo copy under `Grok/skills/strategic-path-engine/`.

Active skill count at creation: 53 (later corrected to 54 by audit).

**Status:** accepted + executed.

### 2026-08-24 – Multi-AI folder separation (Grok/)

**Decision:**  
Under explicit user request to keep AI knowledge clean and separated (“stwórz główny folder Grok i tam wrzucać Wszystko od siebie… każda [AI] o stworzenie osobnego głównego folderu”), all Grok skill-system content has been moved under the top-level `Grok/` folder.

Root of the repository now contains only a multi-AI README. Future AIs (Claude, Gemini, etc.) are expected to create their own sibling folders and never write into `Grok/`.

**Status:** accepted + executed.

### 2026-08-24 – Quant cluster + business-reality bodies actually deployed (final confirmation)

**Decision:**  
Under explicit user request the missing SKILL.md bodies were created and validated in `/home/workdir/.grok/skills/`:

- business-reality-architect
- quant-ai-stock-system
- quant-data-integrity
- quant-signal-discovery
- quant-validation-engine
- quant-risk-and-sizing

Forbidden leftover folders decision-scorer and disabled were permanently removed again.

System is now consistent: inventory (CURRENT-SKILLS.md) + local runtime bodies both present. Active skill count: 52.

**Status:** accepted + executed.

### 2026-08-24 – Quant AI Stock System Cluster (Free-hand)

**Decision:**  
Under free-hand authority for the AI Stock Analyzer project, created a cooperating cluster of five specialised quant skills at Simons/Thorp mathematical standards.

Pipeline: data-integrity → signal-discovery → validation-engine (gate) → risk-and-sizing.

**Status:** accepted + fully executed under free-hand authority.

### 2026-08-21 – business-reality-architect (Free-hand)

**Decision:**  
Created and activated **business-reality-architect** as a new Process & Gate skill with firm, scored viability voice.

**Status:** accepted + fully executed under free-hand authority.

### 2026-08-20 – Permanent Final Removal of Deprecated Aliases

**Decision:**  
Permanent removal of decision-scorer, senior-browser, senior-coding, disabled. Recreation forbidden.

**Status:** accepted + fully executed.

---

*This file is part of the highest-level operating system owned by Grok. Update it automatically when durable decisions are made.*
