# Dispatch Rhythm Map Integration

HlaleleDAO’s Dispatch Ring cadence is visualized in two ways:

## 🌟 Desktop View — Glyph Wheel
- **Animated SVG wheel** with glowing glyphs.
- 🔮 Prestige glyphs at cardinal points (quarterly, cosmic events, milestones).
- 🌿 Parchment glyphs at diagonals (weekly rhythm, mid‑month cadence).
- Center seal: **Eternal Archive**.

## 📱 Mobile View — Rhythm Bar
- **Horizontal SVG timeline** with glowing glyphs.
- 🔮 Prestige glyphs mark rare ceremonies.
- 🌿 Parchment glyphs mark weekly cadence.
- Scroll‑friendly, lightweight for phones.

## ⚙️ Integration
Use CSS media queries to switch views:

```html
<div class="glyph-wheel">
  <!-- Insert SVG wheel code -->
</div>

<div class="glyph-bar">
  <!-- Insert SVG bar code -->
</div>

<style>
  .glyph-wheel { display: block; }
  .glyph-bar { display: none; }

  @media (max-width: 768px) {
    .glyph-wheel { display: none; }
    .glyph-bar { display: block; }
  }
</style>
