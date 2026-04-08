# Accessibility Review Checklist

Use this as a compact QA pass.

## Semantics

- one clear page-level heading
- meaningful heading hierarchy
- real buttons and links
- correctly associated labels and form controls
- landmarks for major regions

## Keyboard

- every interactive element reachable by keyboard
- no keyboard traps
- logical tab order
- visible focus state
- dialogs and menus manage focus correctly

## Names and descriptions

- controls have accessible names
- icon-only buttons are labeled
- error text is associated to the field
- status and validation changes are announced appropriately

## Responsive/mobile

- works at narrow widths
- works at zoom/reflow
- target size and spacing are adequate
- no essential hover-only or drag-only interaction
- orientation changes do not break core tasks

## Visual accessibility

- sufficient text and UI contrast
- text remains readable with spacing overrides
- focus indicators are visible against the background

## ARIA

- ARIA is used only where needed
- roles, states, and properties match behavior
- APG patterns are followed for complex widgets
