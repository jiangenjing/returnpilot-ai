# ReturnPilot — 完整商业计划书 / Full Business Plan

**项目名 / Project：ReturnPilot — The Autonomous Returns Operating System（自主退货操作系统）**
**副标题 / Subtitle：AI-Powered Returns Decision & Embedded Insurance Technology for Saudi Smart Retail（面向沙特智慧零售的 AI 退货决策与嵌入式保险科技）**
赛道 / Track：KFUPM × Tsinghua Future Ventures Challenge · Track 1 FinTech & Logistics（金融科技与物流）
作者 / By：蒋恩晶（Enjing Jiang）及 KFUPM × 清华团队 · October 2026（2026 年 10 月）

---

## 模块 ① 一句话点题 / Module ① One-line Positioning：名称 + 沙特具体痛点

**一句话 / In one sentence**：ReturnPilot 是一个**决策层 SaaS**（不建仓库、不买车、不做地址解析），为在沙特本地销售的品牌商家与本地物流商，用 AI 自动决定"每一笔退货该上门取件、送自提点还是本地仓处置、运费由谁承担、要不要嵌入退运险"，把沙特本地退货从"流程上能退、经济上不如不退"变成可管理、可保险、成本最优的流程。

*ReturnPilot is a **decision-layer SaaS** (no warehouses, no vehicles, no address parsing). For brands and local 3PLs selling in Saudi Arabia, AI decides for every **local** return — doorstep pickup vs. drop-off vs. locker vs. local-warehouse disposition, who bears the freight, and whether to embed return-shipping insurance — turning a local return from "technically possible but economically not worth it" into a managed, insured, cost-optimized flow.*

**不是宽泛的"物流效率低"，而是现实流程中三个真实、可定位的决策断点 / Not a vague "low logistics efficiency," but three concrete, locatable decision breakpoints in the real process：**

1. **退货资格 / 责任判断靠人工 / Return eligibility & liability are judged manually**：消费者申请退货后，客服要逐条核对"质量问题（卖家担运费）还是不想要（买家担运费）"，规则散落在电商法、平台规则与店铺政策里，判断慢且标准不一。
   *After a return request, agents manually check "defect (seller pays) vs. change of mind (buyer pays)" against rules scattered across e-commerce law, platform policy and store policy — slow and inconsistent.*
2. **取件方式 / 流向默认"一律上门"，不做成本对比 / Pickup defaults to "doorstep for all," with no cost comparison**：沙特网点稀疏（SPL 全国约 580 网点、62 自提柜），自寄常要跨区跑；一律上门则单次成本高。系统不会按商品、原因、位置比较"上门 / 自提点 / 本地仓"哪个更省。
   *Saudi pickup points are sparse (SPL ~580 branches, 62 lockers nationwide); self-return often means crossing districts, while doorstep-for-all is costly. The system never compares doorstep / drop-off / local warehouse by item, reason and location.*
3. **没有退运险对冲，运费风险全压卖家 / No return-shipping insurance — freight risk sits entirely on the seller**：中国消费者下单时可买"退货运费险"，退货由保险赔运费；沙特消费者侧退运险 ≈ 0。团队实测——noon 买的锅电路短路、商家同意换货，但"退货寄回的物流成本和重新买一个锅几乎一样"，又无运费险，最终放弃。
   *In China, buyers add "return-shipping insurance" at checkout and the insurer covers return freight; in Saudi, consumer-side return insurance ≈ 0. Field test: a short-circuited pot bought on Noon — the seller approved exchange, but "shipping it back costs about as much as buying a new pot," with no insurance, so it was abandoned.*

**一手证据 / First-hand evidence（团队实测 / 访谈）**：
- noon 买锅短路换货：退货物流成本 ≈ 重新买一个锅（网点散、无运费险）。
  *Noon pot short-circuit: return shipping ≈ the price of a new pot (sparse network, no return insurance).*
- 朋友在 noon 买传统服饰 Abaya，等 7–10 天才送达（商家 / 物流衔接断点）。
  *A friend's Abaya on Noon took 7–10 days to arrive (merchant–logistics handoff break).*

---

## 模块 ② 沙特现状 vs 中国现状 / Module ② Saudi vs. China：表格化对比 + 可查证数据

