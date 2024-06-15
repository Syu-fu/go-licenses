# go-licenses

This GitHub Action uses Google's `go-license` tool to check for license compliance in your Go project.  
By integrating this action into your CI/CD pipeline, you can automatically ensure that all dependencies in your Go project comply with your licensing requirements.

## Features

- **Automated License Checks**: Automatically check licenses of all dependencies in your Go project.
- **Easy Integration**: Simple to set up and integrate into any GitHub repository.

## Prerequisites

- A GitHub repository containing a Go project.
- A working `go.mod` file in your repository root.

## Usage

To use this action, create or modify the `.github/workflows/go-license-check.yml` file in your repository with the following content:

```yaml
name: Go License Check

on:
  pull_request:

jobs:
  license-check:
    runs-on: ubuntu-latest
    name: license check
    steps:
      - uses: actions/checkout@4

      - uses: Syu-fu/go-licenses@v0.1.0
```

## License

This GitHub Action is licensed under the MIT License.  
See the LICENSE file for more details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with your changes.

## Support

If you have any questions or need help, feel free to open an issue on the GitHub repository.

---

For more information on go-license, please visit the [official repository](https://github.com/google/go-licenses).
