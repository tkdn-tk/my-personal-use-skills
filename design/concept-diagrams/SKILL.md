---
name: concept-diagrams
description: Generate flat, minimal light/dark-aware SVG diagrams (flowcharts, structural, anatomical, physical objects) as standalone HTML files. Use when the user wants educational or non-software visuals like physics mechanisms, biology structures, or narrative journeys.
---

# Concept Diagrams | Hermes Agent

Generate flat, minimal light/dark-aware SVG diagrams as standalone HTML files, using a unified educational visual language with 9 semantic color ramps and automatic dark mode.

## Best Suited For:
*   **Educational visuals:** Physics, chemistry, math, biology mechanisms.
*   **Physical objects:** Aircraft, turbines, smartphones, anatomy cross-sections.
*   **Narrative journeys:** Lifecycles, historical processes.
*   **Systems Integration:** IoT networks, electricity grids.

## Design System Philosophy
*   **Flat:** No gradients, drop shadows, or glow effects.
*   **Minimal:** Show only essential nodes; no decorative icons inside boxes.
*   **Dark-mode ready:** Colors auto-adapt via CSS classes.

## Color Palette
Use the 9 color ramps (purple, teal, coral, pink, gray, blue, green, amber, red).
*   **c-gray:** Structural nodes.
*   **c-purple/teal/coral/pink:** General categories.
*   **c-blue/green/amber/red:** Semantic meaning (info, success, warning, error).

## Typography Rules
*   **th (14px, 500):** Node titles.
*   **ts (12px, 400):** Subtitles, arrow labels.
*   **t (14px, 400):** General text.
*   **Sentence case always.** Never Title Case or ALL CAPS.

## Layout & Spacing
*   **ViewBox:** `viewBox="0 0 680 H"`.
*   **Gap:** 60px minimum between boxes.
*   **Padding:** 24px horizontal, 12px vertical.
*   **Stroke Width:** 0.5px.

## Workflow
1.  **Layout components** using the Design System rules.
2.  **Write the HTML page** using a standalone SVG wrapper.
3.  **Save as .html** for direct browser viewing.
