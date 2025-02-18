# pre-commit

GitHub Action that runs pre-commit hooks.

## Usage

```yaml
    steps:
      - name: Checkout
        uses: actions/checkout@<commit-hash>
      - name: Run pre-commit
        uses: nikaro/actions/pre-commit@<commit-hash>
```

## Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|                                   INPUT                                    |  TYPE  | REQUIRED |         DEFAULT         |                   DESCRIPTION                    |
|----------------------------------------------------------------------------|--------|----------|-------------------------|--------------------------------------------------|
|                <a name="input_args"></a>[args](#input_args)                | string |  false   |     `"--all-files"`     |     arguments to pass to pre-commit <br>run      |
| <a name="input_python-version"></a>[python-version](#input_python-version) | string |  false   |                         |                  python version                  |
|                <a name="input_skip"></a>[skip](#input_skip)                | string |  false   | `"no-commit-to-branch"` |  comma separated list of hooks <br>id to skip    |
|           <a name="input_version"></a>[version](#input_version)            | string |  false   |        `"3.5.0"`        |                pre-commit version                |
|           <a name="input_workdir"></a>[workdir](#input_workdir)            | string |  false   |          `"."`          | change working directory for pre-commit <br>run  |

<!-- AUTO-DOC-INPUT:END -->
