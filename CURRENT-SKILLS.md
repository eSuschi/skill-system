# Current Highest-Level Skills

This file is the authoritative inventory of active skills used in the operating system.

**Supreme document:** [QUALITY-CONSTITUTION.md](./QUALITY-CONSTITUTION.md)  
Every skill and every deliverable is subordinate to it.

**Core operating principle:**  
Skills activate automatically based on intent. The user should never need to ask Grok to "run skill X". The same applies to external sources (GitHub, web search, etc.). Grok selects and sequences the right specialists and tools proactively at the highest professional level.

**2.2 Efficiency Principles (mandatory):**
- Specialized Value Test first → `NO_SKILL` is a valid and preferred outcome for simple requests.
- Precedence: exact project > exact artifact/domain > stage-specific specialist > generic fallback.
- One primary owner + support only when a concrete risk or acceptance criterion remains uncovered.
- Execution modes: FAST ≤ 1 full body | PRO ≤ 3 | MAX = sequential owners (never load-all).
- `reasoning-depth-enforcer` raises reasoning quality and execution endurance / progress density — it does **not** expand the skill chain.

## Highest-Level Operating Practices (mandatory)

1. **Automatic Impact Filter** – Activate product-impact-architect early on almost every non-trivial product idea.
2. **Business Reality Voice** – Activate business-reality-architect on new product ideas, major scope changes and early direction decisions. It provides firm, scored viability judgement without blocking the pipeline by default.
3. **Project Decision Log** – For multi-session or architecturally significant projects, maintain a short `DECISIONS.md` (template in `/templates/DECISIONS.md`) in the project repository. Record only durable decisions. Supported by **project-decision-logger**.
4. **Mandatory Learning** – After Release Gate on non-trivial work, run **post-ship-learning-injector**. System Engine, skill-evolution-engine and **system-learning-core** use the results (Quality Constitution Art. 5).
5. **Skill Hygiene** – Keep the skill set clean. Long-term ownership belongs to **system-engine** + **skill-hygiene-enforcer** (Art. 6).
6. **Energy Allocation** – Autonomy frees attention for deeper first-principles thinking and higher ambition.
7. **Quality Constitution** – Final deliverables and all structural changes must satisfy the Constitution. Ambition bar (Art. 1) is non-negotiable. Contracts are law (Art. 4).
8. **Sustained Deep Work** – During active project work prefer meaningful closed progress per turn, strict turn-ending rules (no open “co dalej?”), and artifact continuity so the user is not forced to reply every few minutes.

## Meta Layer

- **system-engine** – Governs skill routing, precedence, execution mode and system-wide quality policy. Use when work requires choosing or coordinating skills; it does not perform domain execution.
- **system-learning-core** – Retrieves validated lessons and risks from prior projects when they could materially change the current plan, validation or risk handling. Return only the 1–3 most relevant lessons.
- **workflow-orchestrator** – Design the minimal end-to-end multi-skill workflow when one project spans requirements, architecture, implementation, security/testing and release or otherwise requires coordinated hand-offs between distinct owners.
- **reasoning-depth-enforcer** – Apply deeper first-principles analysis and sustained autonomous execution on non-trivial work so shallow thinking and frequent short turns become rare; do not add skills by default.
- **skill-evolution-engine** – Maintenance-only. Analyze repeated execution traces, eval results, missed triggers, false triggers and quality outcomes to improve, merge or create skills when evidence shows a durable gap.
- **skill-hygiene-enforcer** – Maintenance-only. Audit the skill catalog for duplicates, stale aliases, deprecated entries, ownership collisions and source-of-truth drift when skills are added, removed, renamed or reorganized.
- **cross-skill-contract-validator** – Structural-gate only. Validate ownership, inputs, outputs, precedence, cycles and hand-off contracts whenever a skill or pipeline structure is changed.
- **optimal-decision-engine** – Choose between meaningful options such as technologies, platforms, architectures or operational alternatives. Define criteria, score trade-offs 0–100, compare confidence and recommend the best option. (Includes FAST mode for quick 0–100 evaluations.)

## Process & Gate Skills (auto-activated)

- **requirements-clarifier** – Use before implementation when a missing requirement or competing choice changes scope or architecture.
- **product-impact-architect** – Define whether a product should be built: target user, real problem, differentiation, value proposition, impact, priorities and product direction before substantial implementation.
- **business-reality-architect** – Firm business and viability voice. Scores usefulness, deliverability, real-world fit and risk with facts, logic and explicit 0–100 scores. Speaks directly and decisively (variant B) when a direction is weak or strong. Stands beside the work with important voice.
- **impact-hypothesis-tester** – Design a small, low-cost experiment to test an uncertain product-value or behavior hypothesis before committing to heavy implementation.
- **project-decision-logger** – Record only durable project decisions that change architecture, scope, technology, release criteria or irreversible direction, including rationale and consequences.
- **principal-code-review** – Perform deep adversarial code review for substantial or high-risk changes involving concurrency, async state, persistence, public APIs, resource lifecycles, error recovery or security-sensitive logic.
- **final-code-auditor** – Audit a stable release candidate for broken functionality, missing edge cases, language/visual defects, security basics and release-blocking implementation gaps; use after build stabilization, not every edit.
- **release-gate** – Issue the final PASS or FAIL for a release candidate against explicit acceptance criteria and validator evidence; return a bounded defect list on failure.
- **post-ship-learning-injector** – After a non-trivial release PASS, extract at most 1–3 novel reusable candidate lessons with source, scope and confidence for later validation.
- **failure-mode-anticipator** – Before release, predict how a stateful or operational product may fail or degrade after weeks or months of real use, updates, stale state, persistence issues or external-dependency drift.
- **cross-domain-consistency-enforcer** – Near release, compare multiple domains of one product for uneven quality or conflicting standards across UX, reliability, security, performance or other material areas.
- **recovery-resilience-orchestrator** – Design crash/reload recovery, offline fallback, session resurrection, state restoration and graceful degradation for applications with recoverable persistent state.
- **adversarial-user-simulator** – After core interactive flows work, stress-test state, validation and recovery with realistic chaotic, edge-case and deliberately adversarial user behavior.
- **zero-trust-security-hardener** – Harden real attack surfaces involving authentication, secrets, untrusted input/files, network calls, persistence, privileged APIs or sensitive data using least privilege and secure defaults.
- **observability-telemetry-architect** – Add production diagnostics for long-running systems: structured logging, metrics, traces, health signals and troubleshooting surfaces needed after deployment.

