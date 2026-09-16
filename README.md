name: Enforce Ceremonial Commit Style

on:
  pull_request:
    types: [opened, synchronize, reopened]

jobs:
  check-commits:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v3
        with:
          fetch-depth: 0

      - name: Verify commit messages
        run: |
          echo "🔍 Checking commit messages for glyph prefixes..."
          invalid=$(git log origin/main..HEAD --pretty=format:"%s" | grep -vE "^(🌿|🔮|📜|✨|🕊️)")
          if [ -n "$invalid" ]; then
            echo "❌ Invalid commit messages found:"
            echo "$invalid"
            echo "Commit messages must start with one of: 🌿 🔮 📜 ✨ 🕊️"
            exit 1
          else
            echo "✅ All commit messages follow ceremonial style."
          fi
