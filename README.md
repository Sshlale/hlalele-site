name: Ceremonial Issue
description: Create an issue aligned with HlaleleDAO’s sovereign rhythm
title: "🌿 / 🔮 / 📜 / ✨ / 🕊️ — [Short description]"
labels: ["ceremonial"]

body:
  - type: dropdown
    id: rhythm
    attributes:
      label: 🔮 Rhythm Declaration
      description: Select the glyph cadence this issue belongs to
      options:
        - 🌿 Parchment Rhythm — Weekly cadence, sponsor gratitude, everyday testimony
        - 🔮 Prestige Dispatch — Rare ceremonies, codex unveilings, milestones
        - 📜 Scroll Update — Documentation, README, guides
        - ✨ Ceremonial Seal — Footer glyphs, archive confirmations
        - 🕊️ Sovereign Archive — Eternal Archive indexing, milestone preservation
    validations:
      required: true

  - type: textarea
    id: summary
    attributes:
      label: 📜 Sovereign Summary
      description: Describe the sovereign act this issue represents
      placeholder: "What scroll, glyph, or dispatch is being updated?"
    validations:
      required: true

  - type: textarea
    id: validation
    attributes:
      label: ✨ Validation
      description: How will this issue uphold ceremonial rhythm?
      placeholder: "Commit style, README badges, wheel/bar visuals…"

  - type: textarea
    id: archive
    attributes:
      label: 🕊️ Archive Note
      description: Explain how this issue contributes to the Eternal Archive
      placeholder: "Does it mark a milestone, seal a ceremony, or index a dispatch?"
