# ARIA and APG

Primary source:
- WAI-ARIA Authoring Practices Guide
- https://www.w3.org/WAI/ARIA/apg/
- https://www.w3.org/WAI/ARIA/apg/practices/read-me-first/

## Core rules

- No ARIA is better than bad ARIA.
- A role is a promise: if you assign a role, implement the expected behavior.
- Native HTML beats ARIA whenever native HTML already provides the semantics and interaction.

## Use ARIA for

- composite widgets that native HTML does not cover well
- state and relationship metadata, such as expanded, pressed, selected, controls, describedby
- landmarks when native sectioning alone is not enough for the structure

## Do not use ARIA for

- replacing a native button with `div role="button"` unless you also implement keyboard support, focus handling, and state
- masking correct native semantics without a strong reason
- styling or visual hooks unrelated to accessibility semantics

## APG usage guidance

When implementing menus, tabs, accordions, dialogs, comboboxes, listboxes, trees, carousels, or similar widgets:
- check the APG pattern first
- follow the documented keyboard interaction model
- ensure accessible name and description are present
- test with keyboard and relevant assistive technology combinations

## Mobile caveat

The APG itself notes that some ARIA features are not consistently supported on mobile browsers and touch interfaces. Treat mobile support as something to test, not assume.
