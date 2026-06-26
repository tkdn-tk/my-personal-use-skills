---
name: pixel-art
description: Convert images into retro pixel art with era-appropriate palettes (NES, Game Boy, PICO-8, SNES, arcade) and optionally animate them with effects. Use when the user wants retro styling, pixel art, or looping 8-bit/16-bit animations.
---

# Pixel Art — Pixel art w/ era palettes (NES, Game Boy, PICO-8)

Convert any image into retro pixel art, then optionally animate it into a short MP4 or GIF with era-appropriate effects (rain, fireflies, snow, embers).

## Overview
This skill guides you through converting photos to pixel-art PNGs using hardware-accurate palettes and adaptive quantization.

## When to Use
*   User wants retro pixel art from a source image.
*   User asks for NES / Game Boy / PICO-8 / C64 / arcade / SNES styling.
*   User wants a short looping animation (rain scene, night sky, snow, etc.).

## Workflow
1.  **Offer a style:** Suggest representative presets (arcade, nes, gameboy, snes, pico8).
2.  **Offer animation (optional):** Ask for a scene (night, urban, snow, storm, fire).
3.  **Generate:** Perform conversion using PIL/Pillow or external scripts if available.

## Preset Catalog
| Preset | Era | Palette | Block | Best for |
| :--- | :--- | :--- | :--- | :--- |
| **arcade** | 80s arcade | adaptive 16 | 8px | Bold posters, hero art |
| **snes** | 16-bit | adaptive 32 | 4px | Characters, detailed scenes |
| **nes** | 8-bit | NES (54) | 8px | True NES look |
| **gameboy** | DMG handheld | 4 green shades | 8px | Monochrome Game Boy |
| **pico8** | PICO-8 | 16 fixed | 6px | Fantasy-console look |
| **c64** | Commodore 64 | 16 fixed | 8px | 8-bit home computer |
| **apple2** | Apple II | 6 fixed | 10px | Extreme retro, 6 colors |

## Scene Catalog (for video)
*   **night:** Twinkling stars + fireflies + drifting leaves
*   **urban:** Rain + neon pulse
*   **snow:** Snowflakes + sparkles
*   **storm:** Rain + lightning
*   **fire:** Embers + sparkles

## Implementation Note
This skill assumes the presence of `Pillow` for image processing and `ffmpeg` for video generation. If scripts like `pixel_art.py` are not present, use standard Python image processing libraries to implement the dithering and palette snapping logic.
