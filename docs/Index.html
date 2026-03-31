<div align="center">

<img src="assets/prometheus-logo.png" alt="Prometheus AI Logo" width="140" />

# Prometheus AI

### Intelligent Financial Planning — Powered by the Orion Engine

[![Live App](https://img.shields.io/badge/Live%20App-Open%20Prometheus-f59e0b?style=for-the-badge&logo=rocket)](https://workspace.rasheekf.replit.app)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178c6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![React](https://img.shields.io/badge/React-18-61dafb?style=for-the-badge&logo=react&logoColor=white)](https://react.dev)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Drizzle%20ORM-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://orm.drizzle.team)
[![Express](https://img.shields.io/badge/Express-5.x-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com)

**[→ Try the Live App](https://workspace.rasheekf.replit.app)**

*Private Beta — request access to explore the full platform*

</div>

---

## What Is Prometheus?

Prometheus is a full-stack financial intelligence platform built for people who want to understand and act on their money — not just track it.

At its core is **Orion**, an AI financial strategist that holds a complete memory of your financial profile. You never re-explain your situation. Orion reasons across your debt, income, savings goals, and investments and gives you specific, step-by-step answers — not generic advice.

> Think Bloomberg Terminal, built for the everyday person.

---

## Live Demo

**[https://workspace.rasheekf.replit.app](https://workspace.rasheekf.replit.app)**

The app is mobile-first. Open the link on any device and explore:

- Chat with Orion about debt payoff, investing, and budgeting
- Run a FIRE retirement projection with your actual numbers
- Browse the Investor Framework Library (Graham, Dalio, Lynch, and more)
- View live market quotes and macro indicators
- Generate a personalized wealth strategy with an AI decision engine

---

## Feature Overview

### Orion AI Chat
Orion is not a chatbot wrapper. It uses a custom domain routing engine that detects the type of financial question, selects the right formula library, runs step-by-step calculations, and returns a structured answer with worked math.

- Debt payoff calculations (avalanche, snowball, hybrid)
- FIRE number and retirement timeline projections
- Budget analysis and savings rate optimization
- Investment portfolio allocation review
- Net worth tracking and wealth structure scoring

### Memory OS
Orion remembers your full financial profile across every conversation. Income, debts, goals, timeline, and risk tolerance are stored and referenced automatically — no repetition required.

### Money Map
A guided onboarding and financial snapshot tool that builds your complete financial profile in one session. Results feed directly into every Orion conversation.

### Investor Framework Library
A curated, searchable database of 10 legendary investor philosophies — Benjamin Graham, Ray Dalio, Peter Lynch, Warren Buffett, and more. Each framework includes core principles, metrics, screening criteria, and a strategy card.

### Market Intelligence
Live and historical market data across 28 securities (20 stocks + 8 ETFs) and 6 macroeconomic series (Fed Funds Rate, CPI, GDP, Unemployment, M2, 10-Year Treasury). Data sourced via Alpha Vantage and FRED APIs with PostgreSQL caching.

### Strategy Engine
An AI-powered decision engine that analyzes your financial profile alongside real market conditions and investor framework logic to generate a personalized, actionable wealth strategy.

### Scenario Modeling
Run side-by-side comparisons of financial decisions — pay off debt vs. invest, lump sum vs. DCA, aggressive vs. conservative allocation — with projected outcomes.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18, TypeScript, Vite, TailwindCSS |
| UI Components | Radix UI, shadcn/ui |
| Animations | Framer Motion |
| Charts | Recharts |
| Backend | Express 5, TypeScript, Node.js |
| Database | PostgreSQL (Replit-hosted), Drizzle ORM |
| AI | OpenAI API (custom reasoning engine) |
| Market Data | Alpha Vantage, FRED (Federal Reserve), SEC EDGAR |
| Auth | Session-based with secure middleware |
| Monorepo | pnpm workspaces with shared type libraries |
| Deployment | Replit Autoscale |

---

## Architecture

```
workspace/
├── artifacts/
│   ├── prometheus-ai/       # React + Vite frontend
│   │   ├── src/
│   │   │   ├── pages/       # Chat, Library, Market, Strategy, FIRE, etc.
│   │   │   ├── components/  # UI components (Orion chat, cards, nav)
│   │   │   └── hooks/       # API client hooks (React Query)
│   │   └── public/          # Static assets and walkthrough videos
│   └── api-server/          # Express backend
│       └── src/
│           ├── routes/      # /api/frameworks, /api/market, /api/strategy
│           ├── services/    # Orion engine, market providers, FRED client
│           └── db/          # Drizzle schema + seed data
└── lib/
    ├── db/                  # Shared Drizzle schema (types + tables)
    └── api-zod/             # Shared Zod validators + TypeScript types
```

**Deployment model:** A single Express process serves both the API (`/api/*`) and the compiled React frontend (SPA with fallback routing). No split static + dynamic architecture — one process, clean cold starts.

---

## Database Schema

| Table | Contents |
|---|---|
| `investor_frameworks` | 10 investor philosophies with principles, metrics, and strategy logic |
| `market_securities` | 28 tracked securities (stocks + ETFs) with sector metadata |
| `macro_series` | 6 FRED macroeconomic indicator definitions |
| `price_cache` | Cached quotes and macro data with TTL logic |
| `orion_decisions` | Persisted AI strategy decisions per user session |
| `users` | User profiles, financial snapshots, Memory OS state |
| `conversations` | Full Orion conversation history per user |
| `messages` | Individual messages with role, content, and metadata |

---

## Design System

- **Color palette:** Deep navy background (`hsl(226, 49%, 8%)`) with amber/orange accents — the Orion signature
- **Typography:** Bricolage Grotesque (display) + Manrope (body)
- **Component library:** shadcn/ui primitives with custom Prometheus theming
- **Motion:** Framer Motion for page transitions, chat streaming, and onboarding sequences
- **Layout:** Fully responsive — sidebar on desktop, bottom nav on mobile

---

## Key Engineering Decisions

**Custom AI reasoning engine over plain chat completion**
Rather than sending raw user messages to the LLM, Orion uses a domain routing layer that classifies the question type, selects the appropriate formula set, pre-calculates numerical results, and sends structured context to the model. This produces more accurate, reproducible financial answers.

**Monorepo with shared type library**
All API request/response shapes are defined once in `lib/api-zod` and consumed by both the Express routes and the React hooks. No type drift between frontend and backend.

**PostgreSQL caching for market data**
Third-party API calls (Alpha Vantage, FRED) are cached in PostgreSQL with configurable TTLs. This keeps the app fast and prevents rate-limit issues without a separate caching layer.

**Single-process production deployment**
In production, Express serves both the compiled React app and the API from one process. This eliminates cold-start race conditions common in split static/dynamic deployment architectures.

---

## About

Built by **Rasheek Felder** as a demonstration of full-stack AI product engineering — from database schema and API design through to a production-deployed, mobile-first user interface.

**[View the live app →](https://workspace.rasheekf.replit.app)**

---

<div align="center">

*Prometheus AI — private beta*

[![Open App](https://img.shields.io/badge/Open%20App-workspace.rasheekf.replit.app-f59e0b?style=for-the-badge)](https://workspace.rasheekf.replit.app)

</div>
