# Button Component Rules (Axon v16 Engine + Semantic Router)

---

# 🧠 CORE PRINCIPLE

This file is an EXECUTION ENGINE.

All rules are deterministic and must be executed, not interpreted.

---

# 🚫 COLOR ENGINE

CASE: Button color assignment

CONDITION:
- Colors are never manually assigned

RESOLUTION:
- Use design tokens only
- Focus exception: ds/color/alt/blue-high
- Danger state: ds/color/alt/red-high

PRIORITY:
1. State tokens
2. Component tokens
3. Global tokens

---

# 🎨 TOKEN ENGINE

CASE: Token resolution request

CONDITION:
- Any property requires styling token

RESOLUTION ORDER:
1. Component tokens
2. Variant overrides
3. Global tokens

RULE:
- If no override exists → inherit base token

---

# 🧩 BORDER ENGINE

CASE: Border styling

CONDITION:
- Button border evaluated

RESOLUTION:
- Border width FIXED
- Border color token-based only

---

# 📐 SIZE ENGINE

CASE: Button sizing

CONDITION:
- Layout calculation

RESOLUTION:
- Height FIXED
- Width CONTENT-DRIVEN
- fullWidth allowed override

---

# 🧱 LAYOUT ENGINE

CASE: Layout behavior

CONDITION:
- rendering rules

RESOLUTION:
- padding FIXED
- spacing system controlled
- layout adapts to content only

---

# 🧠 TEXT OVERFLOW ENGINE

CASE: Text exceeds width

CONDITION:
- content width > container width

RESOLUTION:
- expand horizontally first
- wrap only if constrained
- no truncation by default

PRIORITY:
1. expansion
2. wrapping
3. truncation (forbidden)

---

# 🧩 BUTTON GROUP ENGINE

CASE: Button grouping

CONDITION:
- multiple buttons in same container

RESOLUTION:
- spacing:
  - default = 8px
  - ghost = 16px

ALIGNMENT:
- baseline required
- equal height alignment required

---

# 🧠 ICON ENGINE

CASE: icon usage

CONDITION:
- icon present

RESOLUTION:
- size 20x20px fixed
- leading only
- no resizing

---

# 🏷 LABEL ENGINE

CASE: label rendering

CONDITION:
- text label present

RESOLUTION:
- verbs only
- no punctuation
- token-based typography only

---

# ⚠️ DANGER ENGINE

CASE: danger=true

CONDITION:
- danger state active

RESOLUTION:
- apply ds/color/alt/red-high to all surfaces

---

# 🧭 VARIANT ENGINE

CASE: kind

CONDITION:
- variant defined

RESOLUTION:
- primary = main action
- secondary = requires primary context
- ghost = low emphasis

---

# ⌨️ INTERACTION ENGINE

CASE: keyboard input

CONDITION:
- user interaction

RESOLUTION:
- enter/space trigger
- tab navigation
- shift+tab back

---

# 🎯 FOCUS ENGINE

CASE: focus state

CONDITION:
- element focused

RESOLUTION:
- ds/color/alt/blue-high
- border 0.5px fixed

---

# 🧠 ACCESSIBILITY ENGINE

CASE: accessibility

CONDITION:
- component rendered

RESOLUTION:
- ariaLabel required if label unclear
- full keyboard support required

---

# 🚫 GLOBAL RULE

No behavior outside this engine is valid.

---

# 🧠 SEMANTIC ROUTING LAYER (CRITICAL FIX)

---

## 🎯 PURPOSE

Maps user language → correct execution engine.

---

## 🔑 KEYWORD MAPPING (MANDATORY)

IF user query contains:

- group
- groups
- grouping
- agrupación
- botones juntos
- spacing between buttons

→ USE BUTTON GROUP ENGINE

---

## 🚫 FORBIDDEN BEHAVIOR

Never fallback to generic layout rules if semantic match exists.

---

## 🧠 PRIORITY ORDER

1. Semantic routing layer
2. Specific engine
3. Global fallback (last resort only)

---

## 🎯 RESULT

All “grouping” queries MUST resolve to Button Group Engine.
