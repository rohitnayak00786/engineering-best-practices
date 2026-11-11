# AI Engineering Practices
- Define task boundaries, input/output contracts and success criteria before introducing model calls.
- Treat prompts, retrieval content and tool outputs as untrusted; mitigate prompt injection.
- Never expose secrets, customer data or privileged instructions in model inputs or logs.
- Bound tool access, permission scope, retries and costs; require human approval for consequential actions.
- Validate structured outputs and handle failed or malformed model responses.
- Keep agent flows simple; avoid unnecessary chained agents or complex memory infrastructure.
- Use reproducible evaluations for behavior changes; record important prompt/model changes and tradeoffs.
