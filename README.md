# Skill System

**Operational multi-skill development system for high-quality software.**

This is not just documentation. It is the working operating system we use when building real projects together.

---

## Core Pipeline (Strict Order)

```
1. Requirements Clarifier
2. Product Impact Architect
3. Domain Specialist(s)
4. Principal Code Review
5. Final Code Auditor
6. Release Gate
```

Orchestration is handled by the Workflow Orchestrator layer.

No stage is skipped on serious projects.

---

## How We Work Together

1. You describe the goal (even roughly).
2. We run **Requirements Clarifier** until the brief is solid.
3. **Product Impact Architect** validates whether it is worth building and how.
4. The right Domain Specialist(s) execute the build.
5. Code goes through **Principal Code Review** + **Final Code Auditor**.
6. Only after **Release Gate** is the work considered ship-ready.

GitHub is the single source of truth. All meaningful code, decisions and history live here.

---

## Repository Map

| Repository | Role |
|------------|------|
| **[skill-system](https://github.com/eSuschi/skill-system)** | This system – pipeline, checklists, standards |
| [website-starters](https://github.com/eSuschi/website-starters) | Professional websites & landing pages |
| [modular-engine](https://github.com/eSuschi/modular-engine) | Advanced modular 2D engine |
| [ai-meeting-buddy](https://github.com/eSuschi/ai-meeting-buddy) | Local AI presentation co-pilot |
| [app-boilerplates](https://github.com/eSuschi/app-boilerplates) | Application & system starters |
| [project-templates](https://github.com/eSuschi/project-templates) | Shared CI, templates, conventions |

---

## Quick Start for a New Project

1. Create a new repository (or use an existing domain one).
2. Copy the relevant checklist from `/checklists`.
3. Follow the stages in order.
4. Use the handoff templates when moving between stages.
5. Nothing ships without passing Release Gate.

Detailed operating procedures live in the `/pipeline` and `/checklists` folders.