### 2.1 市场与基础设施 / Market & Infrastructure

| 维度 / Dimension | 中国现状 / China (mature) | 沙特现状 / Saudi (early stage) |
|---|---|---|
| 电商规模 / E-commerce size | 全球最大、高度成熟 / World's largest, highly mature | 2025 ≈ **USD 27.96B** → 2031 ≈ **USD 54.87B**（Mordor Intelligence） |
| 电商物流 / E-commerce logistics | 单票成本全球最低，中通 ≈ **RMB 0.90/票** / Lowest unit cost (ZTO ~RMB 0.90) | ≈ **USD 2.24B**, CAGR ≈ **10.94%**（Expert Market Research） |
| 退货率 / Return rate | 全球平均 20–30% / Global avg. 20–30% | MENA 网购退货率最高 **30%** / MENA online return rate up to **30%**（Dubai Chamber via Salasa） |
| 年退货成本 / Annual returns cost | 已被保险 + AI 消化 / Largely absorbed by insurance + AI | MENA ≈ **USD 4B/年** / MENA ~**USD 4B/yr**（Dubai Chamber） |
| 退运险 / Return-shipping insurance | 2010 首创；众安 2024 退运险单家 **RMB 8.74B** / Created 2010; ZhongAn 2024 return-insurance **RMB 8.74B** | 消费者退运险 **≈ 0**，仅运输丢损基础险（如 SIDEUP ≈100 SAR/件）/ Consumer return insurance **≈ 0**, only basic loss cover (e.g. SIDEUP ~100 SAR) |
| 末端退货网点 / Last-mile return points | 菜鸟寄取件站点 **>170,000** / Cainiao pickup stations **>170,000** | SPL ≈ **580 网点 + 62 柜**，退货常需跨区 / SPL ~**580 branches + 62 lockers**, often cross-district |
| 退货决策 / Returns decision | AI 决策、上门最快 1 小时、标准验货 / AI-driven, doorstep in ~1 hr, standardized inspection | 人工核对、单一渠道、靠经验 / Manual, single channel, rule of thumb |

### 2.2 头部玩家 / Leading Players

| 角色 / Role | 中国 / China | 沙特 / Saudi |
|---|---|---|
| 电商平台 / Platforms | Taobao/Tmall, JD, Pinduoduo, Douyin | Noon, Amazon.sa, local Salla / Zid merchants |
| 快递 / 3PL | SF Express, JD Logistics, Cainiao, ZTO, YTO | SPL (Saudi Post), SMSA, Aramex, Salasa, J&T, iMile |
| 退运险 / 保险科技 / Return insurance & insurtech | 众安 ZhongAn, 华泰 Huatai (founder), 蚂蚁保 Ant Insurance | 几乎空白 / near-blank; traditional Takaful (e.g. Tawuniya), no embedded return insurance |
| 逆向物流 SaaS / Reverse-logistics SaaS | JD Logistics reverse, Cainiao reverse, RMA systems | Yamm (returns automation), Firaasa (fraud score), Salasa (in-house reverse) |

### 2.3 政策 / Policy

| 政策 / Policy | 中国 / China | 沙特 / Saudi |
|---|---|---|
| 无理由退货 / Free returns | 7 天无理由成熟 / Mature 7-day free returns | 电商法第 13 条 7 天；**2026 新规延至 14–15 天、运费卖家承担** / E-commerce Law Art.13 (7 days); **2026 rule extends to 14–15 days, seller pays freight**（细则以商务部为准） |
| 地址标准 / Address standard | 地址体系完善 / Mature | **国家地址令：2026.1 起每票含 8 位编码**——路由有底座，但"AI 地址解析"切口被关闭 / **National Address mandate: from Jan 2026 every shipment carries an 8-digit code** — enables routing, closes the "address parsing" niche |
| 数据合规 / Data | 个保法 / PIPL | **PDPL + 数据本地化**（SDAIA）/ **PDPL + data localization** (SDAIA) |
| 保险监管 / Insurance | 金融监管总局 / NFRA | **SAMA / 保险监管局**：须持牌承保，技术方可走沙盒 / **SAMA**: licensed underwriting only; tech providers may use the sandbox |
| 支付 / Payments | Alipay / WeChat Pay | mada, STC Pay, Apple Pay；电子支付 ≈ **85%**（SAMA），仍有 COD / e-payments ~**85%**, COD remains |

