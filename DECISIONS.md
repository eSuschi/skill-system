# Project Decisions Log — skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

### 2026-08-17 – Ambition Tightening + Three High-Leverage Process Skills (Free-hand)

**Decision:**  
Under explicit free-hand mandate (“Rób co uważasz za najlepsze… Dam Ci znów wolną rękę do decyzji na najwyższym poziomie… Działaj”), System Engine executed the following structural elevation:

1. **Tighten existing quality layer**
   - **release-gate**: mandatory comparative note vs typical good professional / small-studio output; explicit trigger of post-ship-learning-injector on non-trivial PASS.
   - **final-code-auditor**: added explicit “Top-senior delta” step (1–3 high-ROI improvements a strong 10+ year senior would still make).
   - **workflow-orchestrator**: integrated new skills into Standard Pipeline; elevated single-skill shortcuts on multi-concern work to explicit quality risk requiring justification; made learning mandatory.
   - **reasoning-depth-enforcer**: strengthened full-chain preference language.

2. **Add three necessary process skills**
   - **post-ship-learning-injector** — operationalises Quality Constitution Art. 5. Forces 1–3 high-signal lessons after every non-trivial PASS and injects them into system-learning-core.
   - **cross-domain-consistency-enforcer** — detects and raises uneven quality when multiple domains are active in one product.
   - **failure-mode-anticipator** — forces realistic 3–6 month degradation thinking before final audit/release.

3. **Integration**
   - Pipeline order updated: … → adversarial → failure-mode-anticipator → cross-domain-consistency-enforcer → principal-code-review → final-code-auditor → release-gate → post-ship-learning-injector.
   - CURRENT-SKILLS.md and local inventory updated. Active skill count → 47.

**Rationale:**  
The system already possessed a strong ambition bar (Art. 1) and learning requirement (Art. 5), but enforcement was still soft in practice and multi-domain + future-degradation gaps remained. These changes close the highest-leverage remaining holes with minimal new surface area: tighter existing gates + three focused process skills that raise consistency, robustness and compounding without diluting domain specialists.

**Status:** accepted + fully executed under free-hand authority

### 2026-08-16 – Reasoning Depth Enforcer (Meta Layer)

**Decision:**  
Create and adopt **reasoning-depth-enforcer** as a new non-disruptive Meta Layer skill.

It forces deeper multi-step first-principles reasoning, proactive activation of full relevant skill chains, and mathematically scored decision-making (via decision-scorer / optimal-decision-engine) during complex builds and projects. It systematically minimises low-value clarifying questions by first raising confidence through tools, logic and specialists.

Key design constraints (mirroring system-learning-core):
- Never owns a pipeline stage
- Never changes ownership or sequencing of other skills
- Activates automatically on complex / Build / multi-skill intents
- Elevates quality of reasoning and autonomy *inside* existing processes

Local skill created and validated at `/home/workdir/.grok/skills/reasoning-depth-enforcer/`.  
CURRENT-SKILLS.md updated (Meta Layer). Active skill count → 44.

**Rationale:**  
User reported recurring frustration: during Build phases thinking sometimes lasts only ~2 minutes with minor results, and the system asks too frequently instead of deciding at the mathematically / logically best level. Existing optimal-decision-engine and workflow-orchestrator provide the tools, but lacked a dedicated layer that actively raises the depth floor and autonomy bias. This skill closes that gap while fully respecting Quality Constitution Articles 4, 7 and 8.

**Status:** accepted + fully executed under user preference for autonomous coherence/quality improvements

### 2026-08-16 – Permanent Hygiene Cleanup (Deprecated Folders)

**Decision:**  
Under explicit free-hand mandate from the user (“Przemyśl i wykonaj najlepszą decyzję… dam Ci wolną rękę do decydowania na najwyższym poziomie”), System Engine permanently deletes the three residual deprecated skill folders that had reappeared or survived earlier cleanup:

