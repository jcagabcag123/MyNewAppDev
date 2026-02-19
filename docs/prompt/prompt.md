# Prompt: Scaffold empty NestJS app

| Field | Value |
|-------|--------|
| **Purpose** | Scaffold MUB repo and minimal NestJS API from spec only; no extras. |
| **Spec** | [docs/spec_001.md](../spec_001.md) (Scaffold Spec v0.0.1) |
| **Created** | 2026-02-10 |
| **Outcome** | Repo structure (`apps/api`, `apps/web`, `packages/shared`), NestJS app in `apps/api`, `GET /api/hello`, global prefix `/api`, README with run + curl. |
| **Prerequisites** | Empty Git repo; `docs/spec_001.md` (or equivalent) defines structure and API. |
| **Related** | [README.md](../../README.md) (run instructions) |

---

You are working in an EMPTY Git repository for the project "My University Buddy (MUB)".
Your job is to implement ONLY the scaffold described in docs/spec_001.md (Scaffold Spec v0.0.1).
Do not add any extra endpoints, features, product/domain logic, database, auth, or tests unless explicitly required by the spec.

FIRST: Read and follow docs/spec_001.md strictly.

GOAL:

- Create the agreed repo folder structure
- Scaffold a minimal NestJS app in apps/api
- Add a single endpoint GET /api/hello returning JSON:
  { "message": "Hello from My University Buddy API" }
- Configure a global prefix so routes are under /api
- Create README.md with exact run instructions and a curl example

IMPORTANT EXECUTION RULES:

- You must ASK ME before running or suggesting any terminal commands that install dependencies or generate code (npm/pnpm/yarn, nest new, npx, etc.).
- When you need me to run a command, present it in a copy-paste block and explain briefly why.
- After I run commands, I will paste back the output; then you continue.

IMPLEMENTATION DETAILS:

1) Repo structure (create directories and placeholder files as needed):
   - docs/spec_001.md already exists (do not modify unless necessary)
   - create: apps/api, apps/web (empty placeholder), packages/shared (empty placeholder)
2) NestJS app:
   - Must live in apps/api
   - Use TypeScript
   - Use standard NestJS bootstrap (main.ts, app.module.ts, controller)
   - Add global prefix "/api" in main.ts
   - Create controller route "/hello" so final route is GET /api/hello
3) README.md must include:
   - prerequisites (Node.js)
   - install steps
   - run steps
   - how to call /api/hello (curl)
4) Keep everything minimal and readable.

OUTPUT FORMAT:

- Start by telling me what you will create/modify (file list).
- Then tell me the exact commands I should run to initialize NestJS under apps/api (choose npm or pnpm, but ask which one I use if you're unsure).
- After I run the commands, continue with the file edits needed to meet the spec.