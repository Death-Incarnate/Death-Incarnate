# Database Schema (Proposed)

## users

- `id` (pk)
- `email` (unique)
- `api_keys_json`
- `created_at`

## templates

- `id` (pk)
- `name`
- `platform`
- `ratio` (9:16, 1:1, 16:9)
- `composition_key`
- `settings_json`
- `created_at`

## content_jobs

- `id` (pk)
- `user_id` (fk users)
- `topic`
- `hook`
- `script_json`
- `status`
- `template_id` (fk templates)
- `error_message`
- `created_at`
- `updated_at`

## generated_assets

- `id` (pk)
- `job_id` (fk content_jobs)
- `asset_type` (image, audio, subtitle, scene_json)
- `url`
- `metadata_json`
- `created_at`

## platform_exports

- `id` (pk)
- `job_id` (fk content_jobs)
- `platform` (youtube, tiktok, instagram, x)
- `video_url`
- `status`
- `published_url`
- `published_at`
- `created_at`

## batch_jobs

- `id` (pk)
- `name`
- `status`
- `strategy_json`
- `created_at`

## batch_job_items

- `id` (pk)
- `batch_id` (fk batch_jobs)
- `job_id` (fk content_jobs)
- `status`
- `created_at`
