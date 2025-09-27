# Pydantic AI – Unified Template

This folder consolidates:
- Claude Code subagent factory (automation/claude)
- Reference Pydantic AI agents and examples (agents/, examples/)
- Full Agent Application (services/backend + services/frontend)
- Pipelines (pipelines/rag)
- Deployment and infrastructure (deploy/)
- Advanced agent architectures (architectures/)
- Optional integrations (integrations/)

How to use:

- Claude Code subagents: open this `pydantic-ai/` folder in Claude Code. The `.claude/` directory is at the template root, and the orchestration guide is in `CLAUDE.md`. Generated agents will be created under `agents/<your_agent>/`.
- Backend API: see `services/backend/app_backend/` (dev) or `services/backend/agent_api_production/` (production + Langfuse). Use env blueprints in `deploy/blueprints/`.
- Frontend UI: see `services/frontend/app_frontend/` or `services/frontend/app_frontend_production/`. Configure API base URL via the frontend env.
- RAG pipelines: see `pipelines/rag/` for local and production ingestion.
- Deploy: run from `deploy/` — `render.yaml_production`, `cloudbuild.yaml`, and Terraform in `deploy/infra/`. Use `start_configuration.py` from within `deploy/` to create a `render.yaml` for your domains.
