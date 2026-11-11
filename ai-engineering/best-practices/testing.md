# Testing and Validation
- Test changed behavior, not unrelated code.
- Include relevant edge cases (nulls, duplicates, errors, retries and empty results).
- Keep tests deterministic; use existing tooling and project conventions.
- For data changes, verify schemas, quality and idempotency where relevant.
- Run applicable tests, lint/type checks and build checks when possible.
- Never claim that a test passed unless it actually ran. State unverified risks.
