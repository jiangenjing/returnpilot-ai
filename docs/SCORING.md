# ReturnPilot — 5 项评审标准对照 / Scoring Sheet

> 5 项评审标准权重均等、全部必须满足；本文件逐项说明 ReturnPilot 如何回应。
> The five judging criteria are equally weighted and all must be met; this file maps ReturnPilot to each.
> 可交互版见产品 Demo 的「Scoring / 评分对照」子页面。/ Interactive version: the Demo's "Scoring" sub-page.

---

## 总览 / Overview

| # | 评分维度 / Criterion | ReturnPilot 的核心答案 / Core Answer |
|---|---|---|
| 1 | 具体问题，非宽泛主题 / Specific problem, not a broad topic | 锁定本地退货"如何决策、运费谁担、无险对冲"的具体断点 / The concrete breakpoints of decision, freight liability and missing insurance in local returns |
| 2 | 技术可行性 / Technical feasibility | 全为成熟技术（XGBoost/GNN/LLM/规则引擎/VRP），API 集成，3 月出 MVP / All mature tech, API integration, MVP in 3 months |
| 3 | 两国商业落地 / Commercial viability in both markets | 沙特商家/3PL/险企付费，2.6 月回本；中国品牌与技术出海，监管清晰 / Saudi B-side pays, 2.6-month payback; Chinese brands & tech go global; clear regulation |
| 4 | 对双方价值 / Value to both sides | 沙特降本 + 补齐退运险基础设施；中国品牌降售后成本 + 技术出海 / Saudi: savings + missing insurance infrastructure; China: lower after-sales cost + tech export |
| 5 | 跨文化消费行为 / Cross-cultural behavior | 针对支付、信任、语言、宗教性别、售后习惯做具体设计 / Specific design for payment, trust, language, religion/gender, after-sales habits |

---

## 维度 1 · 具体问题，非宽泛主题 / Criterion 1 · Specific Problem

**表态 / Stance**：不做"物流效率低"这类宽泛主题，锁定可定位的现实流程问题。/ Not a vague "low efficiency," but a locatable process problem.

**问题陈述 / Problem**：本地退货中，"上门 / 自提 / 本地仓、运费谁担、要不要险"靠人工经验且无险对冲——"流程上能退、经济上不如不退"。/ In local returns, routing, freight liability and insurance rely on manual judgment with no insurance hedge — "possible but not worth it."

**三个真实断点 / Three real breakpoints**：

| 断点 / Breakpoint | 环节 / Stage | 现状 / Status quo | 后果 / Consequence |
|---|---|---|---|
| 资格 / 责任判断 / Eligibility & liability | 申请售后 / Request | 人工逐条核对 / Manual rule-checking | 慢、标准不一 / Slow, inconsistent |
| 取件 / 流向路由 / Pickup & routing | 安排取件 / Scheduling | 默认一律上门、不对比成本 / Doorstep-for-all, no cost comparison | 跨区跑、成本高 / Cross-district, costly |
| 检测 / 处置 / Inspection & disposition | 退回后 / After return | 单一渠道、靠经验、无险 / Single channel, rule of thumb, uninsured | 卖家独自担风险 / Seller bears all risk |

**一手证据 / First-hand evidence**：
- noon 买锅：退货成本 ≈ 重买一个锅（网点散、无险）/ Noon pot: return cost ≈ a new pot (sparse, uninsured).
- 朋友买 Abaya，7–10 天才到 / Friend's Abaya took 7–10 days.

**问题量级 / Magnitude**：MENA 退货率最高 30%、年成本 ≈ USD 4B；50% 称退货体验影响复购；29% 因缺免运费 / 灵活退货不满。/ MENA return rate up to 30%, ~USD 4B/yr; 50% say returns drive repurchase; 29% dissatisfied.

**关键判断 / Key judgment**：沙特不缺退货服务（SPL/Salasa 已有），缺"决策数字化 + 退运险对冲层"。/ Saudi does not lack returns services (SPL/Salasa); it lacks the decision-digitization + insurance-hedge layer.

---

## 维度 2 · 技术可行性 / Criterion 2 · Technical Feasibility

**结论 / Conclusion**：全部为现有成熟技术，无未验证前沿，短期可落地。/ All mature, proven technology; no unvalidated frontier; near-term deployment.

| 能力 / Capability | 成熟技术 / Mature tech | 为何现在可行 / Why feasible now |
|---|---|---|
| 退货概率预测 / Return-probability | XGBoost / LightGBM | 业界成熟、广泛用于风控 / Proven in risk prediction |
| 反欺诈 / Anti-fraud | GNN / GraphSAGE + Neo4j | 图反欺诈成熟 / Graph anti-fraud proven |
| 多语言 / Multilingual | ASR + LLM | 阿语优先，另支持乌尔都语 / 印地语 / Arabic-first plus Urdu/Hindi |
| 规则与定价 / Rules & pricing | 规则引擎 + 精算公式 / Rules engine + actuarial formula | 责任 / 运费 / 保费自动判断 / Automated liability, freight, premium |
| 路径优化 / Routing | VRP / 整数规划 / Integer programming | 路线、合单、柜格 / Routes, merged pickup, lockers |

**系统集成 / Integration**：本地物流 / 平台普遍开放 API，对接现有 TMS/ERP/平台/保险核心，无需改造底层。/ APIs are common; integrate with existing TMS/ERP/platform/insurance core without re-engineering.

**冷启动 / Cold start**：本地数据少 → 中国模型结构 + 小样本迁移，规则引擎兜底。/ Limited local data → China model structure + small-sample transfer, rules engine as fallback.

