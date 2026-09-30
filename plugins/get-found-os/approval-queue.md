# Approval Queue

The approval queue is how the Get-Found agent system earns autonomy instead of
assuming it. Every action the agents propose lands in one of three lanes.

## Lanes

- **Auto (earned):** reversible, low-risk actions the owner has explicitly
  cleared for this mission (e.g., publishing a pre-approved content template).
- **Queue (default):** everything else. The agent prepares the work, shows the
  exact change, and waits.
- **Blocked:** irreversible or high-risk actions that always need the owner
  (spending money, deleting data, posting public replies, changing DNS/listings).

## How an action earns Auto lane

1. The same action type is proposed and approved unchanged 3 times in a row.
2. The owner explicitly promotes it: "auto-approve [action type] from now on."
3. The owner can demote any action back to Queue at any time, no questions asked.

## Queue item format

Each queued item shows: what, why, the exact change (draft/post/config),
reversibility, and a one-tap approve / edit / reject. Items older than 48h
trigger a nudge via the Heartbeat.

## Scout tier rule

The Scout agent diagnoses and plans ONLY. It never touches live accounts, so its
output is always reports and plans — nothing ever needs the Auto lane.