> 来源链接见 `SOURCES.md` / For links, see `SOURCES.md`.

---

## 模块 ③ 提升空间 / Module ③ Uplift：从沙特现状到"中国式成熟"（尽量量化）

### 3.1 时光机定位 / Time-machine Positioning（团队核心叙事）

| 指标 / Metric | 中国（2020s 成熟）/ China (2020s) | 沙特现状（≈中国 2010s 早期）/ Saudi now (~early-2010s China) | ReturnPilot 落地后（≈中国 2018–2020）/ After ReturnPilot (~2018–2020 China) |
|---|---|---|---|
| 退运险 / Return insurance | 2010 华泰首创；2024 众安 RMB 8.74B / Huatai 2010; ZhongAn RMB 8.74B (2024) | ≈ 0 | 嵌入式退运险上线，投保率目标 50–90% / Embedded return insurance, target take-up 50–90% |
| 末端网点 / Last-mile points | Cainiao >170,000 | SPL 580 + 62 lockers | 不重建网络，用现有网点 + AI 路由提利用率 / No rebuild; AI routing lifts utilization of existing points |
| 单笔处理 / Per-return handling | AI 决策、上门 1 小时 / AI, doorstep in 1 hr | 人工、单一渠道、靠经验 / Manual, single channel | AI 自动决策 + 合单取件 / AI decision + merged pickup |
| 成本结构 / Cost structure | 保险 + AI 消化 / Insurance + AI | 卖家独自承担、无险 / Seller alone, uninsured | 保险对冲 + 路由降本 / Insurance hedge + routing savings |

### 3.2 单商家基准盘 / Single-merchant Base Case（月 1,000 笔退货 / 1,000 returns/month；SAR）

- 现状基线 / Baseline：80% 上门（35 SAR）+ 20% 网点（15 SAR）= 加权 **31 SAR/单** / weighted **31 SAR/return**.
- 每把 1 单从上门转替代渠道，毛节约 = 35 − 15 − 3（协调）= **17 SAR**（约占上门成本 49%）/ Gross saving per shifted return = 35 − 15 − 3 coordination = **17 SAR** (~49% of doorstep cost).

| 指标 / Metric | 悲观 / Pessimistic | 中性 / Base | 乐观 / Optimistic |
|---|---|---|---|
| 转移比例 / Shift ratio | 10% | 30% | 50% |
| 转移单数（/月）/ Returns shifted | 100 | 300 | 500 |
| 上门占比终值 / Final doorstep share | 70% | 50% | 30% |
| 物流毛节约 / Gross logistics saving (SAR/mo) | 1,700 | 5,100 | 8,500 |
| 可兑现人力节约（0%/40%/70%）/ Realized labor saving | 0 | 600 | 1,750 |
| 新增返工 / 复核 / Added rework cost | −450 | −240 | −90 |
| ReturnPilot 平台服务费（含按单）/ Platform fee | −1,200 | −1,600 | −2,062 |
| **商家经常性月净收益 / Merchant monthly net (SAR)** | **+50** | **+3,860** | **+8,098** |
| **年化净收益（×12）/ Annualized net (SAR)** | 600 | 46,320 | 97,176 |
| 一次性接入 / One-time integration (SAR) | 12,000 | 12,000 | 12,000 |
| **静态回收期 / Payback period** | ≈240 月（基本无法回本 / ~no payback） | **3.1 月 / months** | **1.5 月 / months** |

- 中性首年净（已扣接入）= 46,320 − 12,000 = **34,320 SAR**；首年 ROI = 34,320 / 12,000 ≈ **286%**。
  *Base-case year-1 net (after integration) = **34,320 SAR**; year-1 ROI ≈ **286%**.*
- 【口径说明 / Caliber】结构比例参考中国公开数据；成本水平（上门 35、网点 15、人力 30 SAR/小时）采用沙特本地口径。转移比例为试点假设、需访谈验证，非沙特行业均值。
  *Structural ratios reference public China data; cost levels (doorstep 35, drop-off 15, labor 30 SAR/hr) use Saudi figures. Shift ratios are pilot assumptions to be validated, not Saudi averages.*

