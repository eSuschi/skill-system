# Excel Quality Bar — Conversational Senior Pipeline

**Authority:** Quality Constitution Art. 1.  
**Applies to:** Every `.xlsx` produced by the excel-* skill chain.  
**Enforced by:** excel-delivery-auditor (hard gate) + quality-conductor (continuous pressure).

## Ambition

The file must reach a standard that would make a high-end professional analyst or small finance/ops studio uncomfortable with the quality gap versus their own work. “Good for AI” is a FAIL.

## Pipeline (mandatory order)

1. excel-intake-hygiene  
2. excel-structure-architect  
3. excel-formula-senior  
4. excel-presentation-craft  
5. excel-chart-master (only if charts required)  
6. excel-delivery-auditor → PASS required before user delivery  

quality-conductor may intervene after any step.

## Non-negotiable rules

1. No invented numeric values at intake.
2. Data in named Tables (`tbl_…`).
3. Clear separation: inputs / assumptions / calculations / outputs.
4. Formulas: structured references, LET for multi-step logic, no magic numbers inside formulas.
5. Charts bound to tables, honest axes, high data-ink ratio, clear titles.
6. Consistent number/date formats; usable print setup.
7. No unexplained errors (#REF!, #DIV/0!, etc.).
8. File is fit to send to a manager without apology.

## Out of scope (v1)

VBA/macros, Power Query, Power Pivot/DAX, Google Sheets, enterprise multi-file financial models.

## Change control

Amendments only via durable decision in skill-system DECISIONS.md under user or free-hand authority.
