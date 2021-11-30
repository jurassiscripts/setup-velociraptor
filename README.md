# Setup velociraptor

[![CI](https://github.com/jurassiscripts/setup-velociraptor/actions/workflows/ci.yml/badge.svg)](https://github.com/jurassiscripts/setup-velociraptor/actions/workflows/ci.yml)

This action sets up [Velociraptor](https://github.com/jurassiscripts/velociraptor) environment for use in actions.

For convenience, `setup-velociraptor@v2` can also run automatically [`actions/checkout@v2`](https://github.com/marketplace/actions/checkout) and [`denoland/setup-deno@1`](https://github.com/marketplace/actions/setup-deno).

## Usage

See [action.yml](action.yml)

### @v2

Basic:

```yaml
steps:
  - uses: jurassiscripts/setup-velociraptor@v2
  - run: |
      vr --version
```

| Input                  | Description                          | Default value |
| ---------------------- | ------------------------------------ | ------------- |
| `checkout`             | Whether to checkout repository first | `true`        |
| `deno-version`         | Deno version to use                  | `1.x`         |
| `velociraptor-version` | Velociraptor version to use          | `latest`      |
| `velociraptor-alias`   | Velociraptor alias name              | `vr`          |

| Output                 | Description                                          | 
| ---------------------- | ---------------------------------------------------- | 
| `deno-is-canary`       | Whether installed Deno version is a canary version   | 
| `deno-version`         | Deno version that was installed                      | 
| `velociraptor-version` | Velociraptor version that was installed              | 

### @v1

Basic:

```yaml
steps:
  - uses: actions/checkout@v2
  - uses: denoland/setup-deno@v1
  - uses: jurassiscripts/setup-velociraptor@v1
  - run: |
      vr --version
```

| Input                  | Description                 | Default value |
| ---------------------- | --------------------------- | ------------- |
| `velociraptor-version` | Velociraptor version to use | `latest`      |
| `velociraptor-alias`   | Velociraptor alias name     | `vr`          |

## License

The scripts and documentation in this project are released under the
[MIT License](LICENSE)
