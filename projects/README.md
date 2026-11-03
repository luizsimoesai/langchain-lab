# projects

Complete, end-to-end use cases: backend, frontend, database and Docker. Each project shows how LangChain, LangGraph or Deep Agents fit into a real application.

For short, single-concept lessons, see [`../tutorials`](../tutorials/).

## Rules

- Folders are numbered in publishing order: `01-support-chatbot`, `02-research-assistant`, ...
- Each project is self-contained and runs with a single command: `docker compose up`.
- The focus stays on LangChain. Treat the frontend, database and Docker setup as infrastructure: show how it works, but do not turn the project into a React or Docker course.
- One frontend stack per project (for example Vite + React in one, Next.js in another).
- Pin dependency versions and note the date and main library versions in the project README, because these ecosystems change quickly.
- Keep secrets in `.env` only. Never bake keys into Docker images or the frontend bundle.
- Test from a clean clone before publishing.
- Code and docs are in English.

## Template

```
projects/NN-short-name/
├── README.md              # architecture, how to run, video link, versions
├── docker-compose.yml
├── .env.example
├── backend/               # uv project (FastAPI + LangChain) with its own Dockerfile
│   ├── pyproject.toml
│   ├── uv.lock
│   └── Dockerfile
├── frontend/              # Vite/React or Next.js with its own Dockerfile
│   ├── package.json
│   └── Dockerfile
└── db/                    # init scripts, migrations
```

The Python environment (`.venv`) lives in `backend/`. The frontend uses `package.json` and `node_modules`.

## Index

| # | Project | Stack | Topics |
| --- | --- | --- | --- |
| – | _None yet_ | – | – |

## Running a single project without cloning everything

```bash
npx degit luizsimoesai/langchain-lab/projects/NN-short-name my-project
cd my-project
cp .env.example .env
docker compose up
```
