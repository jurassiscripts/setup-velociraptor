# Setup velociraptor

[![CI](https://github.com/jurassiscripts/setup-velociraptor/actions/workflows/ci.yml/badge.svg)](https://github.com/jurassiscripts/setup-velociraptor/actions/workflows/ci.yml)

This action sets up [Velociraptor](https://github.com/jurassiscripts/velociraptor) environment for use in actions.

## Usage

See [action.yml](action.yml)

Basic:

```yaml
steps:
  - uses: denoland/setup-deno@v1
  - uses: jurassiscripts/setup-velociraptor@v1
  - run: |
      vr --version
```

| Input                  | Description    | Default value |
| ---------------------- | -------------- | ------------- |
| `velociraptor-version` | Version to use | `latest`      |
| `velociraptor-alias`   | Alias name     | `vr`          |

## License

The scripts and documentation in this project are released under the
[MIT License](LICENSE)
