# DevOps Engineering Practices
- Prefer small, reviewable, repeatable infrastructure and CI/CD changes.
- Separate development, staging and production; never apply destructive production changes without approval.
- Use approved secrets management, least-privilege identities and safe access boundaries.
- Favor secure, minimal container images and reproducible versions/configuration.
- For Kubernetes, check namespace, RBAC, resources, probes, volumes, rollout and rollback implications.
- Validate plans, manifest syntax, build/test jobs and nonproduction behavior where possible.
- Make rollback, downtime and migration risks clear in the change note.
