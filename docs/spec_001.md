# My University Buddy (MUB) — Scaffold Spec v0.0.1

**Status:** Draft  
**Goal:** Create a minimal, runnable NestJS “Hello World” API project and commit it to the repo.

---

## 1) Scope

### In scope (only)

- Repository folder scaffold
- Minimal NestJS app in `apps/api`
- One endpoint that returns a hello message
- Basic README with run instructions

### Out of scope (explicitly not now)

- No product features, no domain model
- No database
- No authentication
- No testing requirements (optional later)
- No frontend implementation (placeholder folder only)

---

## 2) Repository structure

Create and commit the following structure:

```plain
mub/
  README.md
  docs/
    spec_001.md
  apps/
    api/
    web/              (placeholder folder only; empty is fine)
  packages/
    shared/           (placeholder folder only; empty is fine)
```

---

## 3) Technology constraints

- Language: TypeScript
- Runtime: NestJS
- Backend framework: NestJS (latest stable allowed)

---

## 4) API requirements (Hello World only)

Base URL prefix: `/api`

### Endpoint

- `GET /api/hello`

**Response:**

```json
{ "message": "Hello from My University Buddy API" }
```

---

## 5) Acceptance criteria (Definition of Done)

- [ ] Repository matches the structure defined above
- [ ] `docs/spec_001.md` exists and is committed
- [ ] `README.md` exists and includes:
  - prerequisites (Node.js version if needed)
  - install instructions
  - run instructions
  - example request to `/api/hello`
- [ ] NestJS application starts locally without errors
- [ ] `GET /api/hello` returns the expected JSON response

---

## 6) Notes for Cursor / agents (implementation guidance)

- Use the standard NestJS bootstrap (`main.ts`, `app.module.ts`)
- Configure a global prefix so routes are served under `/api`
- Keep the implementation minimal and readable
- Do not add extra endpoints or features

---

## 7) Next step (after this spec)

Once this scaffold is complete and committed:

1. Verify the app runs on all machines
2. Use this as the baseline for writing the first real product spec
3. Iterate deliberately in the next lab