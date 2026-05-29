# MotionTypo Studio

A browser-based motion typography tool for creating animated text compositions with timeline control and GIF export.

**No install. No build tools. Open the HTML file and work.**

MotionTypo Studio es una herramienta de motion typography que corre directamente en el navegador, sin instalación ni servidor. Permite crear composiciones de texto animado con múltiples capas, controladas por una línea de tiempo, y exportarlas como GIF, video WebM o SVG estático.

**Texto y tipografía**

Cada capa de texto tiene control independiente de fuente (Google Fonts + fuentes del sistema + carga de fuentes locales TTF/OTF/WOFF), tamaño, peso, tracking, alineación y color. Soporta efectos de entrada, hold y salida con más de 15 animaciones: fade, slide, scale, blur, rotate, bounce, elastic, scramble de caracteres, entre otras. Cada fase tiene su propio easing (bounce, back, elastic, lineal, etc.) y dirección.

**Objetos adicionales**

Además de texto, soporta formas geométricas (rectángulo, círculo, línea, triángulo, estrella, polígono) y objetos SVG e imágenes importadas, todos animables con el mismo sistema de fases.

**Canvas y composición**

Tamaño de canvas configurable con presets (1080×1080, 1920×1080, 9:16, etc.), color de fondo con paleta de swatches, y soporte de fondo transparente. Los objetos son arrastrables, escalables y rotables directamente sobre el canvas. El panel de capas permite reordenar, ocultar y bloquear elementos.

**Timeline**

Cada capa tiene una barra visual de tres fases (in / hold / out) con duración y posición temporal ajustables por arrastre. Playback con play, pause, loop y scrubbing manual.

**Exportación**

GIF con control de FPS, escala y calidad. Video WebM con y sin canal alpha. SVG estático del frame actual. Los proyectos se pueden guardar y cargar en formato JSON.

---

MotionTypo Studio is a motion typography tool that runs directly in the browser, with no installation or server required. It allows creating animated text compositions with multiple layers, controlled by a timeline, and exporting them as GIF, WebM video, or static SVG.

**Text and typography** 

Each text layer has independent control over font (Google Fonts + system fonts + local font upload TTF/OTF/WOFF), size, weight, tracking, alignment, and color. Supports in, hold, and out effects with over 15 animations: fade, slide, scale, blur, rotate, bounce, elastic, character scramble, and more. Each phase has its own easing (bounce, back, elastic, linear, etc.) and direction.

**Additional objects**

In addition to text, it supports geometric shapes (rectangle, circle, line, triangle, star, polygon) and imported SVG objects and images, all animatable using the same phase system.

**Canvas and composition** 

Configurable canvas size with presets (1080×1080, 1920×1080, 9:16, etc.), background color with a swatches palette, and transparent background support. Objects can be dragged, scaled, and rotated directly on the canvas. The layers panel allows reordering, hiding, and locking elements.

**Timeline**

Each layer has a three-phase visual bar (in / hold / out) with duration and time position adjustable by dragging. Playback with play, pause, loop, and manual scrubbing.

**Export**

GIF with FPS, scale, and quality control. WebM video with and without alpha channel. Static SVG of the current frame. Projects can be saved and loaded in JSON format.

---

## Features

- Animated text layers with in / hold / out timeline phases
- Shape and SVG object support
- Per-layer font, size, weight, tracking, alignment, and color controls
- Resizable panels (left, right)
- Layer management with drag-to-reorder, lock, and visibility
- GIF export with configurable FPS, scale, and quality
- Canvas size presets

---

## Usage

Download `MotionTypeV10.html`, open it in any modern browser. No server required.

Or click here https://graficogabo.github.io/motiontypestudio/Index.html

---

## Dependencies

| Library | License | Loaded via |
|---|---|---|
| [gif.js 0.2.0](https://github.com/jnordberg/gif.js) | MIT | CDN (on export) |
| [DM Mono / DM Sans](https://fonts.google.com/specimen/DM+Mono) | SIL OFL 1.1 | Google Fonts |

---

## License

Copyright (C) 2026  Grafico Gabo

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
