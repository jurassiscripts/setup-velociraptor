# setup-velociraptor

[![CI](https://github.com/lowlighter/setup-velociraptor/actions/workflows/ci.yml/badge.svg)](https://github.com/lowlighter/setup-velociraptor/actions/workflows/ci.yml)

This action sets up [Velociraptor](https://github.com/jurassiscripts/velociraptor) environment for use in actions.

# Usage

See [action.yml](action.yml)

Basic:

```yaml
steps:
  - uses: denolib/setup-deno@v2
  - uses: lowlighter/setup-velociraptor@master
  - run: |
      vr --version
```

# License

The scripts and documentation in this project are released under the
[MIT License](LICENSE)