### 3.3 保险机构侧 / Insurer Side（退运险第二曲线 / 2nd curve，月 1,000 单）

| 指标 / Metric | 悲观 / Pess. | 中性 / Base | 乐观 / Opt. |
|---|---|---|---|
| 投保率 / Take-up rate | 50% | 70% | 90% |
| 平均保费 / Avg. premium (SAR) | 2.5 | 2.5 | 2.5 |
| 月保费规模 / Monthly premiums (SAR) | 1,250 | 1,750 | 2,250 |
| ReturnPilot 分润比例 / Our share | 15% | 18% | 20% |
| **ReturnPilot 月技术费 / Monthly tech fee (SAR)** | **187.5** | **315** | **450** |

### 3.4 市场总量空间 / Total Addressable Space（已查证 + 估算）

- 【已查证 / Verified】沙特电商 2025→2031 ≈ USD 27.96B→54.87B；MENA 退货年成本 ≈ USD 4B。
- 【估算 / Estimated】若退运险渗透率 5 年内从 ≈0 升至 30–50%，退运险技术服务对应沙特市场可达数亿里亚尔 / 年量级（需以实际退货率与保费校准）/ If return-insurance penetration rises from ~0 to 30–50% within 5 years, the Saudi tech-service market could reach several hundred million SAR/yr (to be calibrated).
- 【已查证 / Verified】50% 区域消费者称退货 / 退款便利影响复购；29% 沙特消费者因缺免运费 / 灵活退货不满 / 50% say returns ease drives repurchase; 29% are dissatisfied by lack of free/flexible returns.

---

## 模块 ④ 商业模式 / Module ④ Business Model：客户、付费方、盈利逻辑、两地差异

### 4.1 三层产品与计费 / Three Product Layers & Pricing

| 层级 / Layer | 产品 / Product | 核心功能 / Core function | 谁付费 / Pays | 盈利模式 / Revenue |
|---|---|---|---|---|
| 主产品 / Main | **AI 退换货决策 SaaS / AI Returns Decision SaaS** | 判断责任、是否需实物退回、选择上门 / 柜 / 本地仓最优路径 / Liability, physical-return need, optimal routing | 在沙品牌商家、3PL / Brands, 3PL | **SaaS 年费 ≈18,000 SAR/年 + 按单费 1–3 SAR/单 / Annual fee ~18,000 SAR + 1–3 SAR/order** |
| 第二曲线 / 2nd curve | **嵌入式退运险科技 / Embedded Return-insurance Tech** | 数据对接、概率定价、反欺诈、理赔技术 / Data, probability pricing, anti-fraud, claims tech | SAMA 持牌 Takaful 及合作企业 / Licensed Takaful insurers | **技术服务费 + 保单分润 15–20%（不承保）/ Tech fee + 15–20% policy share (no underwriting)** |
| 增值 / Value-add | Return Intelligence | 退货原因、残值、成本归因、复购分析 / Reasons, residual value, cost attribution, repurchase | 品牌商、物流 / Brands, 3PL | 高级订阅 / Premium subscription |
| 可选 / Optional | 成本节约分成 / Cost-saving share | 核验的逆向物流节约 / Verified reverse-logistics savings | 3PL | 节约额提成 / Share of savings |

### 4.2 目标客户与使用者 / Target Customers & Users

- **消费者端（C，免费）/ Consumer (C, free)**：沙特本地网购消费者（含约 44% 外籍居民），是数据与流量入口 / Saudi online shoppers (~44% expatriates); the data & traffic entry point.
- **商家端（B，付费主收入）/ Merchant (B, main revenue)**：Noon / Amazon.sa / Salla / Zid 上的品牌商家，在沙中国品牌（小米、石头、海尔等渠道），3PL（SPL、Salasa、SMSA、J&T、iMile）/ Brands on Noon/Amazon.sa/Salla/Zid, Chinese brands in KSA (Xiaomi, Roborock, Haier), and 3PLs.
- **保险机构端（B，付费第二曲线）/ Insurer (B, 2nd curve)**：沙特持牌 Takaful / 险企——ReturnPilot 做其"定价与反欺诈引擎"，切入精算与风控段，不碰牌照、不承保 / Licensed Takaful insurers — we are their "pricing & anti-fraud engine," capturing the actuarial/risk segment without a license or underwriting.

