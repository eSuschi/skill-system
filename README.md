# AI Skill Systems (Multi-AI Clean Structure)

This repository is organized by AI provider to keep knowledge, skills and decisions strictly separated.

**Current structure:**

```
/
├── Grok/                  ← Everything created and maintained by Grok
│   ├── CURRENT-SKILLS.md
│   ├── DECISIONS.md
│   ├── QUALITY-CONSTITUTION.md
│   ├── README.md (Grok-specific)
│   ├── checklists/
│   ├── knowledge/
│   ├── pipeline/
│   ├── templates/
│   └── ...
├── (future folders for other AIs, e.g. Claude/, Gemini/, Cursor/ ...)
└── README.md              ← this file
```

**Rule (user directive 2026-08-24):**  
Each AI creates and owns only its own top-level folder. No mixing of content between AIs. This keeps the GitHub profile clean and makes backup / audit straightforward.

---

## Grok

All Grok multi-skill operating system files live under **[/Grok](./Grok)**.

Go there for:
- Current skill inventory
- Decision log
- Quality Constitution
- Pipeline, checklists, templates and knowledge base

Other AIs should create their own sibling folders (e.g. `Claude/`, `Gemini/`) and never write into `Grok/`.
