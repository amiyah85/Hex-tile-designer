# HexFloor Studio

An interactive browser-based tool for designing period-accurate 1″ hexagon mosaic tile flooring — the kind found in American bathrooms, entryways, and commercial spaces from 1900–1950.

Design your room, place fixtures, create tile patterns on 12″×12″ sheets, add square tile borders, and preview the full layout at true scale.

![HexFloor Studio](https://img.shields.io/badge/tiles-1%22%20hex-c9a86c?style=flat-square) ![Era](https://img.shields.io/badge/era-1900--1950-8a8890?style=flat-square) ![License](https://img.shields.io/badge/license-personal%20use-232328?style=flat-square)

---

## Features

### Phase 1: Draw Room
- **Freehand polygon drawing** — click to place corner points with 1″ grid snap (Shift for 6″ snap)
- **Quick shapes** — instantly create a rectangle or L-shaped room by typing dimensions
- **90° angle snap** — toggle on to lock corners to right angles automatically
- **Live dimension labels** — see wall lengths in feet/inches as you draw
- **Double-click any wall** to type an exact dimension

### Phase 2: Fixtures
- **Drag-and-drop fixtures** — toilet, vanity, bathtub, shower, doorway, cabinet, island, or custom rectangles
- **Resize** by dragging the corner handle, or **double-click** to type exact dimensions
- **Border wrap toggle** — mark which fixtures the tile border should trace around (e.g. cabinets) vs. ignore (e.g. freestanding items)

### Phase 3: Design Pattern
- **12″×12″ sheet-based design** — paint hex tile patterns on standard sheet sizes, just like the real product
- **Multi-sheet layouts** — expand to 2×2, 3×3, etc. for larger repeating units (e.g. a center medallion surrounded by field sheets)
- **Period-accurate color palette** — 42 colors based on classic unglazed porcelain mosaic tiles from manufacturers like American Encaustic, Robertson, and Mosaic Tile Co:
  - Whites & creams, grays, blacks
  - Oxblood / maroon
  - Sanitary green
  - Cobalt & navy
  - Buff, tan, chocolate
- **Custom colors** — visual picker or paste a hex code directly
- **Saveable color palette** — save up to 12 custom colors for the session
- **Quick patterns** — checkerboard, stripes, random, flower
- **Paint tools** — brush, bucket fill, eraser, eyedropper

### Square Tile Border System
- **Configurable width** — 1–8 rows of 1″ square tiles
- **Strip cross-section designer** — paint a repeating border pattern with full control over each row
- **Corner block designer** — paint a separate square block for every corner/turn
- **Border follows room perimeter + fixture edges** — wraps around fixtures you've marked

### Phase 4: Room Preview
- **True-to-scale rendering** — 1″ hex tiles at real inch scale; zoom in to see individual tiles, zoom out for the full room
- **Seamless pattern tiling** — sheet patterns repeat across the room using world-space coordinate wrapping
- **Pattern offset drag** — hold Shift and drag to slide the pattern alignment, or use nudge buttons for 1″ adjustments
- **Border + field integration** — square tile border fills the perimeter, hex field pattern fills the interior

### General
- **12 standard grout colors** — period-accurate Portland cement tones from bright white to black, plus sand and tan
- **Grout width control** — none, thin (~1mm), medium (~2mm), thick (⅛″)
- **Zoom** — scroll wheel (centers on cursor), +/− buttons, zoom-to-fit (⊡)
- **Pan** — Alt+drag or middle-click drag
- **Undo** — Ctrl/Cmd+Z
- **Export** — download your design as a PNG

---

## Usage

Open `index.html` in any modern browser. No install, no dependencies, no build step — it's a single self-contained HTML file.

Or visit the hosted version: **[amiyah85.github.io/Hex-tile-designer](https://amiyah85.github.io/Hex-tile-designer)**

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Shift` (hold) | 6″ grid snap while drawing room |
| `Shift` (hold in preview) | Drag to offset pattern alignment |
| `Alt` + drag | Pan the canvas |
| `Ctrl/Cmd + Z` | Undo |
| `Delete` | Remove selected fixture |

---

## About the Palette

The tile colors are based on the standard unglazed porcelain hex mosaic palette that was ubiquitous in American architecture from roughly 1900 to 1950. These tiles were produced by companies including:

- **American Encaustic Tiling Co.**
- **Robertson Art Tile Co.**
- **Mosaic Tile Company**
- **American Olean**

The grout colors reflect the Portland cement-based grouts of the era, ranging from bright white to charcoal, with warm sand and buff tones.

---

## Tech

- Single HTML file (~650 lines)
- Vanilla JavaScript, no frameworks
- Canvas 2D rendering
- Flat-top hexagonal grid math with axial coordinates
- Fonts: DM Sans + Playfair Display (Google Fonts)
