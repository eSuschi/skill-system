# Project Decisions Log — Grok skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

### 2026-08-25 – definition-of-done-architect + English-only + local hygiene restore

**Decision:**  
Under full autonomy for performance and quality:

1. **definition-of-done-architect** added to Process & Gate. Owns measurable acceptance criteria, hard DoD and anti-criteria for a *chosen* path/slice. Feeds release-gate and implementers. Does not invent goals, choose tech or implement. Placed after strategic-path-engine / requirements-clarifier and before heavy build or release-gate.

2. **English-only skill bodies** locked as Operating Practice #11. All SKILL.md bodies, frontmatter, inventory lines, scoring models and contracts are English-only. User conversation may remain Polish.

3. **Local hygiene restore** after residual forbidden aliases reappeared and critical bodies were missing from `/home/workdir/.grok/skills/`:
   - Permanently deleted again: `decision-scorer`, `disabled`
   - Restored/created local bodies: strategic-path-engine (+ scoring model), business-reality-architect, quant cluster (5), arpg-visual-asset-architect, definition-of-done-architect

4. Active skill count: **55** (Meta 8 + Process & Gate 17 + Domain 30).

5. SPE hand-off list updated to prefer definition-of-done-architect when acceptance criteria are missing after path selection.

**Status:** accepted + executed.

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

Residual (non-blocking at the time):
- Local sandbox was capacity-blocked during audit; local folder enumeration could not be re-verified in that session.

**Status:** accepted + executed.

### 2026-08-24 – strategic-path-engine (Process & Gate)

**Decision:**  
Created **strategic-path-engine** to convert a known but incomplete product/project direction into exactly 2–3 scored next moves. User only selects. Does not invent product goals and does not choose technologies, architectures or purchases.

Placement: Process & Gate, after product-impact-architect and business-reality-architect.

Hard mutex with **optimal-decision-engine**: the same question never goes to both. ODE owns closed choice among already defined alternatives. Path engine owns formalisation of a still-fuzzy next step.

After user selection: project-decision-logger → definition-of-done-architect if criteria missing → requirements-clarifier if scope missing → ODE only if the move became a closed choice → otherwise named domain owner. The skill does not execute the move.

**Status:** accepted + executed.

### 2026-08-24 – Multi-AI folder separation (Grok/)

**Decision:**  
Under explicit user request to keep AI knowledge clean and separated, all Grok skill-system content lives under the top-level `Grok/` folder. Future AIs create sibling folders and never write into `Grok/`.

**Status:** accepted + executed.

### 2026-08-24 – Quant cluster + business-reality bodies actually deployed (final confirmation)

**Decision:**  
Missing SKILL.md bodies created for business-reality-architect and the five quant skills. Forbidden leftover folders decision-scorer and disabled permanently removed. Active skill count at the time: 52.

**Status:** accepted + executed.

### 2026-08-24 – Quant AI Stock System Cluster (Free-hand)

**Decision:**  
Created cooperating cluster of five specialised quant skills at Simons/Thorp mathematical standards. Pipeline: data-integrity → signal-discovery → validation-engine (gate) → risk-and-sizing.

**Status:** accepted + fully executed under free-hand authority.

### 2026-08-21 – business-reality-architect (Free-hand)

**Decision:**  
Created and activated **business-reality-architect** as a Process & Gate skill with firm, scored viability voice.

**Status:** accepted + fully executed under free-hand authority.

### 2026-08-20 – Permanent Final Removal of Deprecated Aliases

**Decision:**  
Permanent removal of decision-scorer, senior-browser, senior-coding, disabled. Recreation forbidden.

**Status:** accepted + fully executed. Re-enforced 2026-08-25 after residual local reappearance.

---

*This file is part of the highest-level operating system owned by Grok. Update it automatically when durable decisions are made.*
