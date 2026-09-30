# Tier Assignments — how the 100 skills were split

The source library (jerid-cyber/get-found-skills) does not label skills as
Scout vs Autopilot, so assignments were made by function and documented here.

## get-found-scout — 8 diagnostic / planning skills

Audits, research, gap analysis, and planning. These produce reports and plans,
never actions:

- get-found-visibility-audit
- conversion-leak-finder
- keyword-prompt-intent-research
- competitor-visibility-gap-report
- helpful-content-quality-audit
- owner-kpi-dashboard
- customer-journey-mapper
- ltv-cac-channel-mix

## get-found-autopilot — 50 execution skills

Optimizers, builders, launchers, and engines: the skills an agent can run
hands-on (GBP optimization, review engines, content engines, ad launchers,
nurture architects, etc.). Full list is in the tier's `.claude-plugin/marketplace.json`.

## get-found-os — all 100 skills

Every skill from the source library, including the 42 strategic, situational,
and governance skills reserved for the full system (e.g., platform-risk FMEA,
reputation crisis response, AI policy & data safety, multilingual SEO).

## Design decisions

- Scout and Autopilot skill sets are **disjoint**; OS is the union (all 100).
- The 3 core skills (command-center, business-brain, heartbeat), the 9
  department agents, event triggers, and the approval queue are shared by the
  Autopilot and OS tiers; Scout gets the core skills plus its own Scout agent
  (diagnose/plan only, never touches live accounts).
- To change assignments, edit `SCOUT_SKILLS` / `AUTOPILOT_SKILLS` in
  `build-marketplace.sh` and re-run it.
