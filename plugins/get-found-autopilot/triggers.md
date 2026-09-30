# Event Triggers

Missions don't only run on schedule. These events can wake a mission outside its
heartbeat cadence.

## Schedule triggers

| Cadence | Watches |
| --- | --- |
| Daily | New leads, new reviews, approval queue age, speed-to-lead breaches |
| Weekly | Ranking movement, content calendar, KPI dashboard |
| Monthly | Visibility Score re-audit, budget vs. forecast, channel mix |

## Event triggers

| Event | Response |
| --- | --- |
| New lead arrives | Speed-to-lead check; draft follow-up (queued for approval unless T2-cleared) |
| New review posted (any rating) | Draft reply within 24h (queued for approval) |
| 1-star review | Immediate owner alert + draft response (never auto-post) |
| Ranking drop on a top-10 term | Diagnose: technical, content, or competitor cause; report, don't panic |
| Competitor launches visible campaign | Gap analysis via Scout skills; propose counter-moves |
| Approval queue item older than 48h | Nudge the owner with a one-line summary |

## Manual triggers

The owner can always wake a mission with: "Run [mission] now" or "Check [signal]".

## Guardrails

- Event triggers never bypass the approval queue for irreversible actions.
- The Scout tier only ever observes and plans — its triggers produce reports.
- Rate-limit: the same trigger fires at most once per hour per mission.