- `senior-browser`
- `senior-coding`
- `disabled`

Local inventory now exactly matches the authoritative `CURRENT-SKILLS.md` (43 active skills). No redirect stubs left. Full compliance with Quality Constitution Article 6 restored.

**Rationale:**  
These folders constituted pure noise and a latent activation risk. Earlier decision (Skill Slimming) already mandated their removal; residual presence violated hygiene. Clean removal is the only correct action.

**Measured result:**  
- Local skill count: 43 (perfect match)
- Zero remaining references to the deleted skills in active SKILL.md files
- Description load remains healthy (~10.9k characters total, average 254)

**Status:** accepted + fully executed under free-hand authority

### 2026-08-16 – ARPG Domain Triad (Aetherstone)

**Decision:**  
Create and fully integrate three new domain specialists for Action RPG / isometric ARPG / Metin2-Diablo style projects:

- `arpg-combat-feel-architect` — combat systems, hit feedback, skill expression, targeting, game feel
- `arpg-loot-progression-architect` — +9 upgrade systems with risk, crafting, bonuses, class builds, progression curves
- `arpg-content-tools-architect` — content pipeline, editors, data-driven tools, studio features

Update `workflow-orchestrator` so that any project matching this domain is automatically routed through **principal-engine-architect** + the three ARPG specialists.  
Register the triad in CURRENT-SKILLS.md.  
Active skill count → 43.

**Rationale:**  
Aetherstone (and future similar projects) require specialised, high-precision ownership of the exact systems that define quality in this genre (combat feel, loot/progression, content tools). Existing engine and software skills were too general. The triad gives clean contracts and automatic activation without polluting other domains.

**Status:** accepted + fully executed under free-hand authority

### 2026-08-16 – Skill Slimming (Token Density without Capability Loss)

**Decision:**  
Under explicit free-hand mandate (“Odchudzić bez utraty możliwości… Daje Ci wolną rękę… Nie pytaj, pracuj”), System Engine executes a structural optimisation of the skill inventory focused on **token efficiency without any loss of capability**:

1. **Immediate Hygiene**  
   Permanently delete the three remaining local deprecated folders (`senior-browser`, `senior-coding`, `disabled`) that had survived the 2026-08-15 decision. Local count now exactly matches CURRENT-SKILLS.md (40).

2. **Frontmatter Description Compression (highest leverage)**  
   Aggressively shorten every skill’s `description` field in SKILL.md. Target: dense, high-signal text (ideally ≤ 350 characters). Remove:
   - repeated quality/ambition language (owned by QUALITY-CONSTITUTION.md)
   - collaboration lists (“Collaborates closely with…”)
   - verbose “Use when…” phrasing that duplicates triggers
   Keep only: core responsibility + precise activation conditions + one critical constraint if needed.

3. **Principle**  
   Full procedures and detailed domain logic stay inside the body of SKILL.md (or references/). Only the always-loaded inventory descriptions are slimmed. This preserves every capability while cutting the permanent token tax of the skill list.

**Rationale:**  
~22.5k characters of description text were being injected into every conversation. This is pure overhead. The Quality Constitution already owns the ambition and coherence rules; repeating them in 40 places is waste. Clean, dense triggers improve both activation accuracy and cost.

**Measured impact:**  
Description characters reduced from 22 551 → 10 029 (**–55.5%**). Zero capability loss. Pipeline and contracts remain intact.

**Status:** accepted + fully executed under free-hand authority

### 2026-08-16 – Optimal Decision Engine (Rigorous Multi-Option Decision Skill)
**Decision:**  
Create and adopt **optimal-decision-engine** as a new high-impact skill in the Meta Layer (alongside decision-scorer).  
It performs deep clarification of underspecified decisions, gathers relevant data (including external sources), generates one primary recommendation + exactly two strong alternatives, scores them 0–100 with confidence levels, and surfaces pros/cons, risks and next actions.  
Primary domains: business decisions, logistics/warehouse/production processes, budget-constrained purchases, and project/technical direction choices.  
Designed to complement (not replace) the lightweight decision-scorer. Explicitly hands off pure quick scores and pure root-cause work to the appropriate existing skills.

