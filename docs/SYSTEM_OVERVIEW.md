# System Overview

## Product Purpose

Prometheus is an AI powered financial intelligence platform designed to help individuals and future small business users understand financial choices, calculations, risks, and tradeoffs in plain language. Its central assistant, Orion, is designed as a real time personal CFO rather than a general purpose chatbot.

## Core User Experiences

| Experience | Purpose |
|---|---|
| Orion | Conversational financial analysis and decision support |
| Money Map | Financial position, goals, projections, and recommended actions |
| Framework Library | Structured investing and decision frameworks |
| Market Intelligence | Market, macroeconomic, and regulatory context |
| Savings and Strategy | Goal planning, allocation modeling, and risk aware guidance |
| Heartbeat | Proactive checks for meaningful financial changes |
| Daily Brief | Concise financial and market summaries |

## Engineering Highlights

- Modular TypeScript financial reasoning architecture
- Deterministic formula engine for financial calculations
- Separate validation and guardrail layers
- Long term memory architecture
- Multiple financial data provider adapters
- Scheduled Heartbeat and Daily Brief services
- PostgreSQL persistence with Drizzle ORM
- React and Vite client with an Express server
- Supabase based authentication model
- Explainability oriented response design

## What Makes the Project Different

Prometheus is designed around decisions rather than chat completion. Orion attempts to identify the user's situation, apply relevant finance logic, check calculations and risk boundaries, and then present understandable next steps.

The project also treats model governance as an engineering concern. Validation, explainability, user isolation, source limitations, and clear disclaimers are part of the system design rather than optional presentation details.

## Repository Scope

This public repository is a portfolio and product documentation layer. It contains product visuals and technical documentation but intentionally excludes:

- Production application source
- Proprietary Orion prompts and business logic
- Credentials and environment files
- Database exports and user records
- Internal deployment configuration

The public boundary allows recruiters and collaborators to evaluate the architecture and product thinking without exposing sensitive intellectual property.