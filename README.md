# Repository Profiler Action
> An action to create a metric-based profile from your repository metadata 🚀

## Usage

Add to your repository:

```yaml
on:
  repository_dispatch:
    types: action_trigger
    branches:
        - master
        - main
jobs:
  profile:
    runs-on: ubuntu-22.04
    steps:
      - name: Checkout
        uses: actions/checkout@v3
        with:
          fetch-depth: 0
      - name: Repository Profiler
        uses: Alokit-Innovations/repo-profiler@v0
```
