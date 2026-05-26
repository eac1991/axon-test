# Button Component Rules (Axon v15 Execution Engine)

---

# 🧠 CORE PRINCIPLE

This file is an EXECUTION ENGINE, not documentation.

Every rule MUST be interpreted as deterministic logic.

If a rule exists → it is executable.

No descriptive language is allowed in decision-critical sections.

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
1. State tokens (danger, focus)
2. Component tokens
3. Global tokens

FINAL:
- No direct color values allowed

---

# 🎨 TOKEN ENGINE

CASE: Token resolution request

CONDITION:
- Any property requires styling token

RESOLUTION ORDER:
1. Component tokens (Button.tokens.json)
2. Variant overrides (Button.variants.json)
3. Global tokens (/tokens/tokens.json)

RULE:
- If no override exists → inherit base token
- Never return “not defined” if fallback exists

---

# 🧩 BORDER ENGINE

CASE: Border styling

CONDITION:
- Button border is evaluated

RESOLUTION:
- Border width = FIXED (no overrides allowed)
- Border color = token-based only

PRIORITY:
- State override > component default > global token

FINAL:
- Border width cannot change under any condition

---

# 📐 SIZE ENGINE

CASE: Button sizing behavior

CONDITION:
- Layout calculation for width/height

RESOLUTION:
- Height = FIXED
- Width = CONTENT-DRIVEN (hug behavior)
- fullWidth = allowed override

PRIORITY:
- fullWidth overrides hug behavior only

---

# 🧱 LAYOUT ENGINE

CASE: Button layout behavior

CONDITION:
- Component rendering layout rules

RESOLUTION:
- Padding is FIXED
- Spacing is SYSTEM CONTROLLED
- Layout adapts to content only

FINAL:
- No manual layout overrides allowed

---

# 🧠 TEXT OVERFLOW ENGINE

CASE: Text exceeds available width

CONDITION:
- content width > container width

RESOLUTION:
- Expand button horizontally FIRST
- Wrap text only if constrained by parent container
- NEVER truncate by default

PRIORITY:
1. Expansion
2. Wrapping
3. Truncation (forbidden unless explicitly defined)

FINAL STATE:
- Text must remain fully visible unless constrained externally

---

# 🧩 BUTTON GROUP ENGINE

CASE: Multiple buttons in same container

CONDITION:
- sibling Button components detected

RESOLUTION:
- Apply spacing rules:
  - default = 8px
  - ghost variant = 16px

ALIGNMENT RULE:
- baseline alignment mandatory
- height consistency required

PRIORITY:
- Variant spacing overrides default spacing

FINAL:
- Groups must remain visually aligned and consistent

---

# 🧠 ICON ENGINE

CASE: Icon usage in Button

CONDITION:
- icon property present

RESOLUTION:
- Icon size fixed: 20x20px
- Position: leading only
- Replacement allowed
- Resizing forbidden

---

# 🏷 LABEL ENGINE

CASE: Button label rendering

CONDITION:
- text label is present

RESOLUTION:
- Must use verbs only
- No punctuation allowed
- Typography controlled by tokens only

---

# ⚠️ DANGER ENGINE

CASE: danger=true state

CONDITION:
- Button marked as danger state

RESOLUTION:
- Apply ds/color/alt/red-high to:
  - background
  - border
  - label
  - icon

PRIORITY:
- Danger overrides all other color rules

---

# 🧭 VARIANT ENGINE

CASE: kind resolution

CONDITION:
- Button kind is defined

RESOLUTION:
- Primary: main action only
- Secondary: requires Primary context
- Ghost: low emphasis / optional action

---

# ⌨️ INTERACTION ENGINE

CASE: keyboard interaction

CONDITION:
- user interacts via keyboard

RESOLUTION:
- Enter / Space → trigger action
- Tab → next element
- Shift+Tab → previous element

---

# 🎯 FOCUS ENGINE

CASE: focus state

CONDITION:
- Button receives focus

RESOLUTION:
- Apply ds/color/alt/blue-high
- Border width fixed at 0.5px
- Layout must NOT change

---

# 🧠 ACCESSIBILITY ENGINE

CASE: accessibility evaluation

CONDITION:
- Button rendered in UI

RESOLUTION:
- ariaLabel required if label is not descriptive
- Must support full keyboard navigation
- Must be operable without pointer input

---

# 🚫 GLOBAL EXECUTION RULE

ONLY rules defined in this engine or inherited tokens are valid.

Everything else is INVALID as a source of behavior.
