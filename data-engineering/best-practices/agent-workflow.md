# Agent Workflow and Engineering Memory
## Before coding
1. Read AGENTS.md, relevant practices and docs/changes/INDEX.md.
2. Check actual repository state, Git status and existing code before trusting old notes.
3. Identify the smallest safe implementation and tests.
## During coding
- Respect existing conventions, avoid unrelated changes, and preserve user work.
- Write or update focused tests and inspect the final diff.
## After coding
- Trivial edits: no new change note.
- Small fixes: optionally summarize in docs/changes/INDEX.md.
- Meaningful features, significant bugs or design decisions: create one dated docs/changes/YYYY-MM-DD-topic.md using _TEMPLATE.md and link it from INDEX.md.
- Record why, what, key files, checks actually run and remaining work.
- Keep INDEX.md around 50 lines. Git is the source of truth for the code; notes explain decisions, not replace code inspection.
## Recovering after context loss
Read AGENTS.md, INDEX.md, only relevant dated notes, then inspect current Git/code before resuming. Never treat documentation as more authoritative than current code.
