# Python Hello World

A simple Python project demonstrating a standard project structure using `uv` for dependency management.

## Getting Started

### Prerequisites

Ensure you have [uv](https://github.com/astral-sh/uv) installed.

### Installation

1.  **Sync the project**:
    This will create a virtual environment and install the package in editable mode.
    ```bash
    uv sync
    ```

2.  **Manual editable install** (if needed):
    ```bash
    uv pip install -e .
    ```

## Running Tests

You can run the tests using the built-in `unittest` module via `uv run`:
```
bash
uv run python tests/test_hello_world.py
```
If you have `pytest` installed, you can simply run:
```
bash
uv run pytest
```
## Usage

You can use the function in your own scripts:
```
python
from py_hello_world.hello_world import hello_world

print(hello_world())
```