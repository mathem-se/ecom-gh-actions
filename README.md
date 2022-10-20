# Reusable workflows

## Getting started

Add the file `.github/workflows/pr.yml` to your project with the following contents.

```yaml
name: Pull request
on: [pull_request]

jobs:
  pull_request:
    uses: mathem-se/ecom-gh-actions/.github/workflows/pr.yml@main
```

Add a `test:ci` script to your `package.json`.

Example:

```json
"test:ci": "jest --coverage --ci --json --testLocationInResults --outputFile=./coverage/report.json"
```
