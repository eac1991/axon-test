# Button Component Rules (Axon Deterministic Version)

---

## 🧠 PURPOSE

This file defines STRICT rules for the Button component.

Rules are deterministic and MUST be interpreted as final truth.

If a rule exists → it overrides all other sources.

---

## 🚫 COLOR RULES (CRITICAL)

### Q: Can colors be modified manually?

❌ NO

- Button colors cannot be overridden manually
- Colors are fully controlled by design tokens
- No direct color values (HEX / RGB / CSS) are allowed

✔ ONLY EXCEPTION:
- Focus state uses predefined token:
  ds/color/alt/blue-high

---

## 🎨 TOKEN RULES

### Q: Can tokens be overridden?

❌ NO

- Design tokens are immutable at component level
- Tokens can only be consumed, not modified
- No custom token injection is allowed

---

## 🧩 BORDER RULES

### Q: Can border width be changed?

❌ NO

- Border width is fixed
- Applies to all variants
- Only color may vary via tokens

---

## 📐 SIZE RULES

### Q: Can size or height be changed?

❌ NO

- Height is fixed
- Width is content-driven only
- fullWidth is the only exception

---

## 🧱 LAYOUT RULES

### Q: Can padding be changed?

❌ NO

- Internal padding is fixed
- Must follow design system spacing rules

---

## 🧠 ICON RULES

### Q: Can icons be modified?

✔ YES (LIMITED)

- Icon can be replaced
- Icon size is ALWAYS 20x20px
- Icon cannot be resized

---

## 🏷 LABEL RULES

### Q: Can label styles be changed?

❌ NO

- Typography is controlled by system tokens
- No custom font, size, or color allowed

### Q: Can label text include punctuation?

❌ NO

- Labels must use verbs only
- No punctuation allowed

---

## ⚠️ DANGER STATE RULES

### Q: What happens when Danger = true?

✔ Applies fixed token:

ds/color/alt/red-high

Affects:
- background
- border
- label
- icon

---

## 🧭 KIND RULES

- Primary → main action only
- Secondary → requires Primary in same context
- Ghost → low emphasis actions

---

## ⌨️ INTERACTION RULES

- Enter / Space → trigger action
- Tab / Shift+Tab → navigation
- Focus → blue outline using ds/color/alt/blue-high

---

## 🧠 FINAL DECISION RULE

When asked a question:

1. Match rule category
2. Return YES / NO based on rule
3. If rule exists → DO NOT infer
4. If rule is missing → assume NOT ALLOWED

---

## 🚫 GLOBAL OVERRIDE RULE

No external design system knowledge is allowed.

Only this file defines Button behavior.
