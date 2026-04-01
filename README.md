 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index f43b27ee95294239202f96eb1e1eb86717a7dbb6..30969515272527d0cdd05469e51faaef1eb151b3 100644
--- a/README.md
+++ b/README.md
@@ -1,105 +1,121 @@
-# Prometheus AI
+<p align="center">
+  <img src="./docs/orion-logo.png" alt="Prometheus AI Logo" width="120" />
+</p>
 
-> **Private Beta** — Intelligent financial reasoning powered by the Orion engine.
+<h1 align="center">Prometheus AI</h1>
+<p align="center"><strong>Financial Intelligence for Humanity</strong></p>
 
-[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-orange?style=for-the-badge)](https://rasheekfutrell.github.io/Prometheus-Showcase/)
-[![App](https://img.shields.io/badge/Full%20App-Replit-blue?style=for-the-badge)](https://workspace-rasheekf.replit.app)
+<p align="center">
+  Prometheus AI is an intelligent financial planning platform powered by Orion, a personalized AI financial strategist designed to help users build wealth with clarity, strategy, and confidence.
+</p>
+
+<p align="center">
+  <a href="https://rasheekfutrell.github.io/Prometheus-Showcase/">Live Demo</a> •
+  <strong>Private Beta</strong> •
+  React · TypeScript · Express · PostgreSQL
+</p>
 
 ---
 
-## What Is Prometheus?
+## Vision
 
-**Prometheus** is a full-stack financial intelligence platform built with React, TypeScript, and Express. At its core is **Orion** — a step-by-step financial reasoning engine that performs real calculations using your actual numbers, not generic advice.
+Prometheus AI was created to make high-level financial intelligence accessible to everyday people.
 
-Prometheus covers the full personal finance stack: debt analysis, FIRE projections, portfolio allocation, savings planning, and investment framework research — all in one place.
+Most people are surrounded by financial advice, but very few have access to a system that can translate numbers, behavior, goals, and strategy into clear action. Prometheus changes that.
 
----
+At the center of the platform is **Orion** — an explainable AI financial strategist built to help users understand their money, improve decision-making, and move with intention toward long-term wealth.
 
-## Features
+The long-term vision is to build a financial intelligence platform that feels personal, trusted, and scalable — a system that can eventually support individuals across mobile, web, and connected devices.
 
-| Module | Description |
-|---|---|
-| **Orion Chat** | AI financial engine — DTI, FIRE, debt vs invest, compound interest, budget, net worth |
-| **Framework Library** | 10 investor frameworks: Graham, Buffett, Dalio, Lynch, Bogle, Munger + more |
-| **Market Data** | Live quotes via Alpha Vantage + Finnhub, macro series via FRED |
-| **Savings Planner** | Goal calculator with compound growth projections and Orion commentary |
-| **Strategy** | Risk-profile portfolio allocator — Conservative / Moderate / Aggressive |
-| **Budget Tool** | 50/30/20 breakdown with personalized investment projections |
+## Meet Orion
 
----
+Orion is the reasoning engine behind Prometheus.
 
-## Tech Stack
+It is designed to be:
+- Explainable, not mysterious
+- Personalized, not generic
+- Strategic, not reactive
+- Supportive, not robotic
 
-**Frontend**
-- React 18 + TypeScript
-- Vite + Wouter (routing)
-- TanStack Query
-- Tailwind CSS + shadcn/ui
+Instead of giving shallow financial answers, Orion is built to walk users through step-by-step reasoning across budgeting, savings, debt strategy, investment planning, and long-term wealth building.
 
-**Backend**
-- Express 5 (TypeScript)
-- PostgreSQL + Drizzle ORM
-- Alpha Vantage API — live equity quotes
-- Finnhub API — supplemental market data
-- FRED API — macro economic series (Fed Funds Rate, CPI, GDP, etc.)
+## Core Features
 
----
+- **Orion Chat**  
+  Ask financial questions and receive structured, step-by-step reasoning.
 
-## Access
+- **Money Map**  
+  Visualize current savings, future projections, and improvement opportunities.
 
-This app is in **private beta**.
+- **Savings Planner**  
+  Model goals such as emergency funds, down payments, or long-term reserves.
 
-Use access code **`ORION-2025`** at the gate screen to enter.
+- **Strategy Engine**  
+  Explore portfolio allocations and financial game plans based on risk tolerance.
 
----
+- **Framework Library**  
+  Learn from timeless investment philosophies inspired by leading financial thinkers.
 
-## Live Demo
+- **Market Data Dashboard**  
+  Track securities, macro indicators, and watchlist movement.
 
-A static interactive demo is available on GitHub Pages — no backend required:
+- **Explainable Financial Logic**  
+  Prometheus is being built so users can understand *why* a recommendation exists, not just see an answer.
 
-**[rasheekfutrell.github.io/Prometheus-Showcase](https://rasheekfutrell.github.io/Prometheus-Showcase/)**
+- **Future Personalization & Memory**  
+  Orion is evolving toward user-specific context memory to make long-term guidance more adaptive and relevant.
 
-The demo includes full Orion chat logic, all 10 investor frameworks, market data snapshots, savings calculator, and strategy allocator — all running client-side.
+## Why This Matters
 
----
+Financial confusion holds too many people back.
 
-## Full Application
+Prometheus is being built to close the gap between information and understanding — to give people a system that helps them make smarter decisions, strengthen discipline, and build real financial confidence.
 
-The live full-stack app (with real API data) is deployed at:
+This is bigger than budgeting. The mission is to build a platform that helps people move from survival thinking to strategic thinking.
 
-**[workspace-rasheekf.replit.app](https://workspace-rasheekf.replit.app)**
+## Current Status
 
----
+Prometheus AI is currently in **beta development**.
 
-## Orion Engine — How It Works
+The current showcase demonstrates:
+- product vision
+- interface direction
+- Orion user experience
+- financial planning modules
+- investment framework concepts
 
-Orion is not a wrapper around a large language model. It is a structured financial reasoning system built on:
+Future versions will expand personalization, live integrations, explainable decision support, and user-specific financial memory.
 
-- **Formula Engine** — executes exact financial math (DTI, FIRE number, compound growth, etc.)
-- **Situation Detector** — identifies the user's financial scenario from natural language input
-- **Finance Knowledge Base** — maps scenarios to verified financial principles
-- **Memory OS** — maintains context across a session
-- **Corporate Finance Engine** — handles advanced multi-variable calculations
+## Tech Stack
 
-Every response shows the math. Every number is derived from the user's actual inputs.
+- **Frontend:** React, TypeScript, Vite, Tailwind CSS
+- **Backend:** Express (TypeScript)
+- **Database:** PostgreSQL
+- **ORM:** Drizzle
+- **Deployment / Prototyping:** Replit, GitHub Pages
+- **AI Direction:** Orion financial reasoning engine
 
----
+## Roadmap
 
-## Investor Framework Library
-
-| Framework | Category | Horizon |
-|---|---|---|
-| Benjamin Graham | Value | 5–10+ years |
-| Warren Buffett | Value | 10–30+ years |
-| Ray Dalio / All Weather | Macro | All-weather long-term |
-| Peter Lynch | Growth | 3–10 years |
-| John Bogle / Indexing | Passive | 20–40+ years |
-| Charlie Munger | Value | 10+ years |
-| Momentum Strategy | Technical | 3–12 months |
-| Dividend Growth | Income | 10–30+ years |
-| Factor Investing | Quantitative | 10+ years |
-| Contrarian Investing | Value | 1–5 years |
+- [x] Build early Prometheus showcase
+- [x] Define Orion identity and product direction
+- [x] Launch beta-style interface demo
+- [ ] Add real authentication flow
+- [ ] Add admin email automation
+- [ ] Add onboarding for beta testers
+- [ ] Add live market APIs
+- [ ] Expand Orion decision engine
+- [ ] Build personalized financial memory system
+- [ ] Launch production beta
 
----
+## Founder
+
+Prometheus AI is being built by **Rasheek Futrell** as part of a broader vision to combine finance, artificial intelligence, and practical human-centered design into a system that helps people build wealth more intelligently.
+
+## The Mission
+
+Prometheus is not just another finance app.
+
+It is the beginning of a larger vision: building a trusted AI-powered financial intelligence system for the future.
 
-## Project Structure
+**Prometheus provides the platform. Orion provides the intelligence.**
 
EOF
)
