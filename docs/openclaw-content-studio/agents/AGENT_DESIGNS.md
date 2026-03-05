# OpenClaw Agent Designs

## trend-agent

Input: source config + niche profile  
Output: scored topic candidates

## hook-agent

Input: selected topic  
Output: short hooks optimized for retention

## script-agent

Input: topic + hook + style guide  
Output: structured script with CTA and duration budget

## scene-agent

Input: script + platform ratio  
Output: scene plan and visual prompts for Nano Banana 2

## optimizer-agent

Input: performance metrics  
Output: prompt/template strategy updates

## Publisher agents

- youtube-publish-agent
- tiktok-publish-agent
- instagram-publish-agent
- x-publish-agent

All publisher agents must support idempotency keys and retry-safe publish operations.
