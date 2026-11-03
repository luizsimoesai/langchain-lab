# langchain-lab

Tutorials, course notes and experiments with [LangChain](https://python.langchain.com), [LangGraph](https://langchain-ai.github.io/langgraph/) and Deep Agents.

This repository is the companion code for my learning journey and for the content I publish about it. Everything here is written in English.

## Repository layout

| Folder | What it contains |
| --- | --- |
| [`academy/`](academy/) | Notes and exercises following external courses (for example LangChain Academy). Each course is an isolated project. |
| [`tutorials/`](tutorials/) | Original, self-contained tutorials. Each one is meant to be cloned and run on its own. |
| [`notes/`](notes/) | Loose studies, drafts and experiments. Shares one environment at the repository root. |
| [`shared/`](shared/) | Small helpers reused across tutorials. |

## Getting started

This project uses [uv](https://docs.astral.sh/uv/) and Python 3.12+.

```bash
git clone <this-repo-url>
cd langchain-lab

cp .env.example .env     # add your API keys
uv sync                  # creates .venv for the shared environment (notes/)
```

Tutorials and academy courses are isolated. Enter the folder and sync there:

```bash
cd tutorials/<tutorial-name>
uv sync
uv run python main.py
```

## Conventions

- **Language:** all code, comments, docs and commit messages are in English.
- **Naming:** lowercase folder names with hyphens. Tutorials are numbered in publishing order (`01-first-agent`).
- **Environments:** one `.venv` per tutorial and per academy course. `notes/` uses the root environment.
- **Secrets:** keep keys in `.env` (ignored by git). Update `.env.example` when a new variable is needed.
- **Style:** `uv run ruff check .` and `uv run ruff format .` from the repository root.

## Credits and licensing

Original work in this repository is released under the [MIT License](LICENSE). Material in `academy/` is derived from third-party courses; each course folder links to its source and keeps the original license.