**时间表 / Timeline**：0–3 月 MVP（1,000 笔）；3–6 月接 SPL/Salasa 与保险沙盒；6–12 月复制 10–50 商家。/ 0–3 mo MVP (1,000 returns); 3–6 mo SPL/Salasa & insurance sandbox; 6–12 mo replicate to 10–50 merchants.

> 工程学生负责系统设计与可行性。/ Engineering students own system design & feasibility.

---

## 维度 3 · 两国商业落地 / Criterion 3 · Commercial Viability

**目标客户与谁付费 / Customers & payers**：

| 市场 / Market | 付费方 / Pays | 模式 / Model |
|---|---|---|
| 沙特 / Saudi | 品牌商家、3PL（B2B）；险企为第二曲线 / Brands, 3PL; insurers (2nd curve) | 消费者基础服务免费 / Free for consumers |
| 中国 / China | 在沙小米 / 石头 / 海尔等品牌；保险科技 / 逆向团队为合作方 / Brands in KSA; insurtech/reverse teams as partners | 技术与品牌母市场 / Tech & brand home market |

**盈利逻辑 / Revenue**：SaaS 年费（18,000）+ 按单费（主）；保费分润 15–20%（第二曲线）；节约分成。/ Annual fee (18,000) + per-order (main); 15–20% policy share (2nd curve); savings share.

**单位经济（自己侧·单客户/年）/ Unit economics (per client/yr)**：收入 21,780、交付 3,600、毛利 18,180（≈83%）、回收 ≈2.6 月。/ Revenue 21,780; delivery 3,600; gross profit 18,180 (~83%); payback ~2.6 mo.

**三年路径 / Three-year path**：Y1（15 客户）净利 -56.7 万；Y2（60）-20.0 万；Y3（150）+101.4 万。/ Y1 (15) net -567k; Y2 (60) -200k; Y3 (150) +1.014M.

**监管现实 / Regulatory reality**：

| 监管点 / Point | 应对 / Response |
|---|---|
| PDPL 数据本地化 / Localization | 本地云 / Local cloud |
| SAMA 保险 / Insurance | 持牌承保，我们做技术方、走沙盒 / Licensed underwriting; we are tech provider via sandbox |
| 国家地址令 / National Address | 路由底座，不做地址解析 / Routing base; no address parsing |
| 退货新规 / Returns rule | 点燃需求 / Ignites demand |
| 中国出海合规 / China outbound | 与持牌保险科技合作 / Partner with licensed insurtech |

> 商科学生负责市场验证与落地推广。/ Business students own validation & GTM.

---

## 维度 4 · 对双方价值 / Criterion 4 · Value to Both Sides

### 沙特获得 / Saudi gains
- **消费者 / Consumers**：退货 0 运费（险）、取件即极速退款、多渠道、运费有保障 / Zero-freight returns, instant refund on pickup, multiple channels, protected freight.
- **商家 / Merchants**：取件成本降约 13%–20%、对冲新规运费风险、体验改善带动复购 / Pickup cost down ~13–20%, hedge new freight risk, better experience drives repurchase.
- **国家 / Nation**：配合 Vision 2030 数字化，补齐退运险基础设施 / Supports Vision 2030 digitization; fills the return-insurance infrastructure gap.

### 中国获得 / China gains
- **品牌 / Brands**：小米 / 石头 / 海尔降海外售后成本，获可复制出海履约工具 / Lower overseas after-sales cost; a replicable outbound fulfillment tool.
- **技术输出 / Tech export**：AI、保险科技、逆向 SaaS 打开沙特，带动数字服务出口 / AI, insurtech and reverse SaaS enter Saudi; digital-service export.
- **可复制 / Replicability**：沙特验证后复制到其他 GCC / 中东 / Replicate to other GCC/Middle East markets after Saudi.

---

## 维度 5 · 跨文化消费行为 / Criterion 5 · Cross-cultural Behavior

| 维度 / Dimension | 中国 / China | 沙特 / Saudi | 产品动作 / Product action |
|---|---|---|---|
| 支付 / Payment | Alipay/WeChat 预付费 / Prepaid | 仍有 COD、mada/STC Pay / COD remains | 不消灭 COD，电子代扣 + 风控；持牌退款 / Keep COD with e-debit + risk control; licensed refunds |
| 信任 / Trust | 信任平台担保 / Platform guarantee | 信任政府 / 雇主背书 / Gov't/employer endorsement | 官方标识，定位沙盒 ISV / Official labels; sandbox ISV |
| 语言 / Language | 中文 / Chinese | 外籍 ≈44% / ~44% expats | 阿语优先 + 乌尔都 / 印地 / 孟加拉，语音 / Arabic-first + Urdu/Hindi/Bengali, voice |
| 宗教与性别 / Religion & gender | — | 礼拜、斋月、性别隔离 / Prayer, Ramadan, segregation | 礼拜为运力因子、斋月校准、女性偏好、尊重隐私 / Prayer as capacity factor, Ramadan calibration, female preference, privacy |
| 售后决策 / After-sales | 一键退货、下单即投保 / One-click, insure at checkout | 繁琐、无险概念 / Cumbersome, no insurance | 下单投保锁定、退货兑现，一键申请 / Insure at checkout, claim on return; one-click |

---

*工程学生负责可行性与系统设计，商科学生负责市场验证与落地推广，两份可行性分析均完整呈现。/ Engineering students own feasibility & system design; business students own validation & GTM — both analyses are fully included.*
