---
name: home-insulation-planner-maintainer
description: Maintain and extend the Home Insulation Planner static web app across root, V1, and V2 HTML variants. Use when updating insulation cost/ROI calculations, UI copy, input fields, validation behavior, version parity, or documentation for this repository.
---

# Home Insulation Planner Maintainer

## Audit repository layout

- Treat `index.html` as the current primary entry point.
- Treat `V1/index.html` and `V2/index.html` as versioned variants that may intentionally diverge.
- Read `README.md` before changing behavior or feature descriptions.

## Implement calculation changes safely

- Locate every calculation path in affected HTML files before editing formulas.
- Keep units explicit in labels and formulas (R-value, square feet, dollars, years).
- Guard against invalid numeric input using sensible defaults and input constraints.
- Preserve deterministic output formatting (currency, percent, and rounded year values).

## Keep UX and copy coherent

- Keep field labels, helper text, and results language aligned with insulation-planning terminology.
- Prefer plain-language explanations for assumptions and savings outputs.
- Keep accessibility basics intact: label/input association, button text clarity, and readable result sections.

## Manage multi-version updates

- Decide whether a change applies to only one version or all versions.
- If applying across versions, port the same logic and text updates deliberately rather than blindly copying blocks.
- If behavior differs across versions, add a short rationale in `README.md`.

## Validate before handoff

- Open each changed HTML entry and confirm no JavaScript console errors.
- Verify at least one realistic scenario end-to-end (inputs → calculation → displayed recommendation).
- Re-check any linked navigation between version pages after edits.
