{
  "schemaVersion": 1,
  "label": "Rhythm",
  "message": "Parchment 🌿",
  "color": "gold"
}
name: Update Rhythm Badge
on:
  schedule:
    - cron: "0 0 * * *" # daily
jobs:
  update:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Update rhythm.json
        run: |
          # Example: prestige on equinox dates
          TODAY=$(date +%m-%d)
          if [[ "$TODAY" == "03-20" || "$TODAY" == "06-21" || "$TODAY" == "09-22" || "$TODAY" == "12-21" ]]; then
            echo '{"schemaVersion":1,"label":"Rhythm","message":"Prestige 🔮","color":"indigo"}' > rhythm.json
          else
            echo '{"schemaVersion":1,"label":"Rhythm","message":"Parchment 🌿","color":"gold"}' > rhythm.json
          fi
      - name: Commit changes
        run: |
          git config --global user.name 'rhythm-bot'
          git config --global user.email 'bot@hlaleledao'
          git add rhythm.json
          git commit -m "Update rhythm badge"
          git push
