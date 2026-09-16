<svg width="400" height="400" viewBox="0 0 400 400" xmlns="http://www.w3.org/2000/svg">
  <style>
    /* Glow animation */
    .glow {
      animation: pulse 2s infinite;
    }
    @keyframes pulse {
      0% { text-shadow: 0 0 5px gold; fill: gold; }
      50% { text-shadow: 0 0 20px orange; fill: #ffd700; }
      100% { text-shadow: 0 0 5px gold; fill: gold; }
    }
    .glow-green {
      animation: pulseGreen 2s infinite;
    }
    @keyframes pulseGreen {
      0% { text-shadow: 0 0 5px #7fff00; fill: #7fff00; }
      50% { text-shadow: 0 0 20px lime; fill: #adff2f; }
      100% { text-shadow: 0 0 5px #7fff00; fill: #7fff00; }
    }
  </style>
  
  <!-- Circle background -->
  <circle cx="200" cy="200" r="180" fill="#1a1a40" stroke="gold" stroke-width="6"/>
  
  <!-- Prestige 🔮 glyphs (glow) -->
  <text x="200" y="40" text-anchor="middle" font-size="28" class="glow">🔮</text>
  <text x="360" y="210" text-anchor="middle" font-size="28" class="glow">🔮</text>
  <text x="200" y="380" text-anchor="middle" font-size="28" class="glow">🔮</text>
  <text x="40" y="210" text-anchor="middle" font-size="28" class="glow">🔮</text>
  
  <!-- Parchment 🌿 glyphs (green glow) -->
  <text x="290" y="90" text-anchor="middle" font-size="26" class="glow-green">🌿</text>
  <text x="310" y="310" text-anchor="middle" font-size="26" class="glow-green">🌿</text>
  <text x="90" y="310" text-anchor="middle" font-size="26" class="glow-green">🌿</text>
  <text x="90" y="90" text-anchor="middle" font-size="26" class="glow-green">🌿</text>
  
  <!-- Center seal -->
  <circle cx="200" cy="200" r="60" fill="gold"/>
  <text x="200" y="205" text-anchor="middle" font-size="18" fill="#1a1a40" font-weight="bold">
    Eternal Archive
  </text>
</svg>
