# Installation and Local Development

This repository is a public product showcase. It does not contain the complete production application or proprietary Orion implementation. The instructions below document the expected development workflow for the private Prometheus application repository.

## Prerequisites

- Node.js 20 or newer
- npm 10 or newer
- PostgreSQL 15 or newer
- A Supabase project for authentication
- Approved credentials for any enabled AI, market, or economic data providers

## Expected Setup

```bash
git clone <private-prometheus-repository-url>
cd prometheus-financial-ai
npm install
cp .env.example .env
npm run db:migrate
npm run dev
```

## Environment Configuration

A private deployment may require variables in the following categories:

```text
DATABASE_URL=
SUPABASE_URL=
SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=
AI_PROVIDER=
OPENAI_API_KEY=
ANTHROPIC_API_KEY=
GEMINI_API_KEY=
ALPHA_VANTAGE_API_KEY=
FINNHUB_API_KEY=
FRED_API_KEY=
SESSION_SECRET=
```

Only variables required by the selected deployment should be configured. Service role keys and provider secrets must remain server side.

## Development Commands

| Command | Purpose |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Produce a production build |
| `npm run typecheck` | Validate TypeScript types |
| `npm test` | Run automated tests |
| `npm run db:migrate` | Apply database migrations |
| `npm run db:studio` | Inspect development database records |

Actual command names may differ in the private application repository and should follow its `package.json` scripts.

## Validation Checklist

Before opening a pull request or deploying:

1. Run TypeScript validation.
2. Run unit and integration tests.
3. Build the frontend and server.
4. Confirm no `.env` files or secrets are staged.
5. Test authentication and user data isolation.
6. Test Orion chat, calculations, memory, Heartbeat, and Daily Brief workflows.
7. Review financial disclaimers and error handling.

## Deployment Model

The current public product is deployed through Replit. A production migration may separate the frontend, API, database, and scheduled services across specialized providers while retaining Orion as the shared intelligence layer.

## Troubleshooting

### Database connection failures

Confirm `DATABASE_URL`, network access, SSL settings, and migration status.

### Authentication failures

Confirm the Supabase project URL, public key, redirect URLs, and server side session validation.

### AI provider failures

Confirm the selected provider is enabled, the API key is server side, account limits are available, and request timeouts are configured.

### Missing market data

Confirm provider credentials and rate limits. Prometheus should degrade safely and explain when current data is unavailable rather than inventing values.