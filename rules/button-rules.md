# Button Component - Rules

## Description
Buttons allow users to perform an action or navigate to another page. They are used to guide user actions within flows and highlight primary interactions.

---

## Guidelines

- Primary button (Kind: Primary) is used for main actions in the interface.
- Secondary button (Kind: Secondary) is used for secondary actions.
- Secondary button must only be used when a Primary button exists in the same context.
- Ghost button (Kind: Ghost) is used for low-emphasis or residual actions.
- Ghost buttons can be icon-only, label-only, or icon + label.

### Layout constraints
- Button height is fixed and cannot be modified.
- Button width is adaptive based on content.
- Buttons can optionally expand to full width using fullWidth property.
- Internal paddings are fixed and cannot be modified.
- Border width is fixed and cannot be modified.

### Icons
- Icons are optional in all variants.
- Icon size is fixed at 20x20px.
- Icons cannot be resized.

### Labels
- Labels must not include punctuation.
- Labels should use verbs.
- Avoid nouns or adjectives as primary labels.

### Colors
- Colors are fully controlled by design tokens.
- Tokens cannot be overridden manually.

---

## Danger State Rules

When Danger = true:
- Background, border, label, and icon use token: ds/color/alt/red-high
- Applies to Primary, Secondary, and Ghost variants depending on state

---

## Behaviours

- Default spacing between buttons: 8px
- Ghost buttons spacing: 16px
- Default width is hug content
- Buttons can expand to full container width

### Keyboard interaction
- Enter / Space triggers action
- Tab navigates forward
- Shift + Tab navigates backward
- Focus state applies blue outline (ds/color/alt/blue-high)

---

## Properties

- kind
- disabled
- loading
- fullWidth
- label
- icon
- onClick
- type
- ariaLabel
- tabIndex
- className
- testId

---

## Accessibility
- ariaLabel is required when label is not descriptive
