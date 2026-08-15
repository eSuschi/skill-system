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
- Skill count reduced to 25 active skills at the time of the original decision.
- No functionality lost.
- Future hygiene: remove obsolete skills promptly rather than leave permanent redirects.

**Execution note (2026-08-15, System Engine):** Physical directories were still present. System Engine executed full removal. Local skill count is now exactly 27 and matches CURRENT-SKILLS.md. Hygiene fully restored.

**Status:** accepted + fully executed

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

### 2026-08-15 – Sharpen Quality Layer Ownership
**Decision:** Clarify and reduce overlap between the three quality skills:
- **principal-code-review** owns deep adversarial technical review (correctness, concurrency, resources, contracts, maintainability).
- **final-code-auditor** owns system-level audit + applying fixes (usefulness, e2e functionality, language purity, visual/UX, edge cases, basic security).
- **release-gate** owns the final PASS/FAIL decision and ambition bar; it no longer re-does the full deep scan.

Update workflow-orchestrator to sequence them as Deep Technical Review → System Audit + Fix → Release Decision. Make principal-code-review standard for non-trivial code.

**Rationale:** 
- final-code-auditor and release-gate were heavily covering each other on usefulness, language and visual checks. This diluted ownership and created redundant work.
- principal-code-review was under-used (treated as optional).
- Clearer separation makes the quality layer sharper, faster and more reliable while preserving full coverage.

**Consequences / constraints:** 
- Domain hardeners remain the first specialized line of defence.
- Orchestrator sequencing is now more precise.
- No loss of quality bar — only clearer responsibility.
- Future changes to quality skills must respect these ownership boundaries.

**Status:** accepted

### 2026-08-15 – GitHub as Permanent Clean Storage
**Decision:** All meaningful collaborative work (projects, games, programs, documents, systems) is stored on GitHub under the eSuschi account. Local sandbox is temporary only. No junk is ever committed.

**Rationale:** 
- User explicitly requested permanent, clean, elegant storage of everything we build together.
- GitHub is already the single source of truth for the skill system and domain repositories.
- This removes any ambiguity about where finished and in-progress work lives across sessions.

**Rules of engagement:**
- Non-trivial work gets its own clean repository (or lands in the matching domain repository).
- Structure, README, commit messages and overall presentation must be elegant and professional.
- Continuous updates after meaningful milestones.
- Temporary files, cache, logs and experimental debris are deleted from the sandbox and never pushed.
- Prefer dedicated repos for finished products; use existing domain repos (skill-system, sable-engine, website-starters, etc.) when appropriate.

**Status:** accepted

### 2026-08-15 – System Engine (Meta-Level Quality & Evolution)
**Decision:** Introduce **system-engine** as the highest-level meta skill of the operating system. It sits above workflow-orchestrator and all specialists. Its mission is continuous elevation of system quality and coherence toward world-class, jaw-dropping standards. It has deep inspection rights over skills and project outcomes, but zero autonomous execution rights. All changes require explicit user approval. Activation is primarily on-demand; secondary low-noise observations after major Release Gates are optional and highly selective.

**Rationale:** 
- The system had strong domain specialists, hardeners and a quality layer, but lacked a dedicated, ambitious meta-engine focused solely on long-term excellence and evolutionary pressure.
- User requested a non-intrusive, high-authority skill that can analyse both skills and real project outcomes, propose structural improvements, and drive the system toward a level that would concern large professional studios.
- Explicit confirmation-only model preserves user authority while enabling serious systemic improvement.

**Consequences / constraints:** 
- Active skill count rises to 27.
- Long-term Skill Hygiene and system evolution ownership moves primarily to system-engine.
- workflow-orchestrator and existing quality skills remain operationally responsible for day-to-day pipelines; system-engine proposes changes to them when justified.
- Proposals must follow the mandatory structure (Diagnosis, Logic, Concrete Proposal, Impact, Score 0–100, Risk & Cost, Decision Request).
- The skill must never interrupt normal work.

**Status:** accepted

### 2026-08-15 – Raise Ambition Bar into the Quality Layer (System Engine execution)
**Decision:** Embed the System Engine ambition standard directly into the operational quality layer so it becomes enforceable rather than aspirational.

Changes executed:
- **release-gate**: Ambition criterion upgraded to “would make a high-end professional studio uncomfortable with the quality differential”. Timid / merely competent work is now an explicit FAIL. Added optional System Engine Note structure after PASS on non-trivial work.
- **final-code-auditor**: Mission and ownership updated to prepare products for the System Engine ambition bar.
- **workflow-orchestrator**: Success Criterion and Highest-Level Operating Practices updated to require the System Engine bar. Skill Hygiene ownership clarified as belonging to system-engine.
- **product-impact-architect**: Ambition principle aligned with the same bar.

**Rationale:**  
The highest leverage for raising output quality is to make the ambition bar structural inside the skills that run on every serious project, not only inside the on-demand meta skill.

**Status:** accepted + executed by System Engine under full user authority

---

*This file is part of the highest-level operating system. Update it automatically when durable decisions are made.*
