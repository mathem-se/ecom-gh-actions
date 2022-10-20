# Reusable workflows

## Getting started

Add the following file `.github/workflows/pr.yml` to your project with this content:

```yaml
name: Pull request
on: [pull_request]

jobs:
  pull_request:
    uses: mathem-se/ecom-gh-actions/.github/workflows/pr.yml@main
```

Add the following scripts:

- `"test:ci"` (i.e. `"jest --coverage --ci --json --testLocationInResults --outputFile=./coverage/report.json"`)
