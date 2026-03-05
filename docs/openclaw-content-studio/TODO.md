# TODO Checklist

## Platform Core

- [ ] Initialize workspace and package boundaries
- [ ] Add shared type package for scene contracts
- [ ] Add centralized env/config loader

## Database

- [ ] Create core tables (templates, jobs, assets, exports)
- [ ] Add batch tables
- [ ] Add analytics tables
- [ ] Add indexes for status and created_at scans

## API

- [ ] templates router
- [ ] content router
- [ ] assets router
- [ ] batch router
- [ ] exports router
- [ ] analytics router

## Agents

- [ ] trend agent
- [ ] hook agent
- [ ] script agent
- [ ] scene planner agent
- [ ] optimizer agent

## Asset Generation

- [ ] Nano Banana 2 adapter
- [ ] TTS adapter
- [ ] caption timing service

## Rendering

- [ ] template pack (9:16, 1:1, 16:9)
- [ ] render queue worker
- [ ] preview render endpoint

## Publishing

- [ ] YouTube upload + metadata mapping
- [ ] TikTok upload flow
- [ ] Instagram Reels flow
- [ ] X media posting flow

## Ops

- [ ] failure alerting
- [ ] DLQ replay tooling
- [ ] daily quality review report
