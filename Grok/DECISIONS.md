# Project Decisions Log — Grok skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

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
