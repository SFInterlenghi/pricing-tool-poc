# Pricing Tool POC

This repository contains a browser-only proof of concept to unify project pricing for Process Systems Engineering teams in Brazil.

## Files

- `index.html`: Single self-contained application (HTML/CSS/JS) with calculation logic and XLSX export.
- `docs/requirements.md`: Consolidated functional and technical requirements.
- `docs/rules.md`: Implemented calculation and validation rules.
- `docs/assumptions.md`: Open questions and placeholders where rules are not yet confirmed.
- `samples/sample_input.csv`: Example input rows for quick manual testing.

## How to run

1. Open `index.html` in a modern browser.
2. Fill project metadata.
3. Add/edit cost lines.
4. Select funding mode.
5. Click **Recalculate** to refresh totals and validation messages.
6. Click **Export XLSX** to download the summary workbook.

No backend or installation is required.

## Notes

- The ANP Petrobras and ANEEL specific formulas are intentionally placeholders until business rules are confirmed.
- See `docs/assumptions.md` for pending rule clarifications.
