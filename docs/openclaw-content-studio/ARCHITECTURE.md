# Architecture

## 1) High-level flow

```text
Trend Source(s)
  -> OpenClaw Orchestrator
     -> Trend Agent
     -> Hook Agent
     -> Script Agent
     -> Scene Planner Agent
  -> Asset Generation Layer
     -> Nano Banana 2 (images)
     -> TTS (voiceover)
     -> Caption timing
  -> Remotion Renderer
  -> Platform Export Adapters
  -> Analytics Ingestion + Optimization Agent
```

## 2) Service boundaries

- **API service**: tRPC + auth + job creation + job status.
- **Agent workers**: queue-driven OpenClaw tasks.
- **Render workers**: Remotion bundle/render/upload.
- **Publisher workers**: platform-specific upload + retries.
- **Scheduler**: recurring trend scans and batch kicks.
- **Storage**: object storage for images/audio/video/subtitles.
- **DB**: Postgres for state and metadata.
- **Queue**: Redis/BullMQ for orchestration.

## 3) Key design principles

- Deterministic rendering (template + scene contract).
- Strict schema validation (Zod) at every hop.
- Idempotent queue workers (safe retries).
- Small reusable templates per platform ratio.
- Feedback loop that updates prompt strategy using performance data.
