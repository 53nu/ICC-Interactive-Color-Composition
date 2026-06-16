# ICC — Interactive Color Composition

An interactive, Mondrian‑inspired archive of my ICC (Introduction to Computational Concepts) p5.js weekly projects. Each colored square is a clickable tile that opens the corresponding week's sketch.

**Live site:** https://53nu.github.io/ICC-Interactive-Color-Composition/

## Features
- **Generative Mondrian layout** — colored "week" squares + black accent blocks, randomly placed on every load; red/yellow/blue are always balanced.
- **One‑ray corner grid** — every box keeps a frame and shoots one line per corner (vertical or horizontal at random), each line in the box's own color, stopping at the first block it meets.
- **Living animation** — boxes slowly change size and position, so the grid keeps re‑flowing.
- **Numbered tiles** — each square shows its week number (Helvetica), scaled to fill the box.
- **Hover preview** — hovering a box shows a `Week#` tooltip and that project's image behind the number.
- **Click‑through** — clicking a box opens the live p5.js sketch.

## Tech
Vanilla JavaScript + HTML5 Canvas 2D. No frameworks, no build step. Deployed with GitHub Pages via GitHub Actions.

## Structure
```
index.html              # the whole app
image/                  # w2…w10.png hover previews
.github/workflows/      # Pages deploy workflow
```
