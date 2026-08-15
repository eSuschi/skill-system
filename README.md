# Skill System

**Operational multi-skill development system for high-quality software.**

This is not just documentation. It is the working operating system we use when building real projects together.

GitHub is the single source of truth. All meaningful decisions, architecture and history live here.

**Core operating principle (highest level):**  
Skills activate automatically based on intent. The user never needs to ask Grok to "run skill X" or "check GitHub". Grok selects the correct specialists, sequences the pipeline, and uses external sources (GitHub, web, etc.) proactively.

---

## Highest-Level Operating Practices (mandatory)

1. **Automatic Impact Filter** – product-impact-architect runs early on almost every non-trivial idea.
2. **Project Decision Log** – multi-session or architecturally significant projects maintain a short `DECISIONS.md` (see `/templates/DECISIONS.md`). Only durable decisions are recorded.
3. **Light Retrospective** – after Release Gate, capture 1–3 short lessons. Improve the system when patterns appear.
4. **Skill Hygiene** – keep the skill inventory clean. This file + CURRENT-SKILLS.md are authoritative.
5. **Energy Allocation** – autonomy exists to free attention for deeper thinking, higher quality ambition and better product decisions.

---

## Core Pipeline (Strict Order)

```
1. Requirements Clarifier
2. Product Impact Architect
3. Domain Specialist(s) + matching Hardener
4. Principal Code Review
5. Final Code Auditor
6. Release Gate
```

Orchestration is handled by the **Workflow Orchestrator**. Domain hardeners (conversion, life-app, live-presentation, engine-ai-native) are sequenced automatically where applicable.

No stage is skipped on serious projects.

---

## Domain Specialists (Current Highest-Level Set)

### Product & Impact
- **product-impact-architect** – first-principles evaluation, go/no-go, high-leverage product definition
- **principal-life-app-architect** + **life-app-hardener** – life-improving mobile apps with real daily-use hardening

### Websites & Studio
- **advanced-website-expert** / **business-site-studio** + **conversion-website-auditor**

### Software Engineering
- **senior-software-engineer** – full lifecycle, architecture, production-ready implementation
- **principal-code-review** – rigorous adversarial review (correctness, races, leaks, contracts)
- **final-code-auditor** – post-build full-system defect scan + language purity
- **release-gate** – mandatory final ship-ready barrier

### Desktop & Office
- **ai-meeting-buddy-builder** / **microsoft-office-companion-builder** + **live-presentation-hardener**
- **microsoft-office-word-expert** – professional document engineering
- **live-presentation-orchestrator** – hands-free presentation sessions on large screens

### Engines & Games
- **principal-engine-architect** + **engine-ai-native-layer**
- **browser-game-expert** – complete playable browser games (shareable by URL)

### Other High-Precision
- **ai-opportunity-hunter** – opportunity discovery + Skill Factory with quality gate
- **ai-problem-investigator** – rigorous root-cause analysis
- **imagine-prompt-specialist** – cinematic / high-quality Grok Imagine prompt engineering
- **machine-fault-logger** – specific offline-first repair session tracker
- **requirements-clarifier** – mandatory front-end clarification before creation
- **workflow-orchestrator** – multi-skill pipeline conductor
- **project-decision-logger** – durable decision continuity

---

## How We Work Together

1. You describe the goal (even roughly).
2. Grok automatically activates **Requirements Clarifier** if needed.
3. **Product Impact Architect** validates whether it is worth building and how.
4. The right Domain Specialist(s) + matching hardener are selected and executed automatically.
5. Code goes through **Principal Code Review** + **Final Code Auditor**.
6. Only after **Release Gate** is the work considered ship-ready.

You should never need to request "use skill X" or "check the skill system". That is handled at the highest professional level.

---

## Repository Map

| Repository | Role |
|------------|------|
| **[skill-system](https://github.com/eSuschi/skill-system)** | This system – pipeline, checklists, standards, decision templates |
| [website-starters](https://github.com/eSuschi/website-starters) | Professional websites & landing pages |
| [modular-engine](https://github.com/eSuschi/modular-engine) | Advanced modular 2D engine foundation |
| [sable-engine](https://github.com/eSuschi/sable-engine) | Advanced Modular 2D Engine + Studio |
| [ai-meeting-buddy](https://github.com/eSuschi/ai-meeting-buddy) | Local AI presentation co-pilot |
| [app-boilerplates](https://github.com/eSuschi/app-boilerplates) | Application & system starters |
| [project-templates](https://github.com/eSuschi/project-templates) | Shared CI, templates, conventions |

---

## Quick Start for a New Project

1. Create a new repository (or use an existing domain one).
2. Copy the relevant checklist from `/checklists`.
3. Copy `/templates/DECISIONS.md` if the project will span sessions or have lasting architecture decisions.
4. Follow the stages in order.
5. Nothing ships without passing Release Gate.

Detailed operating procedures live in the `/pipeline` and `/checklists` folders.

*Maintained at the highest operational level. Skills, tools and external sources activate automatically. Decision logs preserve context across sessions.*
