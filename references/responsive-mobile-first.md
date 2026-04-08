# Responsive and Mobile-First Accessibility

Primary sources:
- WCAG 2.2 guidance on orientation, reflow, text spacing, and target size
- WAI mobile accessibility guidance through WCAG-related practices

## Mobile-first principles

- Start from the narrowest layout and add complexity upward.
- Preserve all core content and functionality at small widths.
- Keep source order meaningful; do not rely on CSS reordering to create a sensible reading order.
- Make controls large enough for touch and spaced to avoid accidental activation.
- Do not require landscape orientation unless essential.
- Do not require drag, hover, or fine pointer precision when a simpler alternative can work.

## Layout review points

- check at 320 CSS px wide
- check browser zoom and reflow
- check text spacing overrides
- verify sticky headers/footers do not obscure focus targets
- verify dialogs, drawers, and menus remain keyboard-usable on small screens

## Implementation guidance

- prefer fluid layouts over brittle fixed widths
- keep breakpoint logic simple and mobile-first
- preserve heading hierarchy and landmark structure across breakpoints
- do not hide essential labels or instructions on small screens
- ensure error messages and validation remain visible after zoom and reflow