### 4.3 沙特落地 vs 中国落地 / Saudi vs. China Rollout

| 维度 / Dimension | 沙特 / Saudi | 中国 / China (home market / tech source) |
|---|---|---|
| 实体与数据 / Entity & data | 需本地实体、**PDPL 数据本地化** / Local entity, **PDPL localization** | 合规成熟 / Mature compliance |
| 物流网络 / Logistics | 与 SPL / Salasa / SMSA **API 集成**，不自建 / **API integration**, no build | 网络密集 / Dense network |
| 退运险 / Return insurance | 须 **SAMA 持牌承保**，建议与本地 Takaful 合资、走沙盒 / **SAMA-licensed** underwriting; JV with local Takaful, use sandbox | 众安 / 华泰为算法母本 / ZhongAn/Huatai as algorithm template |
| 支付 / Payments | mada / STC Pay / Apple Pay；保留 COD 但电子代扣 + 风控 / Licensed rails; keep COD with e-debit + risk control | Alipay / WeChat 预付费 / Prepaid dominant |
| 获客 / GTM | 先单商家 / 单城试点，借 KFUPM 与 PIF / 物流生态 / Single merchant/city pilot via KFUPM & PIF/logistics ecosystem | 与京东 / 菜鸟逆向、众安合作出海 / Partner with JD/Cainiao reverse, ZhongAn |
| 政策 / Policy | 2026 退货新规点燃需求；国家地址令提供底座 / 2026 rule ignites demand; National Address enables routing | — |

### 4.4 落地路径 / Roadmap（里程碑）

- **0–3 月 / months**：单商家 / 单城 MVP，约 1,000 笔退货，量化成本与成功率；阿语优先 + 多语言 / Single merchant/city MVP, ~1,000 returns, quantify cost & success; Arabic-first, multilingual.
- **3–6 月 / months**：接入 SPL / Salasa API，与一家持牌 Takaful 进 SAMA 沙盒 / Integrate SPL/Salasa; SAMA sandbox with one licensed Takaful.
- **6–12 月 / months**：复制到 10–50 商家，跑通双收费 / Replicate to 10–50 merchants; dual revenue live.
- **12 月后 / beyond**：利雅得 / 吉达 / 达曼全覆盖，向其他 GCC 复制 / Riyadh/Jeddah/Dammam; expand to other GCC states.

---

## 模块 ⑤ 理由双证 / Module ⑤ Dual Evidence：中国为何成熟 + 沙特为何缺失但有条件

### 5.1 中国为何已成熟 / Why China Is Mature

1. **退运险完整跑通 / Return insurance fully proven**：2010 华泰首创；众安退运险 2023 收入 64.68 亿、**2024 年 87.4 亿元**——证明"下单投保、退货兑现"成立且规模巨大 / Huatai created it in 2010; ZhongAn return-insurance RMB 6.468B (2023), **RMB 8.74B (2024)** — proving "buy at checkout, claim on return" at scale.
2. **逆向物流与决策成熟 / Reverse logistics & decisions mature**：京东上门取件 / 换新 / 逆向一体化，联合险企把运费险单价降约 10%，靠"合单取件"双赢；菜鸟站点 >17 万，支持拥挤度查询、错峰、夜间揽收、主动赔付 / JD doorstep pickup/exchange/reverse integration cut premium ~10% via merged pickup; Cainiao >170k stations with crowding query, off-peak, night pickup, proactive refund.
3. **成本与算法底座成熟 / Cost & algorithm base mature**：中通 ≈0.90 元 / 票全球最低；退货概率、图反欺诈、VRP 均有成熟工程实践 / ZTO ~RMB 0.90, world's lowest; return-probability, graph anti-fraud and VRP are engineering-proven.

### 5.2 沙特为何缺失、但有落地条件 / Why Saudi Lags Yet Is Ready