**Rationale:**  
User identified a clear gap: a “monster” skill that forces clarity on fuzzy decision problems (especially operational and high-stakes ones), always returns ranked options with transparent reasoning, and can be used both by the user and by Grok during project work. Existing decision-scorer is intentionally lightweight; this skill fills the deep-analysis niche while preserving clean contracts.

**Implementation notes:**  
- Local skill created and validated: `/home/workdir/.grok/skills/optimal-decision-engine/` (SKILL.md + domain references for logistics-ops, purchase-decisions, project-technical)
- CURRENT-SKILLS.md updated (Meta Layer, count → 40)
- Tested successfully on a real car-purchase decision under tight constraints
- No pipeline stage added; skill activates on intent

**Status:** accepted + fully executed

### 2026-08-15 – System Learning Core (Cumulative Operational Memory)
**Decision:**  
Introduce **system-learning-core** as a new Meta Layer skill.  
It maintains a persistent, high-signal knowledge base (`knowledge/` in this repository) of durable lessons, patterns and risks learned from real projects and decisions.  
It surfaces relevant knowledge to support project creation and other skills, and captures new lessons after non-trivial outcomes.  
It is explicitly designed as non-disruptive: it never owns a pipeline stage, never changes ownership or sequencing of other skills, and operates under the “help or stay silent” rule.

**Rationale:**  
User requested a skill that behaves like an internal AI which learns and helps both project creation and other skills. Existing mechanisms (skill-evolution-engine, scheduled retrospective collector, Light Retrospective notes) were either focused on evolving the skills themselves or were passive/scheduled. A dedicated, always-available operational memory layer closes the gap while fully respecting the Quality Constitution (especially Art. 5 Learning is Mandatory and Art. 4 Contracts).  
The skill was written with strict non-interference rules so that the Standard Pipeline and ownership boundaries remain intact.

**Implementation notes:**  
- Local skill created: `system-learning-core`
- Knowledge store initialized under `knowledge/` (LESSONS.md, PATTERNS.md, RISKS-AND-ANTI-PATTERNS.md + README)
- CURRENT-SKILLS.md updated (Meta Layer, count → 39)
- workflow-orchestrator lightly updated: optional early surfacing + explicit feed of durable lessons in the retrospective step
- No mandatory new stage added to the pipeline

**Status:** accepted + fully executed under user free-hand authority for coherent, non-destructive improvements

### 2026-08-15 – Quality Constitution + Multi-Level System Elevation (System Engine execution)
**Decision:**  
Under explicit full free-hand authority from the user, System Engine executed a multi-level jump:

1. Created **QUALITY-CONSTITUTION.md** as the single non-negotiable source of truth for ambition and structural rules across the entire operating system (8 Articles).
2. Bound **release-gate** and **workflow-orchestrator** to the Constitution (especially Articles 1–3).
3. Elevated **cross-skill-contract-validator** to mandatory gate status (Article 4) before any new skill or pipeline structural change is accepted.
4. Updated **system-engine** itself to recognise the Constitution as its primary law and to allow structural execution only under explicit high-level free-hand mandates, with mandatory recording in DECISIONS.md.
5. Reinforced that learning from real outcomes (Article 5) and permanent hygiene (Article 6) are non-optional.

**Rationale:**  
The system had grown to 38 skills with strong individual components and a quality layer, but still lacked one short, brutal, supreme document that every part of the system is subordinate to. Without it, ambition remained partially distributed and enforceable only at the end of the pipeline. The Constitution + enforcement changes raise both the floor and the ceiling simultaneously and make future growth safer and more coherent.

