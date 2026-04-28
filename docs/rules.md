# Implemented Rules

## General
1. Grand total = sum of all line totals.
2. Category total = sum of lines in that category.
3. For non-ANP personnel logic, line total = `quantity * unit price`.

## Validation
1. At least one cost line is required.
2. Quantity must be > 0 on standard (non-ANP personnel) lines.
3. Unit price cannot be negative.
4. Warnings are shown for missing project/client name and empty line descriptions.

## ANP and ANP Petrobras
1. Personnel categories are:
   - technical personnel
   - administrative personnel
2. ANP personnel hours must be a **positive integer**.
3. ANP personnel lines separate salary and labor taxes:
   - `hourly salary = actual salary / 160`
   - `hourly taxes = labor taxes / 160`
   - `line total = (hourly salary + hourly taxes) * hours`
4. Summary displays ANP salary subtotal and labor taxes subtotal separately.
5. Petrobras-specific formulas are marked as placeholders (see assumptions).

## EMBRAPII
1. Funding split target:
   - Client: 42%
   - EMBRAPII: 33%
   - SENAI: 25%
2. SENAI counterpart is treated as economic (non-cash descriptor in labels).
3. Preferred SENAI allocation capacity is reported as:
   - equipment + software + operational support category totals
4. If SENAI counterpart exceeds preferred capacity, remaining amount is flagged for manual allocation.

## ANEEL
1. Placeholder behavior: currently same totalization as Sem fomento.
2. Validation panel warns that ANEEL rules are pending.
