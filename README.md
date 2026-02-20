# Static Site Generator

A static-site generator written in Python. It converts Markdown files in `content/` into HTML pages under `docs/` using `template.html` and utilities in the `src/` package.

**Features**
- Simple Markdown -> HTML conversion using project utilities
- Maintains directory structure from `content/` into `docs/`
- Includes a small test suite for core modules in `src/`

**Quick Start**

Prerequisites:

- Python 3.8 or newer

To build the site (simple):

```
./main.sh
```

Or run the generator directly with Python:

```
python3 -m src.main
```

Run the tests:

```
./test.sh
```

Or with pytest:

```
pytest -q
```

**Repository layout**

- `content/` — source Markdown content
- `src/` — Python source for the generator
- `docs/` — generated output (committed here for convenience)
- `static/` — static assets copied into the output
- `template.html` — HTML template used for pages
- `main.sh`, `build.sh` — small helper scripts

**Development**

1. Create or edit Markdown files under `content/`.
2. Run `./main.sh` to generate `docs/`.
3. Run tests with `pytest` to verify behavior.
