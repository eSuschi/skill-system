# Quality Constitution

This document defines portable quality principles for the skill catalog. The behavioral contract is `WORKING-AGREEMENT.md`. Neither document grants authority beyond the user's request.

## 1. Fitness for Purpose

Quality is measured against the user's goal, explicit requirements, domain standards and observable acceptance criteria. Prestige language and unsupported numeric scores are not evidence.

## 2. Correctness Before Polish

Required behavior, data integrity, safety and recoverability take precedence over visual or rhetorical polish. A specialist should produce sound work at its own stage rather than depend on a later reviewer to rescue it.

## 3. Coherence

Terminology, ownership, interfaces and user-visible behavior should remain consistent across phases. Differences are defects only when they harm correctness, usability or the agreed result.

## 4. Verifiable Claims

State what was inspected, inferred, executed and verified when the distinction matters. A PASS requires relevant evidence against explicit criteria; absence of evidence is uncertainty, not success.

## 5. Proportionate Assurance

Use independent review and formal gates for consequential or explicitly gated work. Routine changes need proportionate verification, not a mandatory procession of reviewers.

## 6. Clean Contracts

New, removed or changed skills must have clear ownership, bounded triggers and resolvable handoffs. Catalog changes should be checked by `cross-skill-contract-validator` and `skill-hygiene-enforcer` before acceptance.

## 7. Learning from Outcomes

Persist lessons only when an observed result supports a reusable conclusion. Proposals to change the catalog remain proposals until the user authorizes them.

## 8. Authority and Reversibility

Prefer reversible progress under uncertainty. Ask before consequential actions outside the granted scope, and preserve the user's existing work.

Amendments require explicit user authority and a durable entry in `DECISIONS.md`.
