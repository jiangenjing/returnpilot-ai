# ReturnPilot — The Autonomous Returns Operating System
# ReturnPilot —— 自主退货操作系统

### AI-Powered Returns Decision & Embedded Insurance Technology for Saudi Smart Retail
### 面向沙特智慧零售的 AI 退货决策与嵌入式保险科技

> KFUPM × Tsinghua Future Ventures Challenge · Track 1: FinTech & Logistics
> KFUPM × 清华 Future Ventures Challenge · 赛道 1：金融科技与物流
> Team / 团队：KFUPM (2) + Tsinghua SIGS (2)

---

## What it is / 产品是什么

ReturnPilot is a **decision-layer SaaS** (we do **not** build warehouses, buy vehicles, or do address parsing). For brands and 3PLs selling in Saudi Arabia, AI decides for every **local** return:

*ReturnPilot 是一个**决策层 SaaS**（我们**不**建仓库、不买车、不做地址解析）。面向在沙特销售的品牌与第三方物流商（3PL），由 AI 对每一笔**沙特本地**退货自动决策：*

- **Pickup method & routing** — doorstep pickup / drop-off point / locker / local-warehouse disposition
  **取件方式与路由** —— 上门取件 / 自提点 / 自提柜 / 本地仓处置
- **Who pays the freight** — customer fault vs. seller fault, under the 2026 return regulation
  **运费由谁承担** —— 依据 2026 年退货新规，区分买家责任与卖家责任
- **Whether to embed return-shipping insurance** — underwritten by a SAMA-licensed insurer; we provide pricing & anti-fraud technology
  **是否嵌入退运险** —— 由 SAMA 持牌保险机构承保，我们提供定价与反欺诈技术

Goal: move a Saudi local return from "the return shipping costs as much as the product" toward a managed, insured, cost-optimized flow.

*目标：把沙特本地退货从"退货运费和商品本身一样贵"，转变为可管理、可保险、成本最优的流程。*

## The three sides / 三端

| Side / 端 | Who pays / 谁付费 | Core modules / 核心模块 |
|---|---|---|
| Consumer / 消费者端 (C) | Free / 免费 | Multilingual returns agent · smart method recommendation · return-protection policy · refund-before-return · tracking / 多语言退货 Agent · 智能方式推荐 · 退货无忧保单 · 先退款后退货 · 全程追踪 |
| Merchant / 商家端 (B) | **Pays (main revenue) / 付费（主收入）** | AI decision engine · returns cost dashboard · insurance config · high-risk alerts · merged-pickup routing / AI 决策引擎 · 退货成本看板 · 退运险配置 · 高风险预警 · 合单取件路由 |
| Insurer / 保险机构端 (B) | **Pays (2nd curve) / 付费（第二曲线）** | Return-probability pricing · tiered premium matrix · anti-fraud underwriting · claims risk control · dashboard / 退货概率定价 · 阶梯保费矩阵 · 反欺诈核保 · 理赔风控 · 承保看板 |

## Repository layout / 目录结构

```
returnpilot-ai/
├── README.md                     # 本文件 / this file
├── site/                         # 静态可托管产品演示（打开 site/index.html）/ static hostable demo
│   ├── index.html
│   └── assets/
└── docs/
    ├── BUSINESS_PLAN.md          # 完整 BP（中英对照）/ full business plan
    ├── SCORING.md                # 5 项评审标准对照 / mapping to 5 judging criteria
    └── SOURCES.md                # 数据来源与引用 / data sources & citations
```

## Run it / 如何运行

The product is a **pure static site** (no backend, no build step). Open `site/index.html`, or host the `site/` folder on any static host.

*本产品为**纯静态站点**（无后端、无构建步骤）。用浏览器打开 `site/index.html`，或将 `site/` 目录托管到任意静态主机。*

## Live interactive demo / 在线交互演示

- **Hosted interactive product / 在线交互产品**：[https://4m35pz21sueq0.doubaoapps.com/app/app_17ft5urc7pr](https://4m35pz21sueq0.doubaoapps.com/app/app_17ft5urc7pr)
  Includes the three-sided apps (consumer / merchant / insurer), the auto-play 8-scene guided storyline, AI return routing & return-insurance pricing, plus the "For the Judges" BP sub-page and the "Scoring" sub-page.
  含三端应用（消费者 / 商家 / 保险机构）、可自动播放的 8 幕剧情主线、AI 退货路由与退运险定价，以及「For the Judges」BP 子页面和「Scoring 评分对照」子页面。
- The static `site/` folder in this repo is an offline snapshot of the same product — just open `site/index.html`.
  本仓库 `site/` 目录为同一产品的离线静态快照，打开 `site/index.html` 即可。

## Business model (summary) / 商业模式（摘要）

- **Main product — AI Returns Decision SaaS**: annual subscription + per-order fee, paid by merchants & 3PLs.
  **主产品——AI 退货决策 SaaS**：年费 + 按单费，由商家与 3PL 付费。
- **Second curve — embedded return-insurance technology**: we do NOT underwrite; a SAMA-licensed Takaful insurer does. We provide the return-probability pricing & anti-fraud engine for a technology fee / policy share (15–20%).
  **第二曲线——嵌入式退运险科技**：我们不承保，由 SAMA 持牌 Takaful 保险机构承保；我们提供退货概率定价与反欺诈引擎，收取技术服务费 / 保单分润（15–20%）。
- **Optional — verified cost-saving share** with logistics partners.
  **可选——与物流伙伴按核验的成本节约额分成。**

## Engineering ↔ Business split / 工程 ↔ 商科分工

- **Engineering students / 工程学生**: feasibility & system design (XGBoost/GNN return-probability & fraud models, LLM multilingual agent, rules engine, VRP routing, API integration).
  可行性与系统设计（XGBoost/GNN 退货概率与反欺诈模型、LLM 多语言 Agent、规则引擎、VRP 路由、API 集成）。
- **Business students / 商科学生**: market validation, pricing, go-to-market and regulatory navigation (PDPL, SAMA insurance sandbox, National Address mandate).
  市场验证、定价、落地推广与监管合规（PDPL、SAMA 保险沙盒、国家地址令）。

*Prepared by Enjing Jiang (蒋恩晶) and the KFUPM × Tsinghua team, October 2026.*
*由蒋恩晶（蒋恩晶）及 KFUPM × 清华团队撰写，2026 年 10 月。*
