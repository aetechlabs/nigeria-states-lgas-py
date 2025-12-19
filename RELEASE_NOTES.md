# Release v1.0.4

Release date: 2025-12-20

Highlights
- Add a simple CLI `nigeria-states-lgas` to query states and LGAs from the terminal.
- Improve `nigeria_states_lgas.utils`:
  - Lazy-loading and robust JSON parsing for dataset loading.
  - Input validation and type hints across public functions.
  - Fuzzy and partial search for LGAs and states using `difflib`.
  - Normalization helper to centralize string handling.
- Packaging improvements:
  - Added `pyproject.toml` for modern builds.
  - `setup.py` enhanced with `long_description`, `keywords`, `project_urls`, and `console_scripts` entry point.

```markdown
# Release v1.0.4

Release date: 2025-12-20

Summary
- Minor feature release introducing a small CLI and improvements to data loading and search.

Notable changes
- Added CLI: `nigeria-states-lgas` — terminal interface to list states, list LGAs, and search.
- `nigeria_states_lgas.utils`:
  - Lazy-loading and robust JSON parsing for dataset loading.
  - Input validation and type hints for public APIs.
  - Fuzzy and partial search for LGAs and states (powered by `difflib`).
  - Centralized name normalization helper.
- Packaging and metadata:
  - Added `pyproject.toml` for modern builds and updated `setup.py` metadata.
  - Console entry point `nigeria-states-lgas` registered.

Compatibility
- Minimum Python version requirement increased to `3.7`.

Files changed (high level)
- `nigeria_states_lgas/utils.py`
- `nigeria_states_lgas/cli.py`
- `setup.py`, `pyproject.toml`
- `README.md`, `tests/test_utils.py`

Notes
- This is a non-breaking minor release; existing public APIs remain compatible, though projects using Python <3.7 should upgrade their runtime.

```
