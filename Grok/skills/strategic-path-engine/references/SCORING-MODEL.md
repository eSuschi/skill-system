# Strategic Path Engine – Scoring Model

All scores are integers 0-100.
Higher is always better except raw risk, which is inverted before weighting.

## Dimension definitions

**Direction Alignment**
How precisely the proposed next move advances the stated or implied direction without drift.
100 = perfect continuation, zero reinterpretation.
0 = contradicts or ignores the direction.

**Strategic Impact**
Expected reduction of uncertainty or advancement of the critical path in the next 1-3 cycles.
100 = unlocks major progress or removes a key bottleneck.
0 = cosmetic or low-leverage.

**Deliverability**
Feasibility given current knowledge, skills, time and existing assets.
100 = can be executed immediately with high confidence.
0 = requires major new discovery or resources.

**Risk / Irreversibility**
`raw_risk` = probability and cost of being wrong or locking the project into a bad path.
Inverted for scoring and for the printed `Risk` field:
`Risk_score = 100 - raw_risk`
100 after invert = almost reversible, low downside.
0 after invert = high chance of a costly dead-end.

**Clarity & Actionability**
How unambiguous and immediately executable the move is.
100 = anyone reading it knows exactly what to do next.
0 = still vague or requires further clarification.

**Business Contribution**
Contribution to real usefulness, viability or reduction of opportunity cost (aligned with business-reality-architect).
100 = clearly strengthens the overall viability case.
0 = neutral or dilutes it.

## Weights (sum = 1.00)

| Dimension | Weight |
|---|---|
| Direction Alignment | 0.28 |
| Strategic Impact | 0.22 |
| Deliverability | 0.18 |
| Risk (inverted) | 0.12 |
| Clarity & Actionability | 0.12 |
| Business Contribution | 0.08 |

## Composite

Composite =
0.28 × Alignment +
0.22 × Impact +
0.18 × Deliverability +
0.12 × (100 − raw_risk) +
0.12 × Clarity +
0.08 × Business

Round to nearest integer.

## Ranking

1. Primary sort: Composite descending.
2. If |Composite_A − Composite_B| ≤ 4 → prefer higher Deliverability.
3. If still tied → prefer higher Direction Alignment.
4. Never present Composite < 45 unless no better alternatives exist (then flag it).
