# Deployment and Scaling

## Services

- `api`
- `agent-workers`
- `render-workers`
- `publish-workers`
- `scheduler`
- `postgres`
- `redis`
- `object-storage`

## Queue and scaling guidance

- Keep queues separate by stage.
- Make workers stateless and idempotent.
- Scale render workers horizontally for throughput goals.

## Throughput target

- Baseline: 1 render worker ~= 2 short videos/minute (template dependent)
- 10 workers ~= up to 1,000+ videos/day under stable load

## Reliability

- Dead-letter queue per stage
- Retry with exponential backoff
- Alert on failure-rate spike and queue lag
