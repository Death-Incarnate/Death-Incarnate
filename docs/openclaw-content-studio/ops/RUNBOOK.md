# Operations Runbook

## Daily checks

- Queue depth by stage
- Render failure percentage
- Publish failure percentage
- Median generation time per platform

## Common incidents

1. **Asset generation failures**
   - Check provider quota and response payload validation.
2. **Render timeouts**
   - Reduce scene count or split job; verify worker memory.
3. **Publish API errors**
   - Refresh platform tokens; check rate limits.

## Recovery

- Replay DLQ items by batch id.
- Re-run failed publish stage without full regeneration.
- Preserve immutable generation artifacts for auditing.
