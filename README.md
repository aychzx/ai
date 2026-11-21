# ai

Agents, orchestration, and data engineering pipelines.

## Layout

| Folder | Purpose |
|---|---|
| `agentic/agents/` | One folder per agent (`_template/` to copy, `base/` for shared classes) |
| `agentic/orchestration/` | Multi-agent coordination: `workflows/`, `routing/`, `state/` |
| `agentic/tools/` | Tools agents can call |
| `agentic/prompts/` | Shared prompt templates |
| `DE/pipelines/` | Data engineering projects, each with `config/ main/ utils/ validation/ test/` |
| `DE/data/` | Local data (`raw/ staging/ processed/`), git-ignored |
| `shared/` | Code reused by both sides (LLM clients, logging, helpers) |
| `config/` | Global configuration |
| `tests/` | Cross-cutting and integration tests |
| `docs/` | Documentation |

## New pipeline
Copy `DE/pipelines/_template/` to `DE/pipelines/<name>/`.

## New agent
Copy `agentic/agents/_template/` to `agentic/agents/<name>/`.
