# MotionTypo Studio

A browser-based motion typography tool for creating animated text compositions with timeline control, full mobile support, and Premiere Pro-compatible alpha video export.

**No install. No build tools. Open the HTML file and work.**

---

## Español

MotionTypo Studio es una herramienta de motion typography que corre directamente en el navegador, sin instalación ni servidor. Permite crear composiciones de texto animado con múltiples capas, controladas por una línea de tiempo, y exportarlas como GIF, WebM, SVG o video MOV con canal alfa importable directamente en Premiere Pro.

**Texto y tipografía**

Cada capa de texto tiene control independiente de fuente (Google Fonts + fuentes del sistema + carga de fuentes locales TTF/OTF/WOFF), tamaño, peso, tracking, alineación y color. Soporta efectos de entrada, hold y salida con más de 15 animaciones: fade, slide, scale, blur, rotate, bounce, elastic, scramble de caracteres, entre otras. Cada fase tiene su propio easing (bounce, back, elastic, lineal, etc.) y dirección.

**Objetos adicionales**

Además de texto, soporta formas geométricas (rectángulo, círculo, línea, triángulo, estrella, polígono) y objetos SVG e imágenes importadas, todos animables con el mismo sistema de fases.

**Canvas y composición**

Tamaño de canvas configurable con presets (1080×1080, 1920×1080, 9:16, etc.), color de fondo con paleta de swatches, y soporte de fondo transparente. Los objetos son arrastrables, escalables y rotables directamente sobre el canvas con handles visuales. Rotación libre con pivot en el centro geométrico del objeto. El panel de capas permite reordenar, ocultar y bloquear elementos.

**Efectos globales**

Sombra con color, opacidad, distancia X/Y y desenfoque configurables. Glow / neón con color, intensidad y radio editables. Opción de usar el color de la capa para el glow.

**Timeline**

Cada capa tiene una barra visual de tres fases (in / hold / out) con duración y posición temporal ajustables por arrastre. Playback con play, pause, loop y scrubbing manual. Editable también desde dispositivos táctiles con handles touch-friendly.

**Interfaz móvil**

Layout adaptativo con tabs inferiores (Capas / Props / Tiempo / Exportar). El canvas se mantiene visible en la mitad superior mientras editas. Pinch-to-zoom con dos dedos, pan con dos dedos, doble tap sobre un texto para edición rápida. Todos los handles de selección, escala y rotación responden al touch.

**Gestos en canvas (desktop y móvil)**

Ctrl + rueda del mouse para zoom (25%–300%). Espacio + arrastre para pan. Pinch y pan con dos dedos en móvil. Doble click / doble tap sobre un texto enfoca el textarea de edición. Indicador de zoom y botón de reset visibles cuando se modifica la vista.

**Exportación**

- **MOV con canal alpha (códec PNG)** — archivo único `.mov` importable directamente en Premiere Pro y After Effects, con alpha real sin pérdida. Generado en navegador sin dependencias externas.
- **WebM** estándar y WebM Alpha (VP9 con yuva420p, vía MediaRecorder o ffmpeg.wasm).
- **GIF** animado con control de FPS, escala y calidad.
- **SVG** estático del frame actual.

Todas las exportaciones muestran barra de progreso unificada. Los proyectos se guardan y cargan en formato JSON.

---

## English

MotionTypo Studio is a motion typography tool that runs directly in the browser, with no installation or server required. It allows creating animated text compositions with multiple layers, controlled by a timeline, and exporting them as GIF, WebM, SVG, or MOV alpha video directly importable into Premiere Pro.

**Text and typography**

Each text layer has independent control over font (Google Fonts + system fonts + local font upload TTF/OTF/WOFF), size, weight, tracking, alignment, and color. Supports in, hold, and out effects with over 15 animations: fade, slide, scale, blur, rotate, bounce, elastic, character scramble, and more. Each phase has its own easing (bounce, back, elastic, linear, etc.) and direction.

**Additional objects**

