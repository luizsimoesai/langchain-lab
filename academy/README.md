# academy

Notes and exercises following external courses, such as LangChain Academy.

## Rules

- One folder per course, each an isolated `uv` project (own `pyproject.toml`, `uv.lock` and `.venv`).
- Each course folder has a `README.md` with a short summary, a link to the source and the original license.
- Keep third-party material clearly separated from my own notes. Original explanations and new examples belong in [`../tutorials`](../tutorials/).

## Template

```
academy/<course-name>/
├── README.md        # summary, source link, license
├── pyproject.toml
├── uv.lock
└── module-1/ ...
```
