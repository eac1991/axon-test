# Button Component Rules (Axon v13 Enhanced)

---

## 🧠 PURPOSE

This file defines deterministic rules for the Button component.

Rules are strict, executable, and override all other sources.

---

# 🚫 COLOR RULES

- Colors are fully controlled by design tokens
- No manual color overrides allowed
- Only exception: focus state uses ds/color/alt/blue-high
- Danger state uses ds/color/alt/red-high

---

# 🎨 TOKEN RULES

- Tokens are immutable
- Only consumption allowed
- No overrides at component level
- Inheritance applies if no explicit mapping exists

---

# 🧩 BORDER RULES

- Border width is fixed
- Border color controlled by tokens
- No override of stroke width allowed

---

# 📐 SIZE RULES

- Height is fixed
- Width is content-driven (hug behavior)
- fullWidth is allowed override

---

# 🧱 LAYOUT RULES

- Internal padding is fixed
- Spacing system is immutable
- Button adapts to content size only

---

# 🧠 TEXT BEHAVIOUR (RESTORED CRITICAL RULES)

## Overflow behavior

- Text grows horizontally by default
- No truncation unless explicitly defined in system
- Button must expand before wrapping text

## Wrapping rules

- Text wraps only if container forces constraint
- No manual line breaks allowed
- Label must remain single logical action

---

# 🧩 GROUPING / SPACING BEHAVIOUR (RESTORED)

## Button groups

- Default spacing between buttons: 8px
- Ghost buttons spacing: 16px

## Group layout rules

- Primary + Secondary buttons can be grouped
- Ghost buttons are visually separated
- Groups must maintain alignment baseline

---

# 🧠 ICON RULES

- Icon optional in all variants
- Icon size fixed: 20x20px
- Icons cannot be resized
- Icon position: leading only (default behavior)

---

# 🏷 LABEL RULES

- Labels must use verbs only
- No punctuation allowed
- Labels are not stylable manually
- Typography comes from design system tokens only

---

# ⚠️ DANGER STATE

When danger=true:

- Background → ds/color/alt/red-high
- Border → ds/color/alt/red-high
- Label → ds/color/alt/red-high
- Icon → ds/color/alt/red-high

Applies to all variants unless overridden explicitly.

---

# 🧭 VARIANT RULES

## Primary
- Main action only
- Highest emphasis

## Secondary
- Requires Primary in same context
- Never used alone

## Ghost
- Low emphasis actions
- Can be icon-only or label-only

---

# ⌨️ INTERACTION RULES

- Enter / Space → trigger action
- Tab → next element
- Shift + Tab → previous element

---

# 🎯 FOCUS STATE

- Focus uses ds/color/alt/blue-high
- Border width remains fixed (0.5px)
- Focus does not modify layout

---

# 🧠 ACCESSIBILITY

- ariaLabel required when label is not descriptive
- Keyboard navigation must be supported
- Button must remain operable without pointer interaction

---

# 🚫 GLOBAL RULE

No behavior is allowed unless explicitly defined in this file or inherited from design system tokens.
