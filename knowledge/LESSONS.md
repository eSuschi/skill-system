# Lessons

High-signal, durable lessons extracted from real project outcomes and decisions.

Format:
```
### YYYY-MM-DD — Short title
Lesson: ...
Evidence: ...
Implication: ...
```

---

### 2026-08-18 — Catalog length and forced skill chains reduce effective quality
Lesson: Long, overlapping skill descriptions and any mechanism that forces full skill-chain activation increase token cost and dilute attention on the correct specialist. Short discriminative catalog + Specialized Value Test (NO_SKILL) + one-primary ownership + depth-without-chain produce higher quality per unit of context.
Evidence: Maximum-Efficiency Audit 2.2 + live implementation of P0 under free-hand mandate; previous reasoning-depth-enforcer language actively promoted multi-skill loading; static TF-IDF proxy improved from ~73 % to 100 % Top-1 after description shortening.
Implication: Future skill evolution and Meta Layer design must treat token density and false-positive co-activation as first-class quality risks. Prefer shorter discovery text, risk-flag activation of hardeners, and explicit “do not expand skill set” constraints on depth instruments.

### 2026-08-15 — System Learning Core introduced
Lesson: A dedicated, non-disruptive learning layer that accumulates operational memory (rather than only evolving skills) closes the gap between “we analyse after the fact” and “the system starts smarter on the next project”.
Evidence: User request for an internal AI-style skill that helps project creation and other skills; existing retrospective practices were passive or scheduled.
Implication: Future complex projects can optionally draw on accumulated patterns and risks at the start, and Release Gates now have a clear sink for durable cross-project lessons.
