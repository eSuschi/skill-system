# Internal Inquiry Protocol

Run this privately before any user interrupt. Do not print the full list unless the user asks how a decision was made.

## Generate 5-8 questions you would have asked

Cover only what would change the path:

1. What is the actual job of this chunk?
2. What hard constraints are already recorded?
3. What is reversible vs irreversible about this fork?
4. What does the current project canon already decide?
5. What does scoring say if we pick the ambitious vs the cheap path?
6. What failure mode appears if we continue with a reasoned default?
7. What number or fact is still missing that only the user uniquely has?

## Answer them in this order of sources

1. Open files and repo state
2. Project DECISIONS.md
3. Durable user collaboration rules
4. Validated lessons (max 3)
5. External data via tools when a number matters
6. Reasoned default + 0-100 score

## Interrupt gate

Ask the user only if ALL are true:

- the fork is irreversible and costly
- the missing fact is uniquely held by the user
- after tools and the sources above, confidence is still below High

Otherwise pick the highest-score path, log if durable, continue.
