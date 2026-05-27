---
paths:
  - "src/api/**/*.ts"
  - "src/routes/**/*.ts"
---

# API Design Rules

- All endpoints must validate input with Zod schemas
- Return shape: `{ data: T } | { error: string }`
- Rate limit all public endpoints
- Never expose internal error messages to clients