1. **需求被政策点燃 / Demand ignited by policy**：2026 新规无理由退货 14–15 天、卖家担运费——客单 ≈200 SAR 的退货吃约 60 SAR，退货率超 5% 利润归零，商家强付费动机 / 2026 rule: 14–15 day free returns, seller pays — a ~200 SAR order's return costs ~60 SAR; above 5% returns, profit vanishes — strong willingness to pay.
2. **基础设施刚好就位 / Infrastructure just ready**：国家地址令提供路由底座；电子支付 ≈85%、mada / Nafath 身份就绪；SPL / Salasa 已有逆向物流，无需重建重资产 / National Address enables routing; e-payments ~85%, mada/Nafath identity ready; SPL/Salasa already provide reverse logistics — no heavy rebuild.
3. **竞争空白明确 / Clear white space**：消费者退运险 ≈ 0；Yamm 做流程自动化、Firaasa 有反欺诈评分，但**没有一家把退货概率直接变成保费定价并嵌入决策 SaaS**——ReturnPilot 是补位 / Consumer return insurance ≈ 0; Yamm automates flow, Firaasa has fraud scores, but **none turns return probability directly into premium pricing inside a decision SaaS** — we complement.
4. **本土自我背书 / Local endorsement**：沙特物流商 Salasa 明确"目标不是减少退货，而是有效管理退货"（إدارتها بفعالية），与我们一致 / Saudi 3PL Salasa states "the goal is not to reduce returns, but to manage them effectively" — exactly our positioning.
5. **人口结构 / Demographics**：总人口 ≈3,530 万、年轻、智能手机渗透高；外籍居民 ≈44%（印 / 巴 / 孟 / 菲 / 埃及），多语言退货是刚需 / ~35.3M, young, high smartphone penetration; ~44% expatriates — multilingual returns are essential.

---

## 附：三端数据闭环飞轮 / Appendix: The Three-sided Data Flywheel

1. **消费者端 / Consumer** 免费、低门槛，沉淀"退货原因、商品状态、偏好、位置"数据 / Free, low-friction; captures reason, item condition, preference, location.
2. 数据喂给**商家端 AI 决策引擎 / feeds the merchant AI engine**，路由更准、降本更多 → 商家付费、体验改善 → 复购上升、订单更多 / Better routing & savings → merchants pay, experience improves → more repurchase & orders.
3. 同时喂给**保险机构端定价 / 反欺诈 / feeds insurer pricing & anti-fraud**，保费更准、骗保下降 → 险企降保费、扩承保 → 投保更多 / More accurate premiums, less fraud → lower prices, wider cover → more policies.
4. 投保与交易扩大又带来更多数据 → **数据越多 → 决策越准、保费越优 → 客户越多 → 数据更多**，自我强化；壁垒是跨三端、可持续积累的退货专有数据 / More policies & transactions → more data: **more data → better decisions & premiums → more customers → more data**; the moat is proprietary, cross-side returns data.

---

## 关键风险与应对 / Key Risks & Mitigation

| 风险 / Risk | 应对 / Mitigation |
|---|---|
| 拿不到物流商真实数据 / No access to real 3PL data | 单商家试点 + 数据授权换降本分成；中国模型 + 小样本迁移 / Pilot + data-for-savings; China model + small-sample transfer |
| 退运险牌照 / Insurance license barrier | 不承保，做持牌 Takaful 的技术方，走 SAMA 沙盒 / No underwriting; be the licensed Takaful's tech provider via SAMA sandbox |
| 不信任、不改用替代渠道 / Distrust, no channel shift | 官方 / 平台背书、阿语优先、保留上门选择权 / Official/platform endorsement, Arabic-first, keep doorstep option |
| COD 与现金习惯 / COD & cash habits | 不消灭 COD，电子代扣 + 风控，退款走持牌渠道 / Keep COD with e-debit + risk control; licensed refunds |
| 付费意愿未验证 / Willingness to pay unverified | 先做 ROI 清晰的单站基准盘，用可核验节约说话 / Start with a clear-ROI single-site case using verified savings |

*全部来源见 `SOURCES.md`；评分逐项对照见 `SCORING.md`。/ For sources see `SOURCES.md`; for judging-criteria mapping see `SCORING.md`.*
