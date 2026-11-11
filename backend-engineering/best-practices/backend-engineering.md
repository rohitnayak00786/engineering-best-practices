# Backend Engineering Practices
- Preserve API contracts, status codes, authentication and response shape unless requirements say otherwise.
- Validate input; enforce authorization at the boundary; use parameterized queries.
- Follow existing service, persistence and error-handling patterns; avoid new layers without need.
- Keep state changes transaction-safe and retry-safe where appropriate.
- Avoid unbounded scans, N+1 queries and surprising destructive schema migrations.
- Log useful operational errors without secrets or sensitive payloads.
- Test normal paths, invalid inputs, permissions, errors and compatibility.
