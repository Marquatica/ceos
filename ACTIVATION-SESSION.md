# EOS Activation Session — agenda (≈90 min, John + optionally Annie)

*Prepared 2026-06-10. The CEOS repo was bootstrapped April 26 with templates
only and never populated. This is the working session that fixes that. Run it
in Claude Code from this repo; the ceos-* skills drive each segment
interview-style. Nothing here requires preparation — answer questions, the
skills write the files.*

## Why this session

Without this data, every ceos-* skill is a no-op, the L10 has no agenda
inputs, and Mission Control → Goals stays empty. This is the single blocking
step for the whole EOS layer.

## Agenda

1. **V/TO core (40 min)** — run `/ceos-vto`.
   Minimum viable: 3-5 core values, core focus (purpose + niche), 1-year plan
   (revenue, profit, 3-7 measurables), and a rough 3-year picture. 10-year
   target can be a placeholder — don't stall on it.

2. **Accountability Chart (15 min)** — run `/ceos-accountability`.
   Seats for the real team: John, Annie, Mauricio, Wendy, Julio + Qompass
   (yes — give the AI agent layer a seat with defined roles; it does delivery
   work and the chart should say what it owns).

3. **Scorecard (15 min)** — run `/ceos-scorecard`.
   Pick 5-7 weekly numbers that already exist in dashboards (e.g. new leads
   across clients, ad spend pacing misses, content posts shipped vs plan,
   client health trips, pipeline value, AR aging). Rule: every metric must be
   pullable in <5 min or by an agent, or it will die.

4. **Q3 Rocks (15 min)** — run `/ceos-rocks`.
   2-4 rocks for the company, ≤3 per person. Candidates surfaced by the
   2026-06-10 audit: ship the Visitor Intelligence program; EOS operating
   rhythm itself (L10 + scorecard live 8 straight weeks); Qompass v2
   reporting reroute stable in production; pick from Operations → Projects,
   not new wishes.

5. **Close (5 min)** — commit everything (`git add data/ && git commit`),
   then run the first ClickUp mirror per [SYNC-CLICKUP.md](./SYNC-CLICKUP.md),
   and confirm the Tuesday L10 calendar slot.

## After the session

- Weekly: Tuesday L10 via `/ceos-l10` (uses this data), ending with the
  ClickUp mirror step.
- The weekly ClickUp hygiene audit (posts to #ops-health) will flag if Rocks
  in Mission Control → Goals drift from the repo.
