# Get-Found Agent Marketplace (v1.0.0)

Three tiers of the Get-Found AI agent system, built on the Top 100 Get-Found
skills library and the 4-Phase System (Discovery, Architecture, Implementation,
Optimization). Proprietary software by Jerid Wempen / TitanOne.

## Tiers

| Tier | Skills | Agents | What it does |
| --- | --- | --- | --- |
| **get-found-scout** | 8 diagnostic | 1 Scout agent | Diagnoses and plans ONLY. Audits, research, gap analysis, 90-day plans. Never touches live accounts. |
| **get-found-autopilot** | 50 execution | 9 department agents | Researches, builds, publishes after approval, monitors on schedule. |
| **get-found-os** | all 100 | 9 department agents | The complete system: every skill, every agent. |

All tiers share 3 core skills — **command-center** (orchestrator),
**business-brain** (setup), **heartbeat** (scheduling) — plus event triggers
and an approval queue.

## Install

Each tier ships as a zip in `dist/` (hidden `.claude-plugin` folders intact).
Unzip the tier you bought and install the folder as a Claude plugin, or install
individual skills from `plugins/<tier>/skills/<name>`.

New here? Read `GETTING-STARTED.md` first.

## Rules every tier enforces

1. **No baseline, no build.** Starting numbers are recorded before any work.
2. **Exposure is not the finish line.** Every workstream ends at a revenue signal.
3. **Approval queue.** Irreversible actions wait for the owner; autonomy is earned.

## License

Copyright (c) 2026 Jerid Wempen / TitanOne. All rights reserved.
This is proprietary software. It may not be copied, redistributed, or resold
without written permission.
