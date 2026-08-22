# BigOBoard

BigOBoard is a lightweight, single-file, infinite canvas whiteboard application built entirely with Vanilla HTML, CSS, and JavaScript. 

It is designed to be lightning-fast, entirely client-side, and highly portable. There are no build steps, no dependencies, and no servers required.

## Features

- **Infinite Canvas:** Pan around limitlessly using the `Spacebar` + drag or the Pan tool. Zoom in and out using the mouse wheel or pinch-to-zoom.
- **Drawing Tools:**
  - Structure Pen
  - Detail Pen
  - Accent Pen
  - Highlighter
- **Shapes & Elements:**
  - Rectangles
  - Arrows
  - Nodes (Circles)
  - Text (Click to type)
- **Dynamic Resizing:** Hold `Alt` (or `Option`) and use the scroll wheel to quickly adjust the width of your drawing tool or the font size of your text.
- **Auto-Save:** Everything you draw is automatically saved in your browser's `localStorage`. When you close and reopen the file, your board will be exactly as you left it.
- **Exporting:**
  - **Export PNG:** Captures everything you've drawn and exports it as a clean image file.
  - **Export JSON:** Downloads the raw data of your board, perfect for backups or sharing the state with another browser.
- **Full History:** Complete Undo/Redo capabilities (`Ctrl+Z` / `Ctrl+Y`).

## How to Use

Simply open the `BigOBoard.html` file in any modern web browser (Chrome, Edge, Firefox, Safari). You don't need a local server.

```bash
# On Windows
start BigOBoard.html

# On Mac
open BigOBoard.html

# On Linux
xdg-open BigOBoard.html
```

## Shortcuts & Controls

| Action | Shortcut / Input |
| --- | --- |
| **Pan Canvas** | `Spacebar` + Drag (or middle-click) |
| **Zoom Canvas** | Scroll wheel (or pinch) |
| **Undo** | `Ctrl` + `Z` |
| **Redo** | `Ctrl` + `Y` |
| **Reset View** | `Ctrl` + `0` |
| **Change Tool Size** | Hold `Alt` + Scroll wheel |
| **Quick Select Tools** | `S` (Structure), `D` (Detail), `A` (Accent), `H` (Highlighter), `T` (Text), `R` (Rect), `W` (Arrow), `N` (Node), `E` (Eraser), `V` (Pan) |

## Tech Stack

- **HTML5 Canvas** for high-performance 2D rendering.
- **Vanilla JavaScript** for all application logic (state machine, hit detection, history).
- **Inline CSS** for layout and styling (custom properties, flexbox).
