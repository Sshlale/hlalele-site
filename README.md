<svg width="300" height="300" viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
  <style>
    /* Glow animations */
    .glow { animation: pulse 2s infinite; }
    @keyframes pulse {
      0% { fill: gold; }
      50% { fill: orange; }
      100% { fill: gold; }
    }
    .glow-green { animation: pulseGreen 2s infinite; }
    @keyframes pulseGreen {
      0% { fill: #7fff00; }
      50% { fill: lime; }
      100% { fill: #7fff00; }
    }
  </style>
  
  <!-- Circle background -->
  <circle cx="150" cy="150" r="140" fill="#1a1a40" stroke="gold" stroke-width="5"/>
  
  <!-- Prestige 🔮 glyphs (quarterly + cosmic) -->
  <text x="150" y="40" text-anchor="middle" font-size="24" class="glow">🔮</text>
  <text x="260" y="155" text-anchor="middle" font-size="24" class="glow">🔮</text>
  <text x="150" y="270" text-anchor="middle" font-size="24" class="glow">🔮</text>
  <text x="40" y="155" text-anchor="middle" font-size="24" class="glow">🔮</text>
  
  <!-- Parchment 🌿 glyphs (weekly rhythm) -->
  <text x="210" y="80" text-anchor="middle" font-size="22" class="glow-green">🌿</text>
  <text x="220" y="220" text-anchor="middle" font-size="22" class="glow-green">🌿</text>
  <text x="80" y="220" text-anchor="middle" font-size="22" class="glow-green">🌿</text>
  <text x="80" y="80" text-anchor="middle" font-size="22" class="glow-green">🌿</text>
  
  <!-- Center seal -->
  <circle cx="150" cy="150" r="45" fill="gold"/>
  <text x="150" y="155" text-anchor="middle" font-size="14" fill="#1a1a40" font-weight="bold">
    Eternal Archive
  </text>
</svg>
