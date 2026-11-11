# Engineering Best Practices

Reusable AI coding guidance organized by engineering discipline. Each folder is independent: copy its **contents** into your target repository root, then instruct your agent to read `AGENTS.md`.

| Folder | Scope |
| --- | --- |
| [data-engineering](data-engineering/) | SQL, Python, Spark, Airflow, Kafka and pipelines |
| [backend-engineering](backend-engineering/) | APIs, services and databases |
| [frontend-engineering](frontend-engineering/) | React, TypeScript and web UI |
| [devops-engineering](devops-engineering/) | CI/CD, containers, infrastructure and Kubernetes |
| [ai-engineering](ai-engineering/) | AI agents, prompts, tools and evaluations |

## Why
- Consistent, minimal, production-minded code changes.
- Relevant validation and secure development.
- Short engineering memory preserving **why** important decisions were made.
- Supports Claude Code and many other coding agents without additional infrastructure.

## Quick start
1. Open the folder for your discipline.
2. Copy every item inside it to the root of your project.
3. Say: **Read AGENTS.md and follow its practices throughout this task.**
4. Review the resulting code and tests. For important changes, the agent should update `docs/changes/`.

These files are templates; add project-specific details only after verifying the actual project. Follow your organization's policies and review requirements.
