---
name: architecture-diagram
description: Generate professional, dark-themed technical architecture and cloud infrastructure diagrams as standalone HTML files with inline SVG. Use when the user wants to visualize software systems, VPCs, regions, microservices, or database topologies.
---

# ARCHITECTURE DIAGRAM
Generate professional, dark-themed technical architecture diagrams as standalone HTML files with inline SVG graphics. Works offline, no external rendering libraries required.

## Scope
**Best suited for:**
*   Software system architecture (frontend / backend / database layers).
*   Cloud infrastructure (VPC, regions, subnets, managed services).
*   Microservice / service-mesh topology.
*   Database + API maps, deployment diagrams.

## Design System & Visual Language

### Color Palette (Semantic Mapping)
| Component Type | Fill (rgba) | Stroke (Hex) |
| :--- | :--- | :--- |
| Frontend | `rgba(8, 51, 68, 0.4)` | `#22d3ee` (cyan-400) |
| Backend | `rgba(6, 78, 59, 0.4)` | `#34d399` (emerald-400) |
| Database | `rgba(76, 29, 149, 0.4)` | `#a78bfa` (violet-400) |
| Cloud/AWS | `rgba(120, 53, 15, 0.3)` | `#fbbf24` (amber-400) |
| Security | `rgba(136, 19, 55, 0.4)` | `#fb7185` (rose-400) |
| Message Bus | `rgba(251, 146, 60, 0.3)` | `#fb923c` (orange-400) |
| External | `rgba(30, 41, 59, 0.5)` | `#94a3b8` (slate-400) |

### Typography & Background
*   **Font:** JetBrains Mono (Google Fonts).
*   **Background:** Slate-950 (`#020617`) with a 40px grid pattern.

## Technical Implementation Details
*   **Component Rendering:** Rounded rectangles (`rx="6"`) with 1.5px strokes. Use a double-rect masking technique (opaque bg rect + semi-transparent styled rect) to hide arrows behind boxes.
*   **Connection Rules:** Draw arrows early in the SVG so they render behind components. Use SVG markers for arrowheads.
*   **Boundaries:** Use dashed lines for Security Groups (rose) and Regions (amber, `rx="12"`).

## Workflow
1.  **Define components** and their technologies.
2.  **Layout** with minimum 40px vertical gaps.
3.  **Generate the HTML file** with inline CSS and SVG.
4.  **Save as .html** (e.g., `./project-architecture.html`).
