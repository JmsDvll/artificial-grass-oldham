# Pipeline queue PR (Orchestrator wake)

**PR:** #24 — [Pipeline queue (orchestrator wake)](https://github.com/JmsDvll/artificial-grass-oldham/pull/24)

Bootstrap keeps one **draft PR** open (branch `cursor/pipeline-queue-wake`, **no** `cursor-job` label).

- **Overseer** adds **`orchestrator-wake`** on this PR after seeding tickets.
- **Orchestrator** wakes, opens the next real `cursor-job` ticket PR, then removes `orchestrator-wake` here.
- **Worker / QA never implement this PR** — it is only a doorbell.

Matches Cursor UI: Orchestrator label trigger on **pull requests** (`pullRequests: true`).