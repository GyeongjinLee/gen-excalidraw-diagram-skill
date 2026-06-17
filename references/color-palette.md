# Color Palette & Brand Style

**This is the single source of truth for all colors and brand-specific styles.** To customize diagrams for your own brand, edit this file — everything else in the skill is universal.

> **Brand basis:** This palette is built **strictly from the Surface, Text, and Hairlines & Borders colors** in `design.md` (Apple web language) — no accent hue. It is a **monochrome / tonal** system tuned for official company documents. Because there is no color hue, meaning is carried by three things working together: **tone** (light tile → gray → near-black tile → pure black), **shape geometry** (ellipse = start/end, diamond = decision, rectangle = process), and **stroke style** (solid / dashed / weight). This mirrors Apple's own method — "alternate the surface before adding chrome; the color change itself is the divider."

---

## Shape Colors (Semantic)

Colors encode meaning, not decoration. Each semantic purpose has a fill/stroke pair drawn only from the surface/ink/hairline ladder. Emphasis rises with tonal weight: light tiles for normal flow, mid-gray for caution, near-black tiles for terminal/AI emphasis, pure black for error.

| Semantic Purpose | Fill | Stroke |
|------------------|------|--------|
| Primary/Neutral | `#ffffff` | `#1d1d1f` |
| Secondary | `#f5f5f7` | `#333333` |
| Tertiary | `#fafafc` | `#7a7a7a` |
| Start/Trigger | `#f5f5f7` | `#1d1d1f` |
| End/Success | `#272729` | `#1d1d1f` (white text) |
| Warning/Reset | `#d2d2d7` | `#333333` |
| Decision | `#ffffff` | `#1d1d1f` |
| AI/LLM | `#2a2a2c` | `#1d1d1f` (white text) |
| Inactive/Disabled | `#fafafc` | `#d2d2d7` (use dashed stroke) |
| Error | `#000000` | `#000000` (white text) |

**Contrast rule**: Light-filled shapes pair a darker ink stroke with the light fill. Dark-tile shapes (End, AI, Error) invert — contrast comes from **white text** (`#ffffff`) on the dark surface, not from a lighter fill.

**Differentiation without hue**: Start vs. End vs. Decision is told apart by **geometry and position**, not color — keep the ellipse/diamond/rectangle conventions strict so a reader can parse the flow in grayscale.

---

## Text Colors (Hierarchy)

Use color on free-floating text to create visual hierarchy without containers. Hierarchy follows Apple's ink scale.

| Level | Color | Use For |
|-------|-------|---------|
| Title | `#1d1d1f` | Section headings, major labels (Near-Black Ink) |
| Subtitle | `#333333` | Subheadings, secondary labels (Ink Muted 80) |
| Body/Detail | `#7a7a7a` | Descriptions, annotations, metadata (Ink Muted 48) |
| On light fills | `#1d1d1f` | Text inside light-colored shapes |
| On dark fills | `#ffffff` | Text inside near-black/black shapes (End, AI, Error) |
| Muted on dark | `#cccccc` | Secondary text on dark tiles (Body Muted) |

---

## Evidence Artifact Colors

Used for code snippets, data examples, and other concrete evidence inside technical diagrams. Dark surfaces use Apple's near-black tile tone; in this monochrome system, syntax is shown with the ink-on-dark scale rather than colored tokens.

| Artifact | Background | Text Color |
|----------|-----------|------------|
| Code snippet | `#272729` | `#ffffff` primary · `#cccccc` secondary · `#7a7a7a` comments |
| JSON/data example | `#272729` | `#ffffff` keys · `#cccccc` values |

---

## Default Stroke & Line Colors

| Element | Color |
|---------|-------|
| Arrows | Use the stroke color of the source element's semantic purpose |
| Structural lines (dividers, trees, timelines) | Hairline (`#e0e0e0`) or Ink Muted 48 (`#7a7a7a`) |
| Marker dots (fill + stroke) | Ink (`#1d1d1f`) |

---

## Background

| Property | Value |
|----------|-------|
| Canvas background | `#ffffff` (Pure White; `#f5f5f7` Parchment for an alternate quiet canvas) |
