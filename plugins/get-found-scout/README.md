# get-found-scout (v1.0.0)

Diagnose and plan only. 8 audit/research skills plus the Scout agent — it never touches live accounts.

## Contents

- **8 skills** in `skills/` (each a standalone Claude Skill)
- **3 core skills** in `core-skills/`: command-center (orchestrator), business-brain (setup), heartbeat (scheduling)
- **1 agents** in `agents/`
- **Event triggers** (`triggers.md`) and the **approval queue** (`approval-queue.md`)

## Install

Unzip `dist/get-found-scout.zip` and install the folder as a Claude plugin, or copy individual `skills/<name>` folders into Claude via Settings > Capabilities > Skills.

## Authority model

Scout observes and plans ONLY. It never touches live accounts — output is reports and plans, never actions.

## License

Licensed under the [PolyForm Internal Use License 1.0.0](LICENSE) — free to use for your internal operations, including at work; you may not distribute, share copies, or sell it. © 2026 Jerid Wempen / TitanOne.
