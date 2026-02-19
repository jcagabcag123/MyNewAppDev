# My University Buddy (MUB)

Minimal NestJS scaffolding for the MUB project.

## Prerequisites

- Node.js 18+ (or the version specified in `.nvmrc`)
- npm 9+

## Install

```bash
cd apps/api
npm install
```

## Run

```bash
cd apps/api
npm start
```

The API will start on `http://localhost:3000`.

## API Example

### GET /api/hello

```bash
curl http://localhost:3000/api/hello
```

**Response:**
```json
{
  "message": "Hello from My University Buddy API"
}
```

---

See [docs/spec_001.md](docs/spec_001.md) for the full specification.
