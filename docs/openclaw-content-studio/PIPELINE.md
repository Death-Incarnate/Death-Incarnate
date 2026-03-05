# Autonomous Pipeline

## Trigger modes

1. Scheduled trend cycle (e.g., every 2 hours)
2. Manual topic submission
3. Batch import (CSV/API)

## Stage-by-stage

1. **Trend ingestion**
   - Pull trends from configured sources.
   - Score by niche relevance and likely watch-through.
2. **Topic selection**
   - Select candidates by policy + strategy mix (trending/evergreen/experimental).
3. **Hook + script generation**
   - Produce short-form script format with CTA.
4. **Scene planning**
   - Convert script into scenes with per-scene visual prompts.
5. **Asset generation**
   - Nano Banana 2 for image assets.
   - TTS for scene voice tracks.
   - Timed captions from script.
6. **Composition mapping**
   - Attach assets to Remotion template contract.
7. **Rendering**
   - Platform variants: 9:16, 1:1, 16:9.
8. **Publishing**
   - Upload to YouTube/TikTok/Instagram/X adapters.
9. **Analytics loop**
   - Pull metrics and write strategy hints for next cycle.

## Queue topology

- `trend_queue`
- `script_queue`
- `scene_queue`
- `asset_queue`
- `render_queue`
- `publish_queue`
- `analytics_queue`
