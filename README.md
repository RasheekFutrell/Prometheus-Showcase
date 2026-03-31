<div align="center">

<img src="https://workspace.rasheekf.replit.app/images/orion-logo.png" alt="Prometheus Logo" width="80"/>

# Prometheus AI

### Intelligent Financial Planning · Powered by Orion Engine

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Try%20Prometheus-f59e0b?style=for-the-badge&logo=rocket)](https://workspace.rasheekf.replit.app)
[![Status](https://img.shields.io/badge/Status-Private%20Beta-orange?style=for-the-badge)]()
[![Stack](https://img.shields.io/badge/Stack-React%20%7C%20TypeScript%20%7C%20Express%20%7C%20PostgreSQL-blue?style=for-the-badge)]()

> **Access Code:** `ORION-2025` — Enter this on the landing page to explore the full app.

</div>

---

## What is Prometheus?

Prometheus is a full-stack financial intelligence platform that puts institutional-grade analysis in the hands of everyday investors. At its core is **Orion** — an AI financial strategist that reads your complete financial picture before answering any question, so you never have to re-explain your situation.

Think Bloomberg Terminal, but built for real people.

---

## Core Features

### Money Map
Your complete financial picture in one structured view — net worth, assets, liabilities, cash flow, and savings rate all live in one place. Orion reads your Money Map automatically before every conversation.

- Real-time net worth calculation across accounts
- Asset allocation breakdown (investments, home equity, cash)
- Monthly cash flow analysis with surplus tracking
- FIRE progress bar toward your retirement target
- Wealth Structure Score across 5 dimensions: Liquidity, Growth, Safety, Income, and Debt Load

### Orion AI Engine
Ask Orion anything about your finances. It reasons step-by-step using real financial formulas — not generic advice.

- Formula-backed calculations (WACC, FIRE, SWR 4% rule, debt ratios, IRR)
- Domain routing: routes questions to the right financial engine automatically
- Contextual memory: remembers your goals and past decisions across sessions (Memory OS)
- Scenario modeling: run what-if analyses on allocation shifts, debt payoff, income changes

### Savings Planner
A goal-based savings tool that calculates exactly how much you need to save per month to hit any target — with Orion explaining the math.

### Market Intelligence
Live market data and macro indicators powered by Alpha Vantage, FRED (Federal Reserve), and Finnhub APIs.

- Watchlist quotes with 5-minute refresh cache
- Fed funds rate, inflation, unemployment, and GDP data
- Market news aggregation

### Strategy Library
18 institutional investor frameworks (Buffett, Dalio, Graham, Lynch and more) with full methodology breakdowns — readable and searchable inside the app.

---

## Technical Highlights

| Area | Implementation |
|------|---------------|
| Frontend | React 19, TypeScript, Tailwind CSS v4, Vite |
| Backend | Node.js, Express, TypeScript |
| Database | PostgreSQL via Drizzle ORM (schema-first) |
| AI Engine | Custom domain-routing formula engine with Memory OS |
| Market Data | Alpha Vantage, FRED, Finnhub, SEC EDGAR APIs |
| Auth | Private beta gate with invite-code system |
| Deployment | Replit autoscale (static + API split architecture) |

---

## App Structure

```
prometheus/
├── frontend (React + Vite)
│   ├── Beta gate with invite-code authentication
│   ├── Orion chat interface
│   ├── Money Map dashboard
│   ├── Savings Planner
│   ├── Market data pages
│   └── Strategy library
│
└── backend (Express API)
    ├── /api/frameworks   — investor frameworks
    ├── /api/market/*     — live quotes, macro data, news
    ├── /api/strategy/*   — Orion decision engine
    └── /api/beta/*       — access code verification
```

---

## Try It Live

1. Visit **[workspace.rasheekf.replit.app](https://workspace.rasheekf.replit.app)**
2. Enter access code **`ORION-2025`**
3. Ask Orion: *"Should I pay off my student loan or invest the difference?"*

---

## Feature Walkthrough Videos

| Video | Description |
|-------|-------------|
| [Money Map Walkthrough](https://workspace.rasheekf.replit.app/money-map-walkthrough.mp4) | Full Money Map feature demo with Orion interaction |
| [Orion Interaction Demo](https://workspace.rasheekf.replit.app/orion-interaction.mp4) | Real FIRE + house affordability conversation |
| [Product Overview](https://workspace.rasheekf.replit.app/prometheus-linkedin.mp4) | 28-second product highlight reel |

---

## Status

This project is currently in **private beta**. The codebase is kept private while in active development. This repository serves as a public-facing showcase.

---

<div align="center">

Built with React · TypeScript · PostgreSQL · Express · Orion Engine

**[rasheekf.replit.app](https://workspace.rasheekf.replit.app)**

</div>
