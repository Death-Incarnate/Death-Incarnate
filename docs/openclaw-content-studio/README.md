# OpenClaw Content Studio Blueprint

This blueprint defines a **fully automated content creation studio** using:

- OpenClaw agent orchestration
- Remotion for deterministic video rendering
- Nano Banana 2 (Gemini image model) for visual generation
- Multi-platform export for YouTube, TikTok, Instagram, and X

## Deliverables in this folder

- `ARCHITECTURE.md` — system architecture and service boundaries
- `PIPELINE.md` — end-to-end autonomous generation flow
- `IMPLEMENTATION_PLAN.md` — phased buildout plan
- `TODO.md` — execution checklist
- `db/SCHEMA.md` — relational schema and table responsibilities
- `api/TRPC_ROUTERS.md` — API surface for templates/jobs/assets/exports
- `remotion/TEMPLATES.md` — composition patterns and platform format matrix
- `infra/DEPLOYMENT.md` — Docker, workers, queues, and scale targets
- `ops/RUNBOOK.md` — daily operations, retries, and incident handling
- `agents/AGENT_DESIGNS.md` — OpenClaw agent responsibilities and contracts

## Objective

Turn topic inputs (or trend sources) into rendered, captioned, voiceover videos, then publish and optimize automatically based on performance feedback.
