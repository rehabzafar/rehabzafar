name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ e2388525-5bd3-4864-8a20-f95e2ac701fa }}
          GH_TOKEN: ${{ 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 }}
