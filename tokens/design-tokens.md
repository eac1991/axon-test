# Design Tokens

## Overview

This document contains the exported design tokens used by the Axon Design System.

The token structure includes:

- Color modes (light / dark)
- Component-specific tokens
- Typography scales
- Spacing scales
- Border and radius values
- Semantic states
- Resolution modes

---

# Color Tokens

## Light Mode

### Content

| Token | Value |
|---|---|
| ds.color.content.default | #000000 |
| ds.color.content.inverse | #FFFFFF |
| ds.color.content.states.hover | #757575 |
| ds.color.content.states.pressed | #363636 |
| ds.color.content.states.disabled | #B3B3B3 |

### Background

| Token | Value |
|---|---|
| ds.color.bg.default | #FFFFFF |
| ds.color.bg.low | #F7F7F7 |
| ds.color.bg.inverse | #000000 |

---

## Dark Mode

### Content

| Token | Value |
|---|---|
| ds.color.content.default | #FFFFFF |
| ds.color.content.inverse | #000000 |
| ds.color.content.states.hover | #C4C4C4 |
| ds.color.content.states.pressed | #D4D4D4 |
| ds.color.content.states.disabled | #757575 |

---

# Component Tokens

## Button

### Primary

| State | Light | Dark |
|---|---|---|
| Default | #000000 | #FFFFFF |
| Hover | #434343 | #EDEDED |
| Pressed | #515151 | #D4D4D4 |

### Danger

| State | Light | Dark |
|---|---|---|
| Hover | #B11E1B | #ED6664 |
| Pressed | #911F1C | #C3382E |

---

# Resolution Tokens

## Border

| Token | High | Low |
|---|---|---|
| none | 0px | 0px |
| default | 0.5px | 1px |
| high | 1px | 2px |

## Radius

| Token | Value |
|---|---|
| none | 0px |
| rounded | 4px |
| full | 144px |

---

# Typography

## Font Families

| Token | Value |
|---|---|
| primary | Inter |
| monospace | NotoSansMono |

## Font Weights

| Token | Medium | Large |
|---|---|---|
| default | 400 | 500 |
| mid | 600 | 700 |
| high | 800 | 900 |

---

# Spacing Scale

| Token | Medium | Large |
|---|---|---|
| 50 | 8px | 12px |
| 100 | 16px | 20px |
| 150 | 24px | 32px |
| 200 | 32px | 40px |
| 300 | 48px | 64px |
| 400 | 64px | 84px |

---

# Token Variable Mapping

| Variable ID | Token | Semantic Name | Native Value |
|---|---|---|---|
| VariableID:01cf4c070149d583e71b0c20ed775dd8e279e87b/23:293 | ds.color.content.inverse | Inverse text color | #FFFFFF |

---

# Notes

These tokens are intended to be consumed by Axon in order to:

- Validate Design System consistency
- Interpret semantic UI decisions
- Support AI-assisted contextual reasoning
- Compare visual states and modes
- Detect inconsistencies across components
- Connect Figma variables and component behavior
