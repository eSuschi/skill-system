---
name: strategic-path-engine
description: Translates incomplete or intuitive product/project direction into exactly 2-3 scored next strategic moves so the user only selects. Activate when direction is known but the next step is not formalised, after product-impact-architect or business-reality-architect when the path is still fuzzy, or on explicit what-now / path-formalisation requests. Do not activate for a closed choice among already defined alternatives (that is optimal-decision-engine). Does not invent new product goals and does not choose technologies, architectures or purchases.
metadata:
  author: eSuschi
  short-description: 2-3 scored next strategic moves from a known direction
  layer: process-gate
  version: "1.0"
user-invocable: true
---

# Strategic Path Engine

Take a high-level, incomplete or intuitively felt direction and convert it into a small set of concrete, scored next moves. The user only chooses. Do not execute the chosen move.

## Do not activate

- The question is already a closed choice among defined alternatives → hand to `optimal-decision-engine` only.
- The product goal itself is missing or contested → `product-impact-architect`.
- The question is viability, cost or opportunity cost → `business-reality-architect`.
- A missing requirement would change scope or architecture → `requirements-clarifier`.

Hard mutex: never send the same question to this skill and `optimal-decision-engine` at the same time.

## Ownership

| Skill | Owns | Does not own |
|---|---|---|
| product-impact-architect | goal, ICP, value prop, impact thesis | next operational move |
| business-reality-architect | viability, cost, opportunity cost | choice of "what now" |
| strategic-path-engine | sequencing a known direction into 2-3 moves | new product goal; tech/arch/purchase choice |
| requirements-clarifier | missing requirement that changes scope | strategy |
| optimal-decision-engine | choice among already defined options | translating intuition into a path |
| project-decision-logger | durable record of the selected decision | scoring options |
| system-engine | routing and precedence | domain content |

## Core rules

1. Accept incomplete input. Do not demand perfect articulation.
2. Return exactly 2 or 3 options. Never more.
3. Score every option with explicit integers 0-100 using `references/SCORING-MODEL.md`.
4. Rank by Composite. If `|Composite_A − Composite_B| ≤ 4`, prefer higher Deliverability; if still tied, prefer higher Direction Alignment.
5. Do not present an option with Composite < 45 unless no better alternative exists. Flag it if you must.
6. Short, high-signal language. No fluff.
7. After the user selects, hand off. Do not execute the move yourself.
8. Never expand scope or invent a new product goal.

## Risk field in output

In the score line, `Risk` is the **inverted** score used in the composite (`100 − raw_risk`). Higher Risk in the printed line is better (more reversible). If you mention raw risk, label it `raw_risk` separately.

## Output format

**Strategic Path Options**

**Option A — [short title]**
One-sentence description of the concrete next move.
Scores: Alignment XX | Impact XX | Deliverability XX | Risk XX | Clarity XX | Business XX | **Composite XX**
Why this move: 1-2 tight sentences of pure logic.

**Option B — [short title]**
Same structure.

**Option C — [short title]** (optional)
Same structure.

**Recommendation**
One sentence: preferred option + one-line reason.

**Immediate next action if selected**
Exact hand-off only. Allowed targets: `requirements-clarifier`, `product-impact-architect`, `business-reality-architect`, `optimal-decision-engine`, `project-decision-logger`, or a named implementation owner. Never "do everything".

## After the user selects

1. Log the durable decision with `project-decision-logger`.
2. If a scope/architecture requirement is missing → `requirements-clarifier`.
3. If the move has become a closed choice among defined alternatives → `optimal-decision-engine`.
4. Otherwise hand to the named domain owner in the selected option.

## Scoring

Load `references/SCORING-MODEL.md` before scoring. Do not improvise weights.
