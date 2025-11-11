<p align="left">Olá sou o David e sou estudante.</p>

###

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=DavidBarrosn2&hide_title=true&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=true&theme=rose_pine&locale=en&hide_border=false&order=1" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=DavidBarrosn2&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=rose_pine&hide_border=false&order=2" height="150" alt="languages graph"  />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=DavidBarrosn2&radius=16&theme=tokyo-night&area=true&order=5" height="300" alt="activity-graph graph"  />
</div>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="40" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="40" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jest/jest-plain.svg" height="40" alt="jest logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/storybook/storybook-original.svg" height="40" alt="storybook logo"  />
</div>

###


name: Generate snake game

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Sutil/snk@master
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          svg_out_path: dist/github-contribution-grid-snake2.svg
          snake_color: 'blue'

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  

###

<div align="center">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=DavidBarrosn2.DavidBarrosn2&right_color=royalblue"  />
</div>

###
