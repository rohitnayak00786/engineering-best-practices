# User Guide — Engineering Best Practices

## Why this exists
AI coding assistants can make changes quickly, but may over-engineer fixes, overlook existing conventions or lose earlier context. These portable rules encourage **small, understandable, secure, tested changes** across different AI tools and developers.

## Benefits
- More consistent engineering quality and easier reviews.
- Smaller diffs and fewer unrelated modifications.
- Clearer recovery after context-window loss or team handoffs.
- Brief explanations of **why** important decisions were made, alongside Git's record of **what** changed.

## Getting started
1. Choose an engineering folder from this repository.
2. Copy **everything inside it** (not the outer folder) into the root of your target project.
3. Tell your agent: **Read AGENTS.md and follow its referenced practices.**
4. Review the result, test reports and relevant change-history notes before approving code.

## What is included?
- `AGENTS.md`: general entry point used by many coding agents.
- `CLAUDE.md`: Claude Code pointer to the same rules.
- `best-practices/`: focused rules for coding, the engineering domain, testing, security and workflow.
- `docs/changes/INDEX.md`: short running index of verified decisions and current work.
- `docs/changes/_TEMPLATE.md`: optional concise record for meaningful work.

## Example
If an Airflow ingestion retry duplicates records, the agent first reads the existing DAG and incremental-load code, then fixes only the failure path, tests replay/idempotency and writes a short note explaining the cause and tradeoff. It should **not** rewrite unrelated pipelines or introduce a new orchestration framework.

## How does history work?
Git captures actual diffs. Change notes explain decisions and outstanding risks. For trivial changes, no note is needed; for a substantial feature or incident, create one dated file and link it from INDEX.md. Avoid sensitive data, unverified claims or huge logs.

## Frequently asked questions
**Do we need new software?** No; only Markdown and the existing Git repository.

**Does every change need documentation?** No. Only meaningful decisions or changes needing future context.

**Will every AI tool automatically obey?** Not guaranteed. Explicitly request the agent to read AGENTS.md; check tool compatibility and review the result.

**Do rules replace human review or tests?** No. Developers remain responsible for security, correctness, policy compliance and merging.

**Should old notes override current code?** Never; inspect repository state and recent Git history first.

## Team ownership
Keep guidance short. When a mistake recurs, improve the relevant rule; don't keep adding more tools or boilerplate.
