# Prometheus System Architecture

Prometheus is an explainable AI financial intelligence platform powered by Orion, a modular financial reasoning engine. This public architecture document describes the system at a portfolio level without exposing proprietary prompts, private implementation details, credentials, or user data.

## System Context

```mermaid
flowchart LR
    U[User] --> W[Prometheus Web App]
    W --> A[Authenticated API Layer]
    A --> O[Orion Financial Intelligence]
    A --> D[(PostgreSQL)]
    O --> M[Memory OS]
    O --> G[Guardrails and Validation]
    O --> K[Finance Knowledge and Formula Engines]
    O --> P[Market and Economic Data Providers]
    O --> H[Heartbeat and Daily Brief Services]
    P --> AV[Alpha Vantage]
    P --> FH[Finnhub]
    P --> FR[FRED]
    P --> SEC[SEC EDGAR]
```

## Application Layers

```mermaid
flowchart TB
    subgraph Client[Experience Layer]
      UI[React and TypeScript Interface]
      MM[Money Map]
      CHAT[Orion Conversation]
      MI[Market Intelligence]
      FL[Framework Library]
    end

    subgraph API[Application Layer]
      EX[Express API]
      AUTH[Supabase Authentication]
      ROUTES[Financial and AI Routes]
    end

    subgraph Orion[Orion Intelligence Layer]
      OE[Orion Engine]
      SD[Situation Detection]
      FE[Financial Engine]
      CF[Corporate Finance Engine]
      FORM[Formula Engine]
      ADV[Advisor Voice]
      VAL[Financial Validation]
      GR[Guardrails]
    end

    subgraph Data[Data and Services]
      DB[(PostgreSQL and Drizzle ORM)]
      MEM[Memory OS]
      HEART[Heartbeat Scheduler]
      BRIEF[Daily Brief Service]
      PROVIDERS[External Data Providers]
    end

    UI --> EX
    MM --> EX
    CHAT --> EX
    MI --> EX
    FL --> EX
    EX --> AUTH
    EX --> ROUTES
    ROUTES --> OE
    OE --> SD
    OE --> FE
    OE --> CF
    OE --> FORM
    OE --> ADV
    OE --> VAL
    OE --> GR
    OE --> DB
    OE --> MEM
    OE --> HEART
    OE --> BRIEF
    OE --> PROVIDERS
```

## Orion Request Lifecycle

```mermaid
sequenceDiagram
    actor User
    participant UI as Prometheus UI
    participant API as Express API
    participant Orion as Orion Engine
    participant Memory as Memory OS
    participant Safety as Guardrails
    participant Data as Financial Data Providers
    participant DB as PostgreSQL

    User->>UI: Submit a financial question
    UI->>API: Authenticated request
    API->>Orion: User message and application context
    Orion->>Safety: Validate request and risk boundaries
    Orion->>Memory: Load relevant user context
    Orion->>Data: Request permitted market or economic data
    Orion->>Orion: Detect situation and apply finance engines
    Orion->>Safety: Validate output and warnings
    Orion->>DB: Store permitted decision metadata
    Orion-->>API: Explainable response
    API-->>UI: Structured result
    UI-->>User: Guidance, assumptions, risks, and next steps
```

## Core Orion Modules

| Module | Responsibility |
|---|---|
| Orion Engine | Coordinates financial reasoning and response generation |
| Situation Detector | Classifies the user's financial situation and selects appropriate workflows |
| Financial Engine | Handles personal finance analysis and recommendations |
| Corporate Finance Engine | Supports valuation, capital budgeting, and business finance logic |
| Formula Engine | Performs deterministic calculations used in financial reasoning |
| Financial Validation | Checks assumptions, calculations, and output consistency |
| Guardrails | Applies safety boundaries and prevents overconfident financial claims |
| Advisor Voice | Produces clear, decision focused explanations |
| Memory OS | Stores and retrieves permitted long term user context |
| Heartbeat | Supports scheduled account and financial condition checks |
| Daily Brief | Produces structured financial and market summaries |

## Architectural Principles

1. **Explainability before automation.** Financial outputs should provide assumptions, reasoning summaries, risks, and next actions.
2. **Deterministic math where possible.** Calculations are separated from generative language to reduce numerical errors.
3. **Modular intelligence.** Knowledge, formulas, memory, providers, validation, and presentation remain separable.
4. **Server side trust boundary.** Provider keys, database access, and protected financial logic remain on the server.
5. **User scoped data.** Authentication and database controls are designed to keep one user's financial context isolated from another.
6. **Provider independence.** External market and economic data sources are wrapped behind provider modules.

## Public Showcase Boundary

This repository documents the product and its architecture. The complete Orion source, private prompts, production configuration, credentials, and user data are intentionally excluded from the public showcase.