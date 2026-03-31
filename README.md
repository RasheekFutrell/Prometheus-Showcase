<div align="center">

<img src="assets/prometheus-logo.png" alt="Prometheus AI" width="120" />

# Prometheus AI

**Intelligent financial planning — powered by the Orion reasoning engine**

[![Try the Demo](https://img.shields.io/badge/▶%20Try%20the%20Interactive%20Demo-f59e0b?style=for-the-badge&logoColor=white)](https://rasheekf.github.io/workspace/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![React](https://img.shields.io/badge/React-19-61dafb?style=for-the-badge&logo=react&logoColor=white)](https://react.dev)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Drizzle%20ORM-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://orm.drizzle.team)
[![Express](https://img.shields.io/badge/Express-5.x-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com)

---

### [→ Live Interactive Demo](https://rasheekf.github.io/workspace/)
*Chat with Orion, see real financial math, no login required — works on any device*

---

</div>

## What Is Prometheus?

Prometheus is a full-stack financial intelligence platform. Users describe their financial situation in plain English and the Orion engine figures out what they're actually asking — then answers with step-by-step math, relevant frameworks, and actionable guidance.

It's not a chatbot that gives generic advice. It's a reasoning system that runs real calculations.

---

## Interactive Demo

The demo at **[rasheekf.github.io/workspace](https://rasheekf.github.io/workspace/)** is a fully static walkthrough that runs in your browser with no server, no login, and no setup. It shows Orion working through four real financial scenarios:

| Scenario | What Orion calculates |
|---|---|
| Debt-to-income analysis | Monthly income → DTI ratio → lender thresholds |
| Debt payoff vs. investing | After-tax return comparison with real numbers |
| FIRE projection | Savings rate → retirement timeline using the 4% rule |
| Portfolio allocation | Age-based equity/bond split with risk adjustment |

All numbers are worked out step-by-step — the same logic the full app runs on.

---

## Core Features

**Orion Reasoning Engine**
- Classifies financial questions by domain (personal finance, corporate finance, market analysis)
- Routes to specialised formula handlers — DTI, amortisation, NPV, FIRE, Black-Scholes
- Shows full calculation steps, not just answers
- Explains *why* each number matters in plain language

**Investor Framework Library**
- 10 frameworks seeded: Graham, Buffett, Dalio, Lynch, Bogle, Munger, and more
- Each framework includes core principles, decision rules, risk warnings, time horizon, and suitability rating
- Filterable by category, risk level, and experience level

**Market Intelligence**
- 28 tracked securities (20 stocks + 8 ETFs) across sectors
- Live quotes via Alpha Vantage and Finnhub (free tier, 5-min cache)
- 6 macro series via FRED (Fed Funds Rate, CPI, unemployment, GDP, yield curve)

**Savings & Strategy Planner**
- Goal-based savings calculator with compound interest projections
- Orion decision engine scores strategies against user risk profile
- Recommended actions ranked by expected impact

**Memory OS**
- Orion remembers facts across conversations (income, debts, goals, risk tolerance)
- Context is used to personalise every answer without the user repeating themselves

**Private Beta Gate**
- Access code required on entry (`ORION-2025`)
- Inline onboarding collects name, income, and primary financial goal
- Hidden admin panel at `/x-admin` for session review

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 19, TypeScript, Tailwind CSS v4, Framer Motion |
| Backend | Express 5, TypeScript, Node.js |
| Database | PostgreSQL, Drizzle ORM |
| AI / Logic | Custom Orion reasoning engine (no external AI API) |
| Data APIs | Alpha Vantage, FRED, Finnhub, SEC EDGAR |
| Monorepo | pnpm workspaces, shared type packages |
| Deploy | Replit Autoscale |

---

## Project Structure

```
workspace/
├── artifacts/
│   ├── prometheus-ai/      # React frontend (Vite)
│   └── api-server/         # Express backend
├── lib/
│   ├── db/                 # PostgreSQL schema + Drizzle client
│   ├── api-spec/           # OpenAPI spec
│   ├── api-zod/            # Shared Zod validators
│   └── api-client-react/   # React Query hooks
└── docs/
    └── index.html          # Static GitHub Pages demo
```

---

## API Endpoints

```
GET  /api/healthz                    Health check
POST /api/beta/verify                Beta access code validation
POST /api/orion/chat                 Orion reasoning engine
GET  /api/frameworks                 All investor frameworks
GET  /api/frameworks/:slug           Single framework detail
GET  /api/market/watchlist           Securities + cached prices
GET  /api/market/quote/:symbol       Live quote (Alpha Vantage)
GET  /api/market/macro               FRED macro series
GET  /api/market/news/:symbol        Recent news (Finnhub)
GET  /api/strategy/decision          Orion strategy recommendation
```

---

## Running Locally

```bash
# Install dependencies
pnpm install

# Set environment variables
DATABASE_URL=postgresql://...
ALPHA_VANTAGE_API_KEY=...
FINNHUB_API_KEY=...
FRED_API_KEY=...

# Push database schema
pnpm --filter @workspace/db run push

# Start both servers
pnpm --filter @workspace/api-server run dev
pnpm --filter @workspace/prometheus-ai run dev
```

---

<div align="center">

Built by Rasheek · [Interactive Demo](https://rasheekf.github.io/workspace/)

</div>
