# CT127 Programming for Data Analysis

This codespace holds the Python environment for the module. This will be updated constantly, please check for latest updates.

## What is in this repository

| Item | What it is |
| --- | --- |
| `pyproject.toml` | The list of Python packages this codespace uses |
| `uv.lock` | The exact versions that were installed from that list |
| `submissions/` | Homework you hand in. Lab work stays outside this folder |

Run the following commands in the terminal:

```bash
source .venv/bin/activate  # activates env in the terminal
uv pip list                # lists installed packages
```

## Notebooks

Open a `.ipynb` file. If it asks for a kernel, choose **Select Kernel**, then the `.venv` environment. Run a cell with Shift+Enter.

## Python packages

All packages in the environment are managed by `uv` and installed in `.venv`. 

To add a package, run:

```bash
uv add <name>
```

The `uv` manager updates both `pyproject.toml` and `uv.lock` files and installs it. Then restart the notebook kernel to reflect changes.

See `uv` [documentation](https://docs.astral.sh/uv/guides/projects/).

## Terminal

Right-click a folder in the Explorer and choose **Open in Integrated Terminal**. Check that the prompt ends with that folder name before you run a command.
