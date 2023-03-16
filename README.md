- 👋 Hi, I’m @ThanhLong0113
- 👀 I’m interested in Web Programming, Machine Learning and Shell Programming.
- 🌱 I’m currently learning Computer Science at Hanoi University of Science and Technology.

<!--START_SECTION:waka-->
<!--END_SECTION:waka-->

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
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
          SHOW_OS: "True"
          SHOW_PROJECTS: "False"
