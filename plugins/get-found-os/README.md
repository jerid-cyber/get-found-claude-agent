# get-found-os (v1.0.0)

The complete Get-Found operating system. All 100 skills plus 9 department agents.

## Contents

- **100 skills** in `skills/` (each a standalone Claude Skill)
- **3 core skills** in `core-skills/`: command-center (orchestrator), business-brain (setup), heartbeat (scheduling)
- **9 agents** in `agents/`
- **Event triggers** (`triggers.md`) and the **approval queue** (`approval-queue.md`)

## Install

Unzip `dist/get-found-os.zip` and install the folder as a Claude plugin, or copy individual `skills/<name>` folders into Claude via Settings > Capabilities > Skills.

## Authority model

Agents execute within set limits. Irreversible actions (spending, publishing, changing listings) are queued for owner approval. An action type earns auto-approval only after 3 unchanged approvals in a row, and the owner can revoke it any time.

## License

Copyright (c) 2026 Jerid Wempen / TitanOne. All rights reserved.