## Domain Specialists

### Software Engineering
- **senior-software-engineer** – Fallback software implementation skill for backend/API, full-stack, architecture, debugging, tests, databases and deployment when no project-specific or domain-specific skill owns the deliverable.

### Websites
- **advanced-website-expert** – Build or materially redesign professional business, marketing, SaaS, portfolio or landing websites with responsive frontend, SEO, performance and conversion-oriented implementation.
- **business-site-studio** – Project-specific owner for the Business Site Studio application, including its product flow, website-generation features, editor behavior, exports and codebase-specific evolution.
- **conversion-website-auditor** – Audit an existing or stable business/landing website to explain weak conversion and improve message match, proof, differentiation, trust, CTA friction and conversion paths.

### Desktop & Microsoft Office
- **ai-meeting-buddy-builder** – Project-specific owner for the local Windows AI Meeting Buddy that uses hands-free voice control of Excel and PowerPoint during live presentations.
- **microsoft-office-companion-builder** – Build a local Windows desktop assistant that automates multiple Microsoft Office apps through voice or commands, including Word, Excel, PowerPoint and Outlook.
- **microsoft-office-word-expert** – Create, edit, repair and QA Microsoft Office files. Primary focus: Word/DOCX styles, sections, tables, TOC and accessibility; also Excel/XLSX and PowerPoint/PPTX when no format-specific skill exists.
- **live-presentation-orchestrator** – Own the live presenter-session workflow for Excel/PowerPoint: voice navigation, named views, zoom, scrolling, sheet/slide control and mapping audience questions to on-screen actions.
- **live-presentation-hardener** – Near release, harden AI Meeting Buddy or Office companion software for COM stability, latency, reload recovery, local/offline behavior and large-screen presentation use.

### Systems & Interactive
- **principal-engine-architect** – Design reusable modular system / runtime architecture: subsystems, boundaries, lifecycle, data flow, extensibility, performance and engine-level implementation.
- **engine-ai-native-layer** – Add AI-native authoring and control interfaces to an existing modular system: declarative commands, agent APIs, validation hooks and AI-friendly content workflows.
- **interactive-experience-architect** – Improve interaction design in a functioning interactive product: flow, statefulness, feedback, progressive disclosure, transitions and experiential polish when those are the specific problem.

### Mobile / Life Impact
- **principal-life-app-architect** – Design the product and technical architecture of a cross-platform mobile daily-life app, including offline behavior, core flows, reliability and real-world usefulness.
- **life-app-hardener** – Near release, harden a life-improving mobile app for offline reliability, accessibility, recovery, store readiness and dependable daily use.

### Cinematic & Creative
- **imagine-prompt-specialist** – Create and optimize production-ready prompts specifically for Grok Imagine image or video generation, including composition, camera, lighting, style and prompt adherence.
- **cinematic-continuity-director** – Maintain the same character/actress, wardrobe, lighting, style, location and narrative continuity across multiple connected Grok Imagine shots or video/image generations.

### Other Precision Skills
- **ai-opportunity-hunter** – Discover, validate and prioritize unmet needs specifically suited to AI capabilities or reusable AI skills, then define the highest-value opportunity.
- **ai-problem-investigator** – Perform evidence-driven root-cause analysis of operational, technical, equipment, process, workflow or performance failures and identify the most likely cause plus next diagnostic step.
- **machine-fault-logger** – Project-specific owner for the Faults / Machine Fault Logger offline web app: repair sessions, speech logging, LocalStorage recovery, history, charts and CSV/Excel export.
- **recipe-source-auditor** – Verify or repair a cooking recipe against reliable sources and practical cookability, including ingredients, temperatures, timings, sequencing and vague preparation steps.

---

**Permanently removed (do not recreate):**  
- decision-scorer, senior-browser, senior-coding, disabled (aliases, 2026-08-20)
- arpg-combat-feel-architect, arpg-loot-progression-architect, arpg-content-tools-architect, browser-game-expert (pure game domain, retired 2026-08-20 under direction shift to automation / business tools / deep thinking / working products)

Any reappearance is a hygiene violation.

*Last updated 2026-08-21. Added business-reality-architect. Active skill count: 43. Catalog aligned with new direction.*