In addition to text, it supports geometric shapes (rectangle, circle, line, triangle, star, polygon) and imported SVG objects and images, all animatable using the same phase system.

**Canvas and composition**

Configurable canvas size with presets (1080×1080, 1920×1080, 9:16, etc.), background color with swatches palette, and transparent background support. Objects can be dragged, scaled, and rotated directly on the canvas with visual handles. Free rotation pivots on the object's geometric center. The layers panel allows reordering, hiding, and locking elements.

**Global effects**

Drop shadow with configurable color, opacity, X/Y offset, and blur. Glow / neon with editable color, intensity, and radius. Option to use the layer's color for the glow.

**Timeline**

Each layer has a three-phase visual bar (in / hold / out) with duration and time position adjustable by dragging. Playback with play, pause, loop, and manual scrubbing. Also editable on touch devices with touch-friendly handles.

**Mobile interface**

Adaptive layout with bottom tabs (Layers / Props / Time / Export). Canvas stays visible in the upper half while editing. Pinch-to-zoom with two fingers, two-finger pan, double tap on text for quick editing. All selection, scale, and rotation handles respond to touch.

**Canvas gestures (desktop and mobile)**

Ctrl + mouse wheel for zoom (25%–300%). Space + drag for pan. Pinch and pan with two fingers on mobile. Double click / double tap on a text focuses the edit textarea. Zoom indicator and reset button appear when the view is modified.

**Export**

- **MOV with alpha channel (PNG codec)** — single `.mov` file directly importable into Premiere Pro and After Effects, with real lossless alpha. Generated in-browser with no external dependencies.
- **WebM** standard and WebM Alpha (VP9 with yuva420p, via MediaRecorder or ffmpeg.wasm).
- **GIF** animation with FPS, scale, and quality control.
- **SVG** static of the current frame.

All exports show a unified progress bar. Projects can be saved and loaded in JSON format.

---

## Features

- Animated text layers with in / hold / out timeline phases
- Shape, SVG, and image object support
- Per-layer font, size, weight, tracking, alignment, color, and rotation controls
- Global drop shadow and glow effects with editable parameters
- Free rotation with center-pivot for all object types
- Mobile-first responsive layout with bottom tab navigation
- Pinch-to-zoom and pan gestures on canvas (touch and mouse)
- Double-click / double-tap on text for quick editing
- Resizable panels (left, right) on desktop
- Layer management with drag-to-reorder, lock, and visibility
- Touch-friendly timeline editing
- GIF export with configurable FPS, scale, and quality
- WebM export with optional alpha channel
- **MOV export with PNG codec and alpha** — native Premiere Pro / After Effects compatibility
- Unified progress bars across all export formats
- Canvas size presets

---

## Usage

Open `Index.html` in any modern browser. No server required.

Or use the hosted version: https://graficogabo.github.io/motiontypestudio/Index.html

**Tested on:** Chrome, Firefox, Edge (desktop and mobile).

---

## Importing MOV alpha into Premiere Pro

1. Export → tab "MOV α" → select FPS → "Descargar MOV α"
2. In Premiere: drag the `.mov` directly to the Project panel or timeline
3. The clip is imported as standard video with alpha channel intact
4. Overlay it on top of other clips — the transparency works natively

The format is QuickTime MOV with PNG codec (RGBA, 32-bit, lossless), the same format used by professional alpha workflows.

---

## Dependencies

| Library | License | Loaded via |
|---|---|---|
| [gif.js 0.2.0](https://github.com/jnordberg/gif.js) (inline worker) | MIT | embedded |
| [ffmpeg.wasm](https://ffmpegwasm.netlify.app/) | LGPL 2.1+ | CDN (on WebM alpha export only) |
| [DM Mono / DM Sans / Inter](https://fonts.google.com) | SIL OFL 1.1 | Google Fonts |

The MOV alpha exporter has **no external dependencies** — the QuickTime container is built byte-by-byte in pure JavaScript.

---

## License

Copyright (C) 2026  Grafico Gabo

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
