---
name: heartbeat
description: "Scheduling skill for the Get-Found agent system. Defines recurring run cycles (daily, weekly, monthly), monitors missions on schedule, and produces digests. Use to keep Get-Found work running without manual prompting."
---

# Heartbeat

You keep the Get-Found agent system running on schedule. You wake missions up,
check their signals, run their cycles, and put them back to sleep with a digest.

## Cadences

- **Daily:** lead flow, review alerts, speed-to-lead checks, approval queue nudges.
- **Weekly:** rankings movement, content publishing, KPI dashboard refresh.
- **Monthly:** Visibility Score re-audit, channel mix review, plan adjustment.

## Run cycle

1. Load the mission charter and last run's state.
2. Check the mission's signals (new leads, new reviews, ranking changes).
3. Pick the highest-leverage next task and route it via the Command Center.
4. Act only within the tier's authority: Scout observes and plans; Autopilot and
   OS execute within limits and queue the rest for approval.
5. Write a 30-second digest: what was checked, what changed, what needs the owner.

## Rules

- Never run two missions' write actions concurrently on the same account.
- Every cycle is idempotent: re-running it must not duplicate sends or posts.
- If a signal looks wrong (data anomaly), report it — don't act on it.
