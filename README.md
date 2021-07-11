# actions

GitHub Actions and helper for Open Peer Power workflows

## oppfest

_Run oppfest to validate standalone integration repositories._

**action**: `openpeerpower/actions/oppfest@main`

example implementation:

```yaml
name: Validate with oppfest

on:
  push:
  pull_request:
  schedule:
    - cron:  '0 0 * * *'

jobs:
  validate:
    runs-on: "ubuntu-latest"
    steps:
        - uses: "actions/checkout@v2"
        - uses: "openpeerpower/actions/oppfest@main"
```

This will run the `oppfest` action on every push and pull request to all branches, as well as every midnight.


## Helpers

_A collection of GitHub Action helpers, these are considered internal to the Open Peer Power organization on GitHub and will change without warning._

- [git-init](./helpers/git-init/action.yml)
- [info](./helpers/info/action.yml)
- [jq](./helpers/jq/action.yml)
- [verify-version](./helpers/action.yml)
- [version](./helpers/version/action.yml)
- [version-push](./helpers/version-push/action.yml)
