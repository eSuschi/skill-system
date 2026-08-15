# Project Decisions Log — skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

### 2026-08-15 – Domain Hardeners + Decision Continuity Layer
**Decision:** Introduce focused post-generation hardeners (live-presentation-hardener, conversion-website-auditor, engine-ai-native-layer) and project-decision-logger. Update workflow-orchestrator to explicitly sequence them.

**Rationale:** 
- Generated Meeting Buddy / Office companions and AI websites frequently reached "demo quality" but not reliable production quality under real conditions (latency, COM, conversion, AI control).
- Decision context was being lost between sessions, weakening multi-skill continuity.
- Hardeners are complementary to final-code-auditor / release-gate (domain-specific vs general).

**Consequences / constraints:** 
- Pipeline for Meeting Buddy, business websites and modular engines is now longer but higher quality.
- workflow-orchestrator must keep the sequencing up to date.
- New skills must remain narrowly scoped; do not let them absorb general responsibilities.

**Status:** accepted

### 2026-08-15 – Skill Hygiene Cleanup
**Decision:** Permanently remove the three deprecated skills (`senior-browser`, `senior-coding`, `disabled`) from the local skill set and from the authoritative inventory.

**Rationale:** 
- They had already been marked as deprecated and redirected.
- Leaving them in the Skills tab created unnecessary noise and potential confusion.
- Active complementary chains (builders → hardeners) remain intact and do not conflict.
- Cleaner inventory improves long-term maintainability and automatic activation accuracy.

**Consequences / constraints:** 
- Skill count reduced to 25 active skills.
- No functionality lost.
- Future hygiene: remove obsolete skills promptly rather than leave permanent redirects.

**Status:** accepted

---

*This file is part of the highest-level operating system. Update it automatically when durable decisions are made.*
