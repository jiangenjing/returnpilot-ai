# ReturnPilot — The Autonomous Returns Operating System

### AI-Powered Returns Decision & Embedded Insurance Technology for Saudi Smart Retail

> KFUPM × Tsinghua Future Ventures Challenge · Track 1: FinTech & Logistics
> Team: KFUPM (2) + Tsinghua SIGS (2)

---

## What it is

ReturnPilot is a **decision-layer SaaS** (we do **not** build warehouses, buy vehicles, or do address parsing). For brands and 3PLs selling in Saudi Arabia, AI decides for every local return:

- **Pickup method & routing** — doorstep pickup / drop-off point / locker / local-warehouse disposition
- **Who pays the freight** — customer fault vs. seller fault, under the 2026 return regulation
- **Whether to embed return-shipping insurance** — underwritten by a SAMA-licensed insurer; we provide pricing & anti-fraud technology

Goal: move the economics of a Saudi local return from "the return shipping costs as much as the product" toward a managed, insured, cost-optimized flow.

## The three sides

| Side | Who pays | Core modules |
|---|---|---|
| Consumer (C) | Free | Multilingual returns agent · smart method recommendation · return-protection policy · refund-before-return · end-to-end tracking |
| Merchant (B) | **Pays (main revenue)** | AI decision engine · returns cost dashboard · return-insurance config · high-risk alerts · merged-pickup routing |
| Insurer (B) | **Pays (2nd curve)** | Return-probability pricing engine · tiered premium matrix · anti-fraud underwriting · claims risk control · underwriting dashboard |

## Repository layout

```
returnpilot-ai/
├── README.md                     # this file
├── site/                         # static, hostable product demo (open site/index.html)
│   ├── index.html
│   └── assets/
└── docs/
    ├── BUSINESS_PLAN.md          # full BP: problem, comparison, uplift, model, evidence
    ├── SCORING.md                # point-by-point mapping to the 5 judging criteria
    └── SOURCES.md                # data sources & citations
```

## Run it

The product is a **pure static site** (no backend, no build step). Open `site/index.html` in a browser, or host the `site/` folder on any static host.

## Live interactive demo

A hosted version (with the 8-scene guided storyline, BP sub-page and Scoring sub-page) is available on the Miaoda platform — link kept out of this repo for privacy.

## Business model (summary)

- **Main product — AI Returns Decision SaaS**: annual subscription + per-order fee, paid by merchants & 3PLs.
- **Second curve — embedded return-insurance technology**: we do NOT underwrite; a SAMA-licensed Takaful insurer does. We provide the return-probability pricing and anti-fraud engine and take a technology-service fee / policy share (15–20%).
- **Optional — verified cost-saving share** with logistics partners.

## Engineering ↔ Business split

- **Engineering students**: feasibility & system design (XGBoost/GNN return-probability & fraud models, LLM multilingual agent, rules engine, VRP routing, API integration).
- **Business students**: market validation, pricing, go-to-market and regulatory navigation (PDPL, SAMA insurance sandbox, National Address mandate).

*Prepared by Enjing Jiang (蒋恩晶) and the KFUPM × Tsinghua team, October 2026.*
