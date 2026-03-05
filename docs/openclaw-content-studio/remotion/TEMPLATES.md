# Remotion Templates

## Platform matrix

- YouTube Shorts: 1080x1920 (9:16), 30fps
- TikTok: 1080x1920 (9:16), 30fps
- Instagram Reels: 1080x1920 (9:16), 30fps
- Instagram Feed: 1080x1080 (1:1), 30fps
- X: 1280x720 (16:9) or 1080x1080 (1:1), 30fps

## Scene contract

Each scene should provide:

- `startFrame`
- `durationFrames`
- `imageUrl`
- `audioUrl`
- `captionText`
- `captionTiming[]`
- `motionPreset`

## Composition strategy

1. Load scene contract from DB/object storage.
2. Resolve URLs to local cache.
3. Render sequence per scene.
4. Apply subtitles and CTA overlay.
5. Export MP4 (H.264 + AAC).
