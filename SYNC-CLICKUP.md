# CEOS → ClickUp Mirror (hybrid model)

*Adopted 2026-06-10. This repo is the source of truth for EOS data. ClickUp
Mission Control is the team-visible mirror. The mirror is one-directional:
repo → ClickUp. Never edit Rocks/Scorecard in ClickUp directly.*

## What mirrors where

| CEOS source | ClickUp destination |
|---|---|
| `data/rocks/<quarter>/*.md` | **Mission Control → Goals** list (`901413183356`) — one task per Rock, assigned to its owner, due = quarter end |
| `data/scorecard/metrics.md` weekly numbers | Weekly summary message in **#ops-health** chat (`8cmr5c7-4694`) after each L10 |
| `data/vision.md` (V/TO) | ClickUp Doc "ClickUp Conventions" links to the repo; V/TO itself stays in git (review quarterly) |

## The manual step (end of every L10)

Run this as the last item of the Tuesday L10, in Claude Code from this repo:

> "Mirror this week's EOS state to ClickUp: upsert one task per active Rock in
> the Mission Control Goals list (name: `Rock: <title> [<quarter>]`, assignee:
> rock owner, due date: quarter end, description: latest status from the rock
> file), and post the scorecard summary table to #ops-health."

ClickUp access: ClickUp MCP in the main Claude Projects session, or the
ClickUp API with the Doppler token (`qompass/prd` → `CLICKUP_API_TOKEN`).

ClickUp user IDs for assignment: John 54022629 · Annie 82403375 ·
Mauricio 94207819 · Wendy 94201067 · Julio 88476874.

## Automation (later)

Once the L10 ritual has stuck for ~4 consecutive weeks, automate this as a
Trigger.dev job in Qompass v1 (`agents/`) that reads this repo on GitHub and
performs the same upsert. Do not build it before the habit exists — the
manual step doubles as the meeting's closing discipline.
