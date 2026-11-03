# tutorials

Original, self-contained tutorials. Each one should run on its own after `uv sync`.

Looking for full applications with frontend, database and Docker? See [`../projects`](../projects/).

## Rules

- Folders are numbered in publishing order: `01-first-agent`, `02-human-in-the-loop`, ...
- Each tutorial is an isolated `uv` project with its own `pyproject.toml`.
- Each tutorial has a `README.md` covering what you will learn, prerequisites, how to run it and key takeaways.
- Code and docs are in English.

## Template

```
tutorials/NN-short-name/
├── README.md
├── pyproject.toml
├── main.py
└── notebook.ipynb   # optional
```

Create a new one with:

```bash
cd tutorials
uv init --app NN-short-name
```

## Index

| # | Tutorial | Topics |
| --- | --- | --- |
| – | _None yet_ | – |
