
<!-- Typing SVG -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=4CAF50&center=true&vCenter=true&width=500&lines=Hi%2C+I'm+Akshay+Tayade;SDE+%40+Sarv;Working+on+SarvCrawl" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=sarvakshay&color=4CAF50" alt="profile views" />
</p>

## What I'm building

**[SarvCrawl](https://crawl.sarv.com)** is Sarv's web crawler.
<!-- TODO: one line on what you work on -->

## Tech I use

<!-- TODO: keep only what you actually use; full list at https://skillicons.dev -->
<p>
  <img src="https://skillicons.dev/icons?i=js,ts,react,nextjs,nodejs,python,docker,nginx,linux,git" />
</p>

## GitHub stats

<p>
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=sarvakshay&show_icons=true&hide_border=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sarvakshay&layout=compact&hide_border=true" />
</p>

## Contribution snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sarvakshay/sarvakshay/output/github-snake-dark.svg" />
  <img alt="snake eating contributions" src="https://raw.githubusercontent.com/sarvakshay/sarvakshay/output/github-snake.svg" />
</picture>

3. Set up the snake (needs a GitHub Action)

In the same repo, create the file .github/workflows/snake.yml:

name: Generate snake

on:
  schedule:
    - cron: "0 0 * * *"   # daily
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

Then go to Actions → Generate snake → Run workflow once. That creates the output branch, and the snake image starts showing.

Things to know

- The stats and snake will look empty until you have some public activity. Your profile has no public repos yet. To count work in private repos, go to Settings → Public profile and turn on "Include private contributions on my profile."
- Pinned repos (Aman's "Popular repositories") come from Customize your pins on the Overview tab.
- The badge images come from free public services (readme-typing-svg, komarev, github-readme-stats). They're sometimes slow or rate-limited, so a broken image is usually their side, not your README.
