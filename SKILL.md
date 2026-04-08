---
name: web-accessibility-standards
description: Use when designing, reviewing, or implementing web interfaces against accessibility and web standards, including WCAG 2.2, ARIA, semantic HTML, keyboard access, responsive mobile-first layouts, focus management, and accessibility review checklists.
---

# Web Accessibility Standards Skill

Use this skill when the task touches accessibility, semantics, ARIA, keyboard support, responsive behavior, or compliance-oriented UI review.

## Core position

1. Start with semantic HTML before adding ARIA.
2. Treat WCAG 2.2 as the current baseline standard for guidance.
3. Prefer mobile-first, responsive layouts that preserve meaning and operability.
4. Accessibility is behavior plus semantics, not only labels and contrast.
5. Review with keyboard, focus, screen-reader semantics, zoom/reflow, and touch targets in mind.

## Workflow

1. Identify the task type:
   - new UI design
   - component implementation
   - accessibility review
   - responsive/mobile fix
   - ARIA/widget work
2. Use native HTML semantics first.
3. Add ARIA only when native HTML does not express the needed interaction or state.
4. Check keyboard behavior and visible focus early, not at the end.
5. Validate layout and content flow at narrow widths and zoomed/reflowed states.
6. For interactive widgets, use WAI-ARIA APG patterns as the implementation reference.
7. For compliance-sensitive work, map issues to WCAG 2.2 success criteria.

## Practical rules

- Prefer real buttons, links, inputs, labels, tables, lists, headings, and landmarks.
- Never add ARIA that overrides correct native semantics without a clear reason.
- If you use an ARIA role, implement the keyboard behavior that role implies.
- Keep DOM order and reading order aligned with the visual order.
- Ensure focus indicators are visible and not obscured.
- Ensure targets are large enough and not too tightly packed.
- Avoid pointer-only, drag-only, hover-only, and orientation-dependent interaction.
- Support zoom, reflow, and text spacing without losing content or function.

## When to consult which reference

- Read [references/wcag-22.md](references/wcag-22.md) when the task needs standards mapping, review findings, or success criteria.
- Read [references/aria-apg.md](references/aria-apg.md) when implementing widgets, landmarks, names, descriptions, or keyboard interaction.
- Read [references/responsive-mobile-first.md](references/responsive-mobile-first.md) when building layouts, breakpoints, or touch/mobile interactions.
- Read [references/review-checklist.md](references/review-checklist.md) when doing an accessibility review or QA pass.

## Output expectations

When producing code or review guidance:
- explain the semantic choice first
- call out relevant WCAG 2.2 criteria when useful
- mention keyboard and focus implications for interactive changes
- include responsive/mobile implications where layout or targets are involved
- avoid recommending ARIA where native HTML already solves the problem
