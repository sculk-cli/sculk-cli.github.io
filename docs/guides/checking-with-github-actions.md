If you publish your Sculk modpack to a GitHub repository, you can use GitHub
Actions to verify your hashes are correct when you push your changes.

Copy the following workflow into `.github/workflows/check.yml`:

```yml
name: Check

on:
  push:
  pull_request:

jobs:
  check:
    runs-on: ubuntu-latest
    permissions:
      contents: read

    steps:
    - uses: actions/checkout@v4
    - name: Set up JDK 17
      uses: actions/setup-java@v4
      with:
        java-version: '17'
        distribution: 'temurin'
    - name: Setup Python 3
      uses: actions/setup-python@v2
    - name: Install Sculk
      run: python3 <(wget https://raw.githubusercontent.com/sculk-cli/sculk/main/install.py -q -O-)
    - name: Check hashes
      run: ~/.sculk/bin/sculk refresh --check
```

And add `.github/workflows/check.yml` to the `.sculkignore` file.

The workflow setups Java 17 and Python 3, then installs Sculk. It uses the
[`sculk refresh --check`](../commands/refresh.md) command to check for the packs
integrity. The workflow will fail if any hashes are invalid.
