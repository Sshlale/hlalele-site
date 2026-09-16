#!/bin/bash

# Prompt contributor for glyph prefix
echo "🌟 HlaleleDAO Commit Ritual 🌟"
echo "Choose a glyph prefix for this commit:"
echo "1) 🌿 [Parchment Rhythm]"
echo "2) 🔮 [Prestige Dispatch]"
echo "3) 📜 [Scroll Update]"
echo "4) ✨ [Ceremonial Seal]"
echo "5) 🕊️ [Sovereign Archive]"

read -p "Enter number: " choice

case $choice in
  1) prefix="🌿 [Parchment Rhythm]" ;;
  2) prefix="🔮 [Prestige Dispatch]" ;;
  3) prefix="📜 [Scroll Update]" ;;
  4) prefix="✨ [Ceremonial Seal]" ;;
  5) prefix="🕊️ [Sovereign Archive]" ;;
  *) prefix="🌿 [Parchment Rhythm]" ;; # default
esac

# Prepend prefix to commit message
sed -i "1s/^/$prefix /" "$1"
