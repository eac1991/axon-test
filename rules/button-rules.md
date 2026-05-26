# Button Component Rules (Axon v14 Enhanced)

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

# 🧠 TEXT OVERFLOW BEHAVIOR (DETERMINISTIC)

## RULE: TEXT EXPANSION

IF content exceeds available width:

→ Button MUST expand horizontally (hug behavior)
→ Text MUST NOT be truncated by default

## RULE: WRAPPING

IF container forces width constraint:

→ Text MAY wrap to next line
→ Wrapping is passive (no manual line breaks allowed)

## RULE: PRIORITY ORDER

Expansion > Wrapping > Truncation

→ Truncation is NOT allowed unless explicitly defined elsewhere

---

# 🧩 BUTTON GROUP BEHAVIOR (DETERMINISTIC)

## RULE: DEFAULT GROUP SPACING

IF buttons are in a group:

→ spacing MUST be 8px

## RULE: GHOST VARIANT SPACING

IF button kind = Ghost:

→ spacing MUST be 16px from other buttons

## RULE: GROUP COMPOSITION

Allowed combinations:

✔ Primary + Secondary
✔ Primary + Ghost
✔ Secondary + Ghost

## RULE: ALIGNMENT

All buttons in a group:

→ MUST align baseline
→ MUST maintain consistent height alignment

---

# 🧠 ICON RULES

- Icon optional in all variants
- Icon size fixed: 20x20px
- Icons cannot be resized
- Icon position: leading only

---

# 🏷 LABEL RULES

- Labels must use verbs only
- No punctuation allowed
- Typography controlled by design system tokens only

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

## Secondary
- Requires Primary in same context

## Ghost
- Low emphasis actions

---

# ⌨️ INTERACTION RULES

- Enter / Space → trigger action
- Tab → next element
- Shift + Tab → previous element

---

# 🎯 FOCUS STATE

- Focus uses ds/color/alt/blue-high
- Border width fixed at 0.5px

---

# 🧠 ACCESSIBILITY

- ariaLabel required when label is not descriptive
- Must support full keyboard navigation

---

# 🚫 GLOBAL RULE

No behavior is allowed unless explicitly defined in this file or inherited from design system tokens.
