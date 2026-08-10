# myceliumhq/.github

Org-wide defaults for [github.com/myceliumhq](https://github.com/myceliumhq):

- `profile/README.md` — shown on the org's GitHub profile page.
- `.github/workflows/node-ci.yml` — reusable CI workflow (lint, typecheck, build, test via pnpm). Consuming repos call it with:

```yaml
name: CI
on:
  push:
    branches: [main]
  pull_request:
jobs:
  ci:
    uses: myceliumhq/.github/.github/workflows/node-ci.yml@main
```
