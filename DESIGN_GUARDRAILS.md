# DESIGN_GUARDRAILS

This document defines strict visual guardrails for the periodic table project. Future implementation tasks must preserve the existing design system unless the user explicitly requests a specific visual change.

## 1) Non-negotiable design rules

1. Preserve the current visual identity exactly as the default baseline.
2. Keep the existing element color palette unchanged.
3. Keep the current grid layout structure, spacing logic, and placement model unchanged.
4. Keep the EL data array structure/content unchanged unless the request is specifically about data correction.
5. Keep the existing background tone unchanged.
6. Keep the current panel style (shape, borders, shadows, depth language, and card treatment) unchanged.
7. Keep the existing typography scale hierarchy unchanged.
8. Maintain current interaction behavior and information hierarchy.
9. Any change that affects visual rhythm, density, or contrast must be treated as a design change and blocked unless explicitly requested.

## 2) Forbidden changes

- Re-theming or replacing the color system.
- Changing element category colors or semantic mapping.
- Altering the core periodic-table grid model or moving groups/periods for visual preference.
- Refactoring/reformatting EL data array values for stylistic reasons.
- Changing the page/app background tone.
- Redesigning panel/card style (including corners, border language, shadows, or translucency).
- Modifying typography scale steps, base sizing system, or heading/body ratio.
- Introducing new fonts or changing font families purely for style.
- Applying visual “modernization” passes without explicit user instruction.

## 3) Allowed changes

- Bug fixes that do not alter established visual output.
- Accessibility improvements that preserve overall look and layout intent.
- Performance or code-quality refactors with no visual delta.
- Content/data fixes where the user requests factual correction.
- Additive features that are visually consistent with existing styles and do not alter core system tokens.
- User-explicit visual fixes that clearly name what must change.

## 4) Visual tone keywords

Use these keywords as a validation lens for any future UI work:

- Scientific
- Structured
- Clear
- Balanced
- Educational
- Precise
- Calm contrast
- Functional

If a proposal conflicts with these keywords, treat it as out-of-scope unless explicitly requested.

## 5) Desktop / tablet / mobile QA checklist

Before finalizing UI-related work, verify all of the following:

### Desktop QA

- Grid alignment remains consistent with current baseline layout.
- Element tiles/panels retain original color and panel styling.
- Typography scale and hierarchy match baseline.
- No unexpected spacing, overflow, or clipping.
- Background tone remains unchanged.

### Tablet QA

- Responsive layout preserves the same visual hierarchy.
- Panel style and color mapping remain identical to baseline.
- Tap targets and readability remain usable without retheming.
- No breakpoint introduces unintended token/style drift.

### Mobile QA

- Core content remains legible with original type scale relationships.
- Grid/list adaptation keeps established identity and tone.
- No palette shifts, panel restyling, or background changes.
- Scrolling and interaction remain functional without visual redesign.

## 6) Explicit change warning (must follow)

**Do not change any of the following unless the user explicitly asks for that exact visual fix:**

- Element color palette
- Grid layout
- EL data array
- Background tone
- Panel style
- Typography scale

If a task is ambiguous, default to **no visual change** and request clarification in task planning notes.