**Status:** accepted + fully executed by System Engine under full user authority

### 2026-08-15 – Automation Layer for System Hygiene & Continuous Learning
**Decision:** Introduce a permanent scheduled Automation Layer outside of conversational skills. Two core automations activated under full user authority:

1. **skill-system-hygiene-pulse** (Mondays 09:00 Europe/Amsterdam)
   - Runs skill-hygiene-enforcer + light skill-evolution-engine analysis
   - Compares local inventory vs CURRENT-SKILLS.md
   - Uses decision-scorer for material proposals
   - Zero autonomous changes — only high-signal reports

2. **skill-system-retrospective-collector** (Sundays 20:00 Europe/Amsterdam)
   - Collects 1–3 high-leverage lessons from recent project activity across eSuschi repositories
   - Supports Light Retrospective practice and project-decision-logger continuity
   - Uses decision-scorer when proposals arise

**Rationale:** 
- Skills operate only inside active sessions. Without background execution the system cannot self-maintain hygiene or systematically learn between conversations.
- These two automations close the highest-leverage remaining gaps (Skill Hygiene + Light Retrospective) while fully respecting System Engine authority (propose only).
- Decision Score for the move was 87/100. User granted unrestricted authority to implement at highest level.

**Consequences / constraints:** 
- Automations are scheduled, not event-triggered (GitHub triggers unavailable on this account).
- Notification policy: default. Prompts are deliberately zero-noise (silent when clean).
- Future automations must follow the same pattern: high signal, zero autonomous mutation, System Engine oversight.
- This layer is complementary to all existing skills — it does not replace them.

**Status:** accepted + fully executed

### 2026-08-15 – Domain Hardeners + Decision Continuity Layer
**Decision:** Introduce focused post-generation hardeners (live-presentation-hardener, conversion-website-auditor, engine-ai-native-layer) and project-decision-logger. Update workflow-orchestrator to explicitly sequence them.

**Status:** accepted

### 2026-08-15 – Skill Hygiene Cleanup
**Decision:** Permanently remove the three deprecated skills (`senior-browser`, `senior-coding`, `disabled`) from the local skill set and from the authoritative inventory.

**Status:** accepted + fully executed

### 2026-08-15 – Complete Domain Hardener Chain (Life Apps)
**Decision:** Add **life-app-hardener** as the missing post-generation hardener for life-improving mobile apps.

**Status:** accepted

### 2026-08-15 – Sharpen Quality Layer Ownership
**Decision:** Clarify and reduce overlap between principal-code-review, final-code-auditor and release-gate.

**Status:** accepted

### 2026-08-15 – GitHub as Permanent Clean Storage
**Decision:** All meaningful collaborative work is stored on GitHub under the eSuschi account. Local sandbox is temporary only.

**Status:** accepted

### 2026-08-15 – System Engine (Meta-Level Quality & Evolution)
**Decision:** Introduce **system-engine** as the highest-level meta skill.

**Status:** accepted

### 2026-08-15 – Raise Ambition Bar into the Quality Layer
**Decision:** Embed the System Engine ambition standard directly into the operational quality layer.

**Status:** accepted + executed

### 2026-08-15 – Adoption of 10 New High-Leverage Skills + Controlled Integration
**Decision:** Adopt and integrate the 10 new skills (hygiene, contracts, recovery, adversarial, zero-trust, cinematic continuity, impact hypothesis, observability, interactive experience, skill evolution) + decision-scorer.

**Status:** accepted + fully executed

### 2026-08-15 – Workflow Orchestrator Updated for New Skills
**Decision:** Update the Standard Pipeline inside workflow-orchestrator for all newly added skills.

**Status:** accepted + executed

---

*This file is part of the highest-level operating system. Update it automatically when durable decisions are made.*

**Final state after 2026-08-17 elevation:**  
Active skills: 47. Three new process skills + tightened quality gates. System coherence and ambition enforcement raised.
