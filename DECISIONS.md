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

### 2026-08-15 – Complete Domain Hardener Chain (Life Apps)
**Decision:** Add **life-app-hardener** as the missing post-generation hardener for life-improving mobile apps. Update workflow-orchestrator to sequence principal-life-app-architect → life-app-hardener. Update CURRENT-SKILLS.md inventory.

**Rationale:** 
- The builder → hardener pattern was already proven on websites, Meeting Buddy/Office companions and engines. Life apps were the remaining major domain without an equivalent real-world hardening layer.
- Generated life apps risk remaining at "demo / simulator" quality (weak offline, incomplete recovery, accessibility gaps, daily friction) unless a focused hardener systematically closes those gaps before release-gate.
- Keeping the hardener narrowly scoped preserves the clean separation already established for the other domain hardeners.

**Consequences / constraints:** 
- Life-app pipeline is now consistent with the rest of the system: architect → implement → domain hardener → auditor → release-gate.
- Active skill count rises to 26.
- workflow-orchestrator must continue to keep sequencing accurate.
- Future domain hardeners should follow the same narrow, high-signal pattern.

**Status:** accepted

---

*This file is part of the highest-level operating system. Update it automatically when durable decisions are made.*
