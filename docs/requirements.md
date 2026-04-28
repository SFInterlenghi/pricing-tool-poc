# Requirements

## Business context
Unify three pricing spreadsheets into one browser application:
1. General Firjan project pricing
2. ANP labor breakdown
3. EMBRAPII pricing summary

## Funding modes
- Sem fomento
- EMBRAPII
- ANP
- ANP Petrobras
- ANEEL (placeholder until rules are confirmed)

## Functional requirements
- Single browser page (`index.html`), no backend.
- User inputs project metadata.
- User adds/removes cost lines by category:
  - technical personnel
  - administrative personnel
  - travel
  - software
  - equipment
  - consumables
  - third party services
  - indirects
  - operational support
- User selects funding mode.
- Tool calculates totals by category.
- Tool calculates totals by funding source where applicable.
- Tool exports `.xlsx` summary using SheetJS.
- Visible validation panel showing warnings/errors.
- Sample data button for fast testing.

## Technical requirements
- Plain HTML/CSS/JavaScript.
- Calculation logic separated from UI rendering logic inside the same file.
- Clear comments indicating where key rules are applied.
- Start with total project price (cashflow intentionally out of scope for now).
