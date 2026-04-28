# Assumptions and Open Questions

## Safe placeholders currently implemented
1. **ANP Petrobras formula placeholder:** Until Petrobras-specific labor-cost formula is confirmed, ANP Petrobras uses the same personnel base formula as ANP and emits a warning.
2. **Academic-title pricing placeholder:** Academic title is captured per line, but no price multiplier is applied yet because the rule table is not confirmed.
3. **ANEEL placeholder:** ANEEL mode currently behaves like Sem fomento (single-source totalization) with a warning.
4. **ANP hour base assumption:** ANP personnel monthly salary conversion currently uses `160 hours/month` as a temporary conversion factor.
5. **EMBRAPII SENAI allocation:** Tool reports preferred allocation capacity and unmet remainder but does not auto-redistribute remaining SENAI counterpart to avoid guessing prioritization rules.

## Questions for user
1. What is the exact **Petrobras-specific ANP labor-cost formula**?
2. What is the official **academic-title pricing logic** (table and multipliers) for ANP Petrobras?
3. Confirm or replace the temporary `160 hours/month` conversion for ANP salary/taxes.
4. For EMBRAPII SENAI counterpart, what is the exact fallback allocation order when preferred categories are insufficient?
5. What are the official ANEEL funding and calculation rules?
6. Should indirects have any funding-mode-specific caps or formulas?
7. Should any categories be prohibited or mandatory per funding mode?
