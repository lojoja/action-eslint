# action-eslint

A composite action that lints files with [ESLint](https://eslint.org).

This repository is not meant to be referenced in third-party workflows; please fork the repository if you would like to use it in your project.

## Inputs

| Name              | Description                                     | Default |
| ----------------- | ----------------------------------------------- | ------- |
| cache             | Whether to cache dependencies.                  | "true"  |
| node_version      | The node version to use in version spec syntax. | "22"    |
| working_directory | The working directory for the action.           | "."     |

## Examples

```
jobs:
  eslint:
    runs-on: ubuntu-latest
    steps:
      - uses: lojoja/action-eslint@main
        with:
          cache: "true"
          node_version: "22"
```

## License

action-eslint is released under the [MIT License](./LICENSE)
