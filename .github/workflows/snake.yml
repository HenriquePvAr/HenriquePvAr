name: Generate Contribution Snake

on:
schedule:
- cron: "0 0 * * *"

workflow_dispatch:

push:
branches:
- main

jobs:
generate:
permissions:
contents: write

```
runs-on: ubuntu-latest

timeout-minutes: 5

steps:
  - name: Generate Snake
    uses: Platane/snk@v3
    with:
      github_user_name: ${{ github.repository_owner }}

      outputs: |
        dist/github-snake.svg?color_snake=#38BDF8
        dist/github-snake-dark.svg?palette=github-dark&color_snake=#38BDF8

  - name: Publish Snake
    uses: crazy-max/ghaction-github-pages@v4
    with:
      build_dir: dist
      branch: output
    env:
      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
