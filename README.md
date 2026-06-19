# M-101 — Column Frame (3D)

Interactive 3D model of the column-marking layout for the residential building at
**No 4, Dhanakodiammal Street, Kodambakkam**, framed as a **stilt + 3-storey** skeleton.

Built from drawing **M-101 R0 — Column Marking Layout** (19.6.2026).

## How to open

Double-click **`index.html`** — it opens in any modern web browser
(Chrome, Edge, Safari, Firefox). No installation needed.

> Requires an internet connection the first time, as the 3D engine (three.js)
> loads from a CDN.

## Controls

- **Drag** — orbit / rotate
- **Scroll** (or pinch) — zoom
- **Right-drag** (or two-finger drag) — pan
- **Click / tap a column** — popup with its grid reference and section size
- **3D / Plan / Elev·A / Elev·1** buttons — preset camera views
- **Display toggles** — beams, floor plates, site boundary, compass, grid refs,
  column tags, scale figure

## What's modelled

- **20 columns**, extracted directly from the drawing's vector geometry (the
  magenta column-marking rectangles only). Each sits on its grid node to within
  ~0.01 ft. See `data/column_schedule.csv`.
- Sections **9"×1'-6"**, **9"×2'**, and rotated **1'-6"×9"** — at true position,
  size and orientation. The layout is staggered (e.g. row 1 = A·C·D, row 3 = D only).
- **Stilt + 3 storeys** at **10'-0"** floor-to-floor (40'-0" to roof), with tie/floor
  beams between columns at every level and a roof slab. The stilt is left open.
- **Site boundary** (blue) traced from the survey line on the drawing.
- **North** taken from the title-block arrow (points to grid A): N = grid A,
  S = grid D, E = row 1, W = row 12. Shown by the ground compass and cardinal labels.

## Notes / assumptions

- Storey height (10'-0") and the stilt + 3 configuration are as advised by the client;
  the beam layout is an indicative skeleton, not a stamped framing/beam drawing.
- Grid lines are drawn for all 12 rows as reference, even where a row carries one column.

## Files

```
M-101_Column_Frame_3D/
├── index.html                     ← open this
├── README.md
└── data/
    ├── column_schedule.csv        ← 20 columns: grid, position, size (ft & mm)
    └── column_schedule.json       ← same data + grid definition
```
