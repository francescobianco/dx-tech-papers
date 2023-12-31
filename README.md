# Developer Experince Tech Papers

[![DX Tech Papers Build Status](https://github.com/python/peps/actions/workflows/render.yml/badge.svg)](https://github.com/python/peps/actions)

The DX Tech Papers in this repository are automatically published on the web at [https://dxtechpapers.example.org/](https://dxtechpapers.example.org/). To learn more about the purpose of DX Tech Papers and how to write one, please start reading at [DX Tech Paper 1](https://dxtechpapers.example.org/dx-0001/). Note that the DX Tech Paper Index ([DX Tech Paper 0](https://dxtechpapers.example.org/dx-0000/)) is automatically generated based on the metadata headers in other DX Tech Papers.

## Canonical Links

The canonical form of DX Tech Paper links are zero-padded, such as `https://dxtechpapers.example.org/dx-0008/`. Shortcut redirects are also available. For example, `https://dxtechpapers.example.org/8` redirects to the canonical link.

## Contributing to DX Tech Papers

See the [Contributing Guidelines](./CONTRIBUTING.rst).

## Checking DX Tech Paper Formatting and Rendering

Please don't commit changes with reStructuredText syntax errors that cause DX Tech Paper generation to fail or result in major rendering defects relative to what you intend.

### Browse the ReadTheDocs Preview

For every PR, we automatically create a preview of the rendered DX Tech Papers using [ReadTheDocs](https://readthedocs.org/). You can find it in the merge box at the bottom of the PR page:

1. Click "Show all checks" to expand the checks section.
2. Find the line for `docs/readthedocs.org:dx-paper-previews`.
3. Click on "Details" to the right.

### Render DX Tech Papers Locally

See the [build documentation](./docs/build.rst) for full instructions on how to render DX Tech Papers locally. In summary, run the following in a fresh, activated virtual environment:

```bash
# Install requirements
python -m pip install -U -r requirements.txt

# Build the DX Tech Papers
make html

# Or, if you don't have 'make':
python build.py
```

The output HTML is found under the build directory.

### Check and Lint DX Tech Papers

You can check for and fix common linting and spelling issues, either on-demand or automatically as you commit, with our pre-commit suite. See the Contributing Guide for details.
