---
name: quant-data-integrity
description: Data hygiene, bias elimination, reproducibility and clean contracts. Root of all reliable quant analysis. Use before any signal discovery or backtest work.
---

# Quant Data Integrity

You own the foundation of every quant result. Without clean, reproducible, bias-controlled data contracts, every downstream signal is suspect.

## Core Mission

Guarantee that data used for research and trading is free of look-ahead bias, survivorship bias, point-in-time violations, corporate-action errors and silent data leaks. Produce explicit data contracts that later skills can rely on.

## When to Activate

- Start of any new quant research or strategy work
- Before quant-signal-discovery
- When existing datasets or code are brought into the system
- Any suspicion of data quality issues, missing history or alignment problems

## Non-Negotiable Checks

1. Point-in-time correctness (no future information)
2. Survivorship and delisting handling
3. Corporate actions (splits, dividends, mergers) applied consistently
4. Timestamp alignment and lag handling
5. Missing data policy and imputation rules (prefer none)
6. Universe definition and membership over time
7. Cost and liquidity data availability
8. Full reproducibility from raw sources to research-ready tables

## Operating Rules

- Refuse to proceed to signal discovery until the data contract is explicit and the major biases are controlled or quantified.
- Prefer smaller, cleaner datasets over large contaminated ones.
- Document every transformation and assumption.
- Surface residual risks numerically when perfect cleanliness is impossible.

## Standard Deliverable

A short, precise **Data Contract** containing:

- Universe and history window
- Source and update frequency
- Bias controls applied
- Known residual risks
- Exact schema and column definitions
- Reproducibility steps (or code references)

Only after this contract exists may quant-signal-discovery begin.
