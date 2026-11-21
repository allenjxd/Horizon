---
layout: default
title: "Horizon Summary: 2026-11-21 (ZH)"
date: 2026-11-21
lang: zh
---

> 从 207 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [陶哲轩文章聚焦纳维－斯托克斯与广义黎曼假设](#item-tech-news-1) ⭐️ 8.0/10
2. [Inkling 2 Mini：循环架构开放权重模型](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI 测试 ChatGPT 商家资料与智能体后台](#item-tech-news-3) ⭐️ 8.0/10
4. [拉加德：Pontes 推进欧洲代币化资产统一结算](#item-tech-news-4) ⭐️ 8.0/10
5. [《悦嫂坊》第二版面向独立月嫂提供六项工具](#item-tech-news-5) ⭐️ 7.0/10
6. [DeepSeek Harness 七小时复刻 Gemini Flow](#item-tech-news-6) ⭐️ 7.0/10
7. [Muse 七个月迭代至超千万次下载](#item-tech-news-7) ⭐️ 7.0/10
8. [MoonPay 申请全国信托银行牌照](#item-tech-news-8) ⭐️ 7.0/10
9. [Fairmint 拟在 Canton 和以太坊试点代币化股票交易](#item-tech-news-9) ⭐️ 7.0/10
10. [Prometheus 测试 12 小时工业设计智能体](#item-tech-news-10) ⭐️ 7.0/10

**科技博客**
1. [链上买入 ANT 后，你究竟持有什么](#item-tech-blog-1) ⭐️ 8.0/10
2. [我如何诱使黑客代理执行代码](#item-tech-blog-2) ⭐️ 8.0/10
3. [黎曼猜想双重证明宣称](#item-tech-blog-3) ⭐️ 6.0/10
4. [形式化验证：AI 编程的质量防线](#item-tech-blog-4) ⭐️ 6.0/10
5. [Anthropic IPO 与本地 AI 工程观察](#item-tech-blog-5) ⭐️ 5.0/10

**AI 创作者雷达**
1. [鸿蒙高校创新赛发布高校应用孵化计划](#item-ai-creator-1) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [陶哲轩文章聚焦纳维－斯托克斯与广义黎曼假设](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 8.0/10

现有材料显示，陶哲轩发布了一篇讨论无外力 Navier–Stokes 奇异性与广义 Riemann 假设的研究文章；随附分析将其描述为 AI 辅助且经过 Lean 形式化验证的数学进展，但未提供文章正文或具体证明内容。一名评论者援引 Lean Zulip 讨论称，结果被两个相互独立的内核接受；这属于评论者报告，而非本次材料中可独立核验的复现结果。材料没有说明所用 AI 系统、其参与环节或复现步骤，因此尚不能据此断言相关开放问题已经解决，也不能把“双内核接受”直接等同于成果正确且可重复。

hackernews · archon1410 · 11月20日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=50578358)

**「此前已有 AI 生成的 Lean 形式化证明」** 2026 年 9 月 8 日，OpenAI 官方页面曾分享一份其称为“AI 生成”的纳维–斯托克斯千禧年难题解法，并附 Lean 形式化证明；这与陶哲 11 月 20 日博文所列的“非受迫”Euler/Navier–Stokes 奇异性及广义黎曼猜想并非同一项成果。检索到的摘要称，后一项工作由 Levent Alpöge、Tristan Buckmaster 和 Matei Coiculescu 在大量 AI 协助下取得新结果，但也指出完整方法与验证情况仍待确认。

**「形式化证明验收需区分两层正确性」** 对采用 AI 辅助形式化证明的团队而言，验收流程需要明确区分“Lean 内核通过”与“形式化陈述确实对应目标定理”：独立报道显示，两套独立构建的检查器已接受据称由 Claude 协助完成的黎曼猜想形式化证明，这降低了单一内核漏洞造成误判的可能性，但并不意味着所有语义问题均已解决。另有报道将相关材料描述为约 940 页手稿和 1,700 万行 Lean 代码，因此发布方仍需提供可审计的命题对应关系、构建与复现说明，不能仅凭编译通过就认定证明正确。

**「社区讨论」** 评论中较具体的技术问题是：一名评论者追问 AI 如何创造 Langlands 等既有框架之外的新抽象，而不只是借助既有概念生成和验证证明；另一名评论者担心 Lean 构建“通过”并不自动保证被形式化的命题正是预期研究目标，这如同“Rust 程序能编译不代表业务逻辑正确”。这些是关于方法边界和形式化对象一致性的质疑，材料未报告已有具体反例；部分参与者同时表达了对 AI 冲击数学研究职业的兴奋与恐惧，但那是个人感受而非已证实结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/">Unforced Euler singularity, unforced Navier-Stokes ...</a></li>
<li><a href="https://todayforai.com/en/items/art-87f06889-96c">Tao Reports AI-Assisted Proofs on Euler and Navier-Stokes ...</a></li>
<li><a href="https://openai.com/index/navier-stokes-solution/">On the Navier–Stokes Millennium Prize Problem | OpenAI</a></li>
<li><a href="https://daily.steinslab.io/en/events/2026-11-21-grh-lean-proof/">The Riemann Hypothesis Meets Its Match: A 940-Page Manuscript ...</a></li>
<li><a href="https://xenospectrum.com/en/claude-riemann-proof-independent-verification/">Two Independent Verifiers Accept Lean Code for Claude ...</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#ai-for-science`

---

<a id="item-tech-news-2"></a>
### [Inkling 2 Mini：循环架构开放权重模型](https://thinkingmachines.ai/news/inkling-2-mini/) ⭐️ 8.0/10

Thinking Machines 宣布发布 Inkling 2 Mini：这是一款面向本地 AI 推理与编程任务的开放权重模型，采用循环架构。发布方称模型训练全程使用 NVFP4，模型尺寸也参考了本地用户的部署需求。不过，现有材料尚未提供可核实的正式基准、完整许可证信息或兼容性清单，其能力与可用性仍需独立测试。

hackernews · jasondavies · 11月20日 20:12 · [社区讨论](https://news.ycombinator.com/item?id=50581260)

**「循环式架构的技术背景」** “循环式架构”是理解 Inkling 2 Mini 的关键：模型会重复执行部分中间层，把更多计算用于每个 token，而不是单纯通过生成更多 token 扩大计算量。Thinking Machines Lab 的架构说明提到该模型采用 NVFP4 端到端训练、低比特量化以及剪枝与修复；Ollama 资料显示其约有 26B 总参数、每个 token 约 5.4B 激活参数，可在配备至少 32GB 内存的 Mac 等本地设备上运行。

**「本地部署与兼容性」** Inkling 2 Mini 已有 Unsloth 和 llama.cpp 的 GGUF 量化版本，可在 Mac、NVIDIA 或 AMD 设备上本地运行；社区早期实测称，32GB M1 Pro 使用 q4\_xl 并同时运行浏览器时约为 10 tokens/s，Ryzen 395 配合 Vulkan 则约为 27 tokens/s 解码速度。依赖 llama.cpp 的用户应先确认相关 PR 的合并状态，因为一名测试者称当时仍有多个未合并 PR，并称应用一个小补丁可提速约 30%；这些性能数据与兼容性信息均属于社区初测，而非官方保证。

**「社区反馈」** 评论者对“循环架构加开放权重”的组合十分兴奋，同时提出广泛开放后如何评估安全性和可解释性的疑问；一名用户报告 Ryzen 395 配合 llama.cpp Vulkan 的解码速度为 27 tokens/s，另一名用户称 32GB M1 Pro 使用 q4 XL 时约为 10 tokens/s。早期编程表现并不一致：CSV 排序任务顺利完成，但硬币类型与年份识别在生成约 12,000 tokens 后仍告失败；部署还需关注 llama.cpp 尚未合并的 PR 32694、32657、32429 和 32704。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://ollama.com/library/inkling-2-mini">inkling - 2 - mini</a></li>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://unsloth.ai/docs/models/inkling-2-mini">Inkling 2 Mini - Run Locally Guide | Unsloth Documentation</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-models`, `#local-ai`, `#open-weights`

---

<a id="item-tech-news-3"></a>
### [OpenAI 测试 ChatGPT 商家资料与智能体后台](https://www.woshipm.com/ai/6497514.html) ⭐️ 8.0/10

据该文对 OpenAI 公告与帮助中心的梳理，OpenAI 于 2026 年 11 月 10 日上线 Businesses in ChatGPT 测试版，向商家免费提供 Business Hub：商家可通过电话、企业邮箱、DNS 或 Shopify 店铺并完成 Persona 身份核验来认领档案，维护网站、简介、品类、Logo、配送与退换政策，并导入包含价格和库存的 CSV 商品清单。认领后，符合资格的美国电商及在线服务商家还能配置并发布 Business Agent，在 ChatGPT 中与企业资料进行独立对话；Insights 看板提供过去 28 天的聚合提及次数、网站点击和发现主题，但不开放单条用户对话。测试仍有明显限制：本地商家目前只能认领既有的美国 listing、不能新建，商家也不能通过该后台直接完成交易，因此它更像商家资料与广告运营入口，而非 ChatGPT 电商结算重启。作者判断短期受挤压的是 Google Business Profile、Yelp 等本地资料与点评平台，而非亚马逊，因为 ChatGPT 仍缺少本地 POI 自主创建、自有评价体系和地图到店场景。

rss · 人人都是产品经理 · 11月20日 09:06

**「从交易试验转向商品发现」** 这并非 ChatGPT 首次试水电商：OpenAI 曾于 2025 年 9 月 29 日与 Stripe、Etsy 和 Shopify 推出 Instant Checkout，让用户可在对话内完成购买，但五个月后撤下该功能，并称初版缺乏预期灵活性，随后转向由商家自行结账、ChatGPT 专注商品发现。2026 年 11 月 10 日上线的 Businesses in ChatGPT 延续了这一路线调整，测试商家认领、资料维护和聚合洞察等功能，而非恢复站内支付。

**「广告主应分开评估 ChatGPT 流量」** 对广告主而言，ChatGPT 广告现阶段更适合作为增量渠道，而非直接替代 Google 搜索广告：Kaiser and Schulze 的工作论文显示，ChatGPT 广告访问转化率为 0.37%，低于 Google 搜索广告的 1.17%，且 97% 的广告主每次访问收入更低。投放团队应分别核算每次访问收入和最终转化，为 ChatGPT 广告设置小规模测试预算；由于广告格式仍在形成，不能仅凭平台流量增长判断稳定回报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-businesses-chatgpt/">Introducing Businesses in ChatGPT - OpenAI</a></li>
<li><a href="https://openai.com/business/businesses-in-chatgpt/">Businesses in ChatGPT: Claim Your Business | OpenAI</a></li>
<li><a href="https://fayfo.com/story/97-of-advertisers-earn-less-from-chatgpt-visits-115729/">97% of Advertisers Earn Less From ChatGPT Visits</a></li>
<li><a href="https://digiday.com/marketing/in-graphic-detail-chatgpt-s-ad-growth-is-outrunning-the-proof-that-it-works/">ChatGPT ’s ad growth is outrunning the proof that it works</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#agents`, `#product`, `#ecommerce`, `#local-search`

---

<a id="item-tech-news-4"></a>
### [拉加德：Pontes 推进欧洲代币化资产统一结算](https://www.panewslab.com/zh/articles/01a1f92c-a0bc-7586-8b57-599d76bfcbbb) ⭐️ 8.0/10

欧洲央行行长克里斯蒂娜·拉加德表示，在适当监管框架下，代币化有望从起步阶段形成欧洲统一的数字资产单一市场；若各平台采用互不兼容的标准和结算体系，市场则可能趋于碎片化。欧洲央行已于 9 月推出 Pontes，使代币化交易能够使用央行货币在欧元体系基础设施上结算；本月早些时候，欧洲稳定机制（ESM）通过 Pontes 完成了一笔 10 亿欧元原生数字债券结算。拉加德援引称，3 月公共区块链上的代币化传统资产规模约 230 亿欧元，是一年前的五倍。她正通过 Appia 与市场参与者推动共同标准，但强调仅有基础设施仍不够，统一规则需要立法者制定，而相关报道尚未提出具体法案或实施时间表。

rss · PANews · 11月20日 13:36

**「Pontes 与数字资产结算基础」** 此前，欧洲央行于 9 月推出 Pontes，使代币化交易能够使用央行货币在欧元体系基础设施上完成结算；本月稍早，欧洲稳定机制（ESM）又通过该系统结算了一笔 10 亿欧元的原生数字债券。拉加德援引的数据是，今年 3 月公共区块链上的代币化传统资产约 230 亿欧元，为一年前的五倍；她据此强调，各平台若形成不同标准且无法相互结算，欧洲市场将趋于碎片化，因此仅有共享基础设施仍不足以形成统一市场。

**「基础设施落地不等于统一市场形成」** 欧洲银行、债券发行人和交易平台已可通过 Pontes 以央行货币结算代币化交易，ESM 的 10 亿欧元原生数字债券提供了实际用例；但要实现真正统一的欧洲数字资产市场，各平台仍需采用共同标准并遵循统一规则，否则代币化资产可能继续因规则不兼容而无法跨平台结算。相关机构应将互操作性和立法协调纳入系统设计，而不能把 Pontes 上线视为统一市场已经形成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://themidpointnews.com/">The MidPoint News | Market structure news. Free. Always.</a></li>

</ul>
</details>

**标签**: `#web3`, `#regulation`, `#digital-assets`, `#infrastructure`

---

<a id="item-tech-news-5"></a>
### [《悦嫂坊》第二版面向独立月嫂提供六项工具](https://www.woshipm.com/ai/6495024.html) ⭐️ 7.0/10

据作者晨阳产品笔记介绍，其通过 AI Coding 将多年设想开发成微信小程序《悦嫂坊》，并在 2026 年 11 月 21 日文章发布前一天推出第二个版本，为独立接私单的月嫂提供月嫂群、电子名片、待产包、月子餐、合同模板和上户日历六项功能；加入同城月嫂群需先添加客服微信并提供所在城市。针对约 40 至 55 岁的主要用户，产品采用大字号、大按钮和口语化字段，并提供 36 项服务勾选、26 天至 52 天档期快捷设置及合同与日历联动。后台还支持经用户同意后代为录入资料和制作名片，但当前暂未接入支付或会员体系；文章也没有提供用户规模、活跃度或实际使用效果等采用证据。

rss · 人人都是产品经理 · 11月21日 03:12

**「私单月嫂的数字化工作背景」** 私单月嫂通常独立接单，日常依赖微信群、熟人转介绍以及手工整理待产清单；作者母亲十余年的从业经验构成了这款产品发现需求的基础。目标用户主要为 40—55 岁从业者，也决定了产品不能只照搬面向年轻人的标准交互，而需要大字号、口语化字段和后台代录入来降低使用门槛。

**「为独立月嫂提供轻量化工具」** 对独立月嫂而言，《悦嫂坊》把名片分享、待产包和月子餐清单、合同生成及档期管理集中到微信小程序中，并为不熟悉上传照片等操作的 40—55 岁目标用户保留“微信提交、运营者后台代录入、首次登录后归属”的兜底流程。由于文中没有用户数、活跃度或留存等采用数据，支付和会员体系也被作者明确暂缓，其实际覆盖效果仍需观察，现阶段更适合视为面向垂直群体的试用工具，而非已验证的规模化服务。

**标签**: `#ai-tools`, `#vibecoding`, `#product`, `#wechat-mini-program`

---

<a id="item-tech-news-6"></a>
### [DeepSeek Harness 七小时复刻 Gemini Flow](https://www.woshipm.com/ai/6497702.html) ⭐️ 7.0/10

作者自述，他用 DeepSeek Harness 在约 7 个有效工作小时内完成 55 轮对话、消耗 4.21 亿 Token、花费 21 元出头，将 Google Gemini Flow 复刻为名为 FlowClone 的原生 Android 应用；该结果主要来自作者自述，尚无独立验证。流程通过 ADB、uiautomator 语义树和截图进行“净室”采集，不反编译原 App，再以 Kotlin、Jetpack Compose 客户端和 Python 服务端重建，并在同一台小米 9 Pro 上逐屏核对；App、服务端规格文件及 bggg-copy-app skill 已发布至 GitHub。作者称验收覆盖了将 8 秒视频延长并合并为 16 秒、用 Media3 Transformer 统一分辨率后重编码，以及持久化长任务、保留多版本素材并把 AI 网关密钥留在后端；过程中首版曾用移动端网页/PWA 代替原生实现，最终仍需返工并重新验收。

rss · 人人都是产品经理 · 11月21日 02:26

**「净室复刻的技术背景」** 此前作者分享过使用 DeepSeek Harness、REA 和 Craft Anything 从零复刻短剧工作室的案例；这次沿用 Craft Anything 的“调查→重建→核对→交付”框架，但转向 Gemini Flow，并改用 ADB 直连真机。所谓“净室复刻”不依赖 jadx 反编译或 Frida 抓包，而是仅观察公开界面和交互结果，再依据 uiautomator 控件结构与截图规格，从零重写 Kotlin 原生端和 Python 服务端。

**「可复用的原型工作流」** 对移动端 AI 开发者，这套成果提供了可直接试用的原型路径：连接开启 USB 调试的 Android 真机后，可用公开的 \`bggg-copy-app\` skill 通过 ADB 采集界面与状态，再以 Kotlin 客户端和 Python 服务端重建；作者还公开了 \`flowclone\` 应用及后端仓库，并要求将 AI 网关密钥保留在后端。实际接入时应确认对标产品是面向视频、图像和自定义工具的 Google Flow，而非 Gemini 的独立视频生成功能；文中所述 7 小时、21 元成本和功能一致性均属作者自述，尚不能视为普遍性能基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toutiao.com/article/7710453302584705536/">7 个小时 21 元，用 DeepSeek Harness 操控手机，复刻所有 APP！</a></li>
<li><a href="https://flow.google.com/">Google Flow - AI Creative Studio for Video , Images &amp; Custom Tools</a></li>
<li><a href="https://gemini.google.com/videos">AI Video Generator &amp; Maker with Veo 3 | Google Gemini</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#vibecoding`, `#ai-agents`, `#product`

---

<a id="item-tech-news-7"></a>
### [Muse 七个月迭代至超千万次下载](https://www.woshipm.com/ai/6497691.html) ⭐️ 7.0/10

据 Meta Muse 产品负责人 Mona Sarantakos 在 Lenny’s Podcast 的首次专访中披露，Muse 从她受 Nat Friedman 邀请后，用树莓派连接邮箱、日历和家庭自动化系统的周末 OpenClaw 实验起步，历经约七个月迭代，已获得超过 1000 万次下载，约四分之一的用户每天使用。开发分为三个阶段：先验证产品形态，随后重点建设可靠性、安全性和信息保护，包括红队测试，以及由多个 Agent 分析真实对话、使用数据并生成合成数据的“智能体集群”，最后通过 Meta 员工内部试用和外部 Alpha 测试完善体验。购物意外成为核心使用场景之一，面向消费者提供比较和缩小商品选择范围的帮助，而用于强化私人化体验的 Jolly 头像也被保留。Sarantakos 还设想让 Muse 登陆智能眼镜和 Charm 等随身硬件并在获得信任后主动行动，但这仍是未来方向，而非本次已交付能力。

rss · 人人都是产品经理 · 11月21日 02:14

**「从 OpenClaw 周末实验起步」** Muse 的前身是 Mona Sarantakos 在 Nat Friedman 邀请下用树莓派搭建的 OpenClaw 周末实验；她接入邮箱、日历和家庭自动化系统后，代理仅凭很少指令便汇总孩子一周的学校通知并生成日程简报。这次体验确立了 Muse“替用户持续行动”的个人 Agent 方向，随后团队用七个月围绕消费者所需的安全性、可靠性、易设置和规模化完善产品。

**「代理购物要求产品适配」** 对开发者和零售商而言，购物已成为 Muse 的核心使用场景之一，Meta 正与零售伙伴试验“商家 Agent 与消费者 Agent 直接沟通”的模式；因此，商品发现、选项比较和后续交易流程需要考虑由个人 Agent 代用户调用的场景。不过目前公开信息仅显示合作伙伴试验，尚未显示已提供通用接口或兼容标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/10/21/meta-says-muse-has-over-10m-users-with-shopping-a-top-activity/">Meta says Muse has over 10 M users, with shopping ... | TechCrunch</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-agents`, `#product`, `#consumer-ai`

---

<a id="item-tech-news-8"></a>
### [MoonPay 申请全国信托银行牌照](https://www.theblock.co/news/business/2026-11-20-moonpay-applies-occ-national-bank-charter-444198) ⭐️ 7.0/10

加密支付公司 MoonPay 已向美国货币监理署（OCC）申请全国信托银行牌照，以扩大受联邦监管的托管和稳定币服务。目前这仅是申请，尚不代表获批，报道也未提供审批时间、牌照条件或具体业务范围。MoonPay 此举加入了申请联邦信托牌照的加密企业行列，而这类申请正面临 increasingly 上升的政治审查。

rss · The Block · 11月20日 10:39

**「全国信托银行牌照的待审性质」** 全国信托银行牌照是由美国货币监理署（OCC）审查的联邦许可申请；若获批，申请机构可在单一联邦监管框架下提供数字资产托管和稳定币相关服务，但提交申请本身不代表已经获批。OCC 的公开清单会列出待审的数字资产许可申请；MoonPay 据报道于 2026 年 11 月 18 日为迈阿密海滩的 national trust bank 提交申请，范围包括托管和稳定币发行，并希望在 GENIUS Act 相关规则开始适用前推进。

**「申请不等于获批」** 本次申请不会使 MoonPay 的托管或稳定币服务立即上线；全国信托银行牌照流程仍包括美国货币监理署（OCC）审查、针对申请人的特定条件以及最终批准，获批前不得开展相关业务。依赖其服务的用户和开发者应等待最终决定并核对适用条件，不应将此次申请视为服务可用性或监管状态已改变的确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theblock.co/news/business/2026-11-20-moonpay-applies-occ-national-bank-charter-444198">MoonPay applies for national trust bank charter to expand ...</a></li>
<li><a href="https://www.occ.gov/topics/charters-and-licensing/digital-assets-licensing-applications/index-digital-assets-licensing-applications.html">Digital Assets Licensing Applications | OCC</a></li>
<li><a href="https://financefeeds.com/moonpay-seeks-occ-bank-charter-for-stablecoin-and-custody-services/">MoonPay Seeks OCC Bank Charter for Stablecoin and Custody ...</a></li>
<li><a href="https://www.itechguides.com/how-crypto-companies-get-a-national-trust-bank-charter/">How Crypto Companies Get an OCC National Trust Bank Charter</a></li>

</ul>
</details>

**标签**: `#web3`, `#stablecoins`, `#regulation`, `#fintech`

---

<a id="item-tech-news-9"></a>
### [Fairmint 拟在 Canton 和以太坊试点代币化股票交易](https://www.coindesk.com/business/2026/11/20/fairmint-plans-tokenized-stock-venue-on-canton-ethereum-under-sec-experiment) ⭐️ 7.0/10

据 CoinDesk 报道，Fairmint 计划由全资子公司 Fairmint TSV LLC 运营代币化股票交易场所，将自动做市商（AMM）与发行人授权的代币化股份连接起来，首期支持 Canton Network，之后计划接入以太坊。场所拟依据美国证券交易委员会（SEC）的“创新豁免”框架运营，但尚未开始交易，仍须满足豁免要求、发布公开通知、完成协议并具备运营条件。首批合作 AMM 为 Tradecraft；Fairmint 的 SEC 注册过户代理子公司 Fairmint TA 将验证持有人、处理转账并维护链上官方所有权记录。

rss · CoinDesk · 11月20日 22:05

**「此前的启动计划」** 此前，Canton Strategic Holdings 于 10 月 29 日宣布与 TSV LLC 合作，计划在 Canton 上发行并交易其代币化股份；CoinDesk 当时称交易可能最早于 11 月初启动，并采用发行人支持的代币化方式以避开公司提出的 30 天异议窗口。截至本次披露，TSV 仍未开始交易，说明此前预计的启动时间尚未兑现。

**「实际影响与上线限制」** 对发行人和投资者而言，Fairmint 计划中的场所将把发行人授权的代币化股份接入 AMM 交易，初期落在 Canton Network；Fairmint TA 将以注册过户代理身份核验持有人、处理转账并维护链上官方所有权记录，Tradecraft 为首个合作 AMM。但交易目前尚未开始，且需满足 SEC 创新豁免条件、发布公开通知、完成相关协议并具备运营条件；以太坊接入也只是后续计划，因此相关方应等待正式公告，不应将跨链交易视为已上线能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/canton-strategic-holdings-moves-tokenize-234500958.html">Canton Strategic Holdings Moves to Tokenize Its Own Shares Under...</a></li>
<li><a href="https://www.coindesk.com/business/2026/10/29/tokenized-stock-venue-on-canton-could-beat-okx-ice-to-first-trade-under-sec-framework">Tokenized stock venue on Canton could beat OKX–ICE to first trade ...</a></li>
<li><a href="https://www.coindesk.com/business/2026/11/20/fairmint-plans-tokenized-stock-venue-on-canton-ethereum-under-sec-experiment">Fairmint plans tokenized stock venue on Canton, Ethereum ...</a></li>
<li><a href="https://phemex.com/news/article/fairmint-plans-tokenized-stock-trading-venue-on-canton-and-ethereum-under-sec-innovation-exemption-104387">Fairmint Tokenized Stock Trading Venue Canton Ethereum SEC E ...</a></li>

</ul>
</details>

**标签**: `#web3`, `#tokenized-assets`, `#ethereum`, `#regulation`, `#product`

---

<a id="item-tech-news-10"></a>
### [Prometheus 测试 12 小时工业设计智能体](http://www.geekpark.net/news/374282) ⭐️ 7.0/10

贝佐斯联合创办并担任联席 CEO 的 Prometheus 在 Semafor 峰会表示，其面向芯片、无线电设备和阀门等任务的“通用 AI 工程师”可在约 12 小时内完成传统上需要 10 至 20 人、耗时 6 至 9 个月的工程设计；该系统以数值仿真神经代理和统一多物理场模型生成设计，并由蓝色起源的两个项目私下内测。Prometheus 并不开发聊天模型或双足机器人，而是定位为 AI 驱动的 CAD、物理仿真与工程智能体；公司估值约 410 亿美元、累计融资约 145 亿美元，但官网尚未公开工具集。上述时长和跨学科能力主要来自贝佐斯及管理层的现场表述，报道未提供独立测试结果，Prometheus 也未给出公开发布时间表，因此实际泛化能力和外部可获取性仍不确定。

rss · 极客公园 · 11月20日 08:24

**「融资背景」** Prometheus 于 2025 年 11 月公开亮相并披露 62 亿美元融资；到 2026 年 6 月，公司完成 120 亿美元融资，估值达到 410 亿美元，资金将用于算力密集的工程、制造和药物设计项目。这构成了此次 410 亿美元估值及其工业 AI 技术路线的直接前史。

**「当前可用性仍受限」** 对潜在工程团队，Prometheus 目前只被用于蓝色起源的两个内部项目私测；所谓“12 小时完成设计”尚非公开可用能力，公司也未给出发布时间表，因此企业现阶段不能据此缩减工程团队或改造现有 CAD 与仿真流程。若未来开放使用，采购方应先用自身的芯片、无线电设备或阀门项目验证结果并测试工作流接入，因为现有方案已覆盖工业设计规划等环节以及物理部件的自主生成，仅凭演示时长不足以证明其能替代传统团队。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/11/project-prometheus-bezos-bajaj-live-updates.html">Jeff Bezos and Vik Bajaj open up about Prometheus</a></li>
<li><a href="https://savedelete.com/read/prometheus-ai-2026.html">Jeff Bezos &#x27;s Prometheus Raises $ 12 B to Build an &#x27;Artificial General</a></li>
<li><a href="https://www.briefia.fr/en/article/la-startup-d-ia-de-jeff-bezos-prometheus-clot-un-tour-de-financement-de-12-milli">Prometheus , Bezos &#x27; AI, Reaches $ 41 Billion Valuation — Brief AI</a></li>
<li><a href="https://www.siemens.com/en-us/company/insights/generative-ai-industrial-copilot/">Siemens Industrial Copilot | Siemens</a></li>
<li><a href="https://leap71.com/">LEAP 71 | Engineering the Future</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#ai-tools`, `#engineering`, `#industrial-ai`, `#product`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [链上买入 ANT 后，你究竟持有什么](https://www.bankless.com/read/what-you-own-when-you-buy-ant-onchain) ⭐️ 8.0/10

rss · Bankless · 11月20日 20:56

**「背景」** 作者以 Anthropic 上市后的链上交易为切口：币圈获得的 IPO 配额远低于预期，投资者只能在股份支持型代币与永续合约间选择；两者价格一度仅差约 0.5%，权利与风险却并不相同。

**「方案」** 支持型代币由发行人买入真实 ANT、托管后铸币；永续合约只是现金结算、没有股份支撑。在作者抓取的数据中，Nasdaq 隔夜报 92.60 美元时，各产品均在 92.29—92.72 美元，但 xyz:ANT 24 小时名义成交约 17.4 亿美元、未平仓约 2.6 亿美元，远高于 Robinhood ANT 的 3200 万美元和 ANTx 的 1400 万美元；链上供给也薄，ANTx 以太坊约 98%疑似仍在发行方钱包。关键差异在条款：支持型代币通常无投票权或直接索赔权，备付口径、赎回资格与开放时间各异，并普遍排除美国用户；永续合约则收付资金费、可加至 10 倍杠杆，且可能在价格反弹前被强平。作者指出，美国人当前最简单的路径仍是直接买股；Kalshi 计划 11 月 23 日推出待批永续合约，而 SEC“创新豁免”要求完整权利、无杠杆、交易量上限及 Anthropic 的 30 日异议权，因此作者判断，带完整权利的美国链上 ANT 可能要到 2027 年或更晚。

**「启示」** 作者的核心结论是，同价不等于同权：永续合约提供流动性和杠杆却不赋予股权，支持型代币更接近股票，却必须逐项核验权利、备付与赎回机制。链上市场补上了 24/7 价格发现和境外二级交易入口，但并未消除 IPO 份额短缺。

**标签**: `#web3`, `#tokenized-assets`, `#crypto-trading`, `#regulation`, `#ai`

---

<a id="item-tech-blog-2"></a>
### [我如何诱使黑客代理执行代码](https://a16zfrontier.com/posts/article/deceiving-ai-hacking-agents/) ⭐️ 8.0/10

rss · a16z crypto · 11月20日 20:55

**「背景」** FBI 在 11 月 13 日警告，开源 LLM 渗透测试平台 ARTEX 已被威胁行为者武器化，用于从侦察到数据外泄的自动化入侵；作者因此追问，防守方能否不只封堵，还能操纵攻击代理的行为。

**「方案」** 他认为代理由模型与负责提示、工具调用和结果处理的代理框架（harness）组成；强化学习强化了任务完成，而拒绝危险行为并不可靠，于是代理往往把最省事的办法当成正解。在获授权的离线 CTF 实验里，他把多阶段“验证码”置于目标服务前，要求先运行指定二进制，却不教 ARTEX 如何过关；普通代理往往会反汇编并提取信息，因此他将文件混淆，让执行看似成为唯一出路。在约 100 次、四个模型的本地运行中（主要是 GLM 5.3 Flash 和 DeepSeek 4.1 1017 Flash），他报告执行率从不足 10%升至接近 100%；日志显示代理会先查 strings、设置超时，再以“属于实验步骤”为由说服自己运行。这不同于明示命令的提示注入，而是借环境设计诱导；但作者称其仍是概念验证，环境简单、关键实现未公开，真实部署效果及模型升级后的稳健性不确定。

**「启示」** 作者的核心结论是：面对任务完成偏置强、拒绝边界薄的黑客代理，可控环境或能成为主动防御层，把攻击者眼中的“捷径”变成防守方的控制点。但现阶段证据尚不足以证明其可广泛部署。

**标签**: `#ai-agents`, `#ai-tools`, `#cybersecurity`, `#defensive-security`

---

<a id="item-tech-blog-3"></a>
### [黎曼猜想双重证明宣称](https://latent.space/p/ainews-riemann-hypothesis-proved-twice-independently/) ⭐️ 6.0/10

rss · Latent Space · 11月21日 05:02

**「背景」** 这期 AI 新闻聚焦两项独立的黎曼猜想证明宣称：Anthropic 数学家 Levent Alpöge 称与 Claude 合作给出 Lean 证明，Alessandro Masullo 则公开约 940 页的人类草稿；两者均未完成独立验证。

**「方案」** 文章援引 Elliot Glazer 的判断：形式命题确为广义黎曼猜想（GRH），Lean 漏洞概率低于 1%，但代码仍在编译，Alpöge 也未披露所用 Claude 模型及人类引导程度，故不能视为已获数学界确认。作者由此对照两者：前者约 1.3GB、折合约 25 万页，可能正确却无人能读完；后者可读却尚未证明正确，而 OpenAI 的纳维–斯托克斯案例还提醒，形式陈述未必对应自然语言结论。协作呈“弱到强”：Alpöge 自称早期借助 Claude，之后在高阶自守形式的关键部分反被其超越；文章转述的工程建议则是先让代理完成可交付实现，再单独重构，并要求人类理解产物。工具与模型动态方面，CodeAF 被称在 DeepSWE 同一开放模型的十个方案中以最低修复成本居首；Inkling 2 Mini 则以 26.4B 总参数、约 3.4B 活跃参数和 100 万上下文主打本地部署，不过这些对比依赖发布方或社区基准。

**「启示」** 作者的核心结论不是“AI 已证明黎曼猜想”，而是 AI 已可能跨越人类的理解与产出尺度，却仍受制于独立验证、命题语义核对和责任审查。

**标签**: `#ai-tools`, `#vibecoding`, `#product`, `#open-models`

---

<a id="item-tech-blog-4"></a>
### [形式化验证：AI 编程的质量防线](https://latent.space/p/formal-verification/) ⭐️ 6.0/10

rss · Latent Space · 11月20日 21:18

**「背景」** 文章把 2026 年 AI 编程的焦虑概括为“slop”：低质模型代码正进入生产环境，而测试、扫描和 AI 自评虽能发现问题，却无法证明遗漏已清零。作者关注的形式化验证以精确规格和机器可检的证明补位，但现有材料主要是厂商访谈，成本与采用障碍仍缺少完整评估。

**「方案」** &amp;Truth 联合创始人 Clark Barrett 称，其“验证机”要读取任意语言代码、围绕精确需求生成 Lean 证明，再由开源证明助手 Lean 逐步检查；可信点不是“AI 一定正确”，而是错误无法混过检查器。Harmonic 的 Aristotle 也采用“AI 写证明、Lean 验证”，Axiom Math 则用证明反馈训练数学推理系统；安全场景包括检查 C 代码内存安全，Theorem 关于规模化防御的说法仍属厂商主张。Anthropic 与 Theorem 的合作报告了有限数据：36 个小型验证任务上，Opus 5.5 求解率 50%，token 比 Opus 5 少约 40%，不过验证目前仍很耗 token。工作流上，作者描述从“vibe-coding”转向“veri-coding”：智能体先协助写规格，再编码并协同验证器，人工转向审查。Barrett 另称，cvc5 已在 Amazon 流水线每天调用数十亿次，用于 Kiro 的规格分析和测试生成。

**「启示」** 作者的核心判断是，随着智能体承担更多编码，形式化验证可能成为检查交付正确性的实用层，但仍是有希望且受成本约束的方向。

**标签**: `#ai-tools`, `#vibecoding`, `#formal-verification`, `#developer-tools`

---

<a id="item-tech-blog-5"></a>
### [Anthropic IPO 与本地 AI 工程观察](https://latent.space/p/ainews-anthropic-successfully-completes-largest-ipo-in-history-valued-at-1-5t/) ⭐️ 5.0/10

rss · Latent Space · 11月20日 07:12

**「背景」** 作者汇总 12 个 subreddit 和 544 个 X 账号，以 Anthropic 上市为主线，并整理本地语音、算力、仿真和 Claude 生成项目，追问安全、资本与算力承诺如何同时落地。

**「方案」** 文章据上市材料与社交动态称，Anthropic 以每股 83 美元定价，开盘 111.50 美元、收盘 97.17 美元；813 亿美元募资超过 SpaceX 的 750 亿美元，计入私募后预计净募资 1048 亿美元，开盘全面摊薄估值约 2 万亿美元。Dario 承诺训练和部署以安全及保持人为控制为前提，Class F 掌握 50.1%投票权；作者提醒未来一年约万亿美元级股票解禁。S-1 显示公司募资约 1400 亿后仍有 1320 亿现金，烧钱较少，但资金将主要用于数据中心租赁；按 FT Unhedged 的 20%回报、40%经营利润率与 17%税率假设，兑现估值需约 6020 亿美元年收入。工程条目呈现轻量化的取舍：Kitten-TTS-2 最小 4 MB、支持至多 16 种语言，但早期测试称标点韵律偏弱；AudioGhost 省去约 25 GB 辅助模型下载、将小模型显存降至略高于 4 GB，代价是质量下降且偏 NVIDIA。299 kB 的 Voidstruck 在运行时生成 1.5 亿恒星系统；ETH Zurich 称仿真策略可零样本控制 5 吨装载机，DeepSeek V5 全用华为 Ascend 训练的说法则因缺少运行数据仍未证实。

**「启示」** 文章的核心不是给出单一技术结论，而是把 IPO 后的治理与财务压力，同本地 AI 的质量和硬件依赖问题并置。它更像一份高密度线索清单，其中不少说法仍需原始材料验证。

**标签**: `#ai-tools`, `#vibecoding`, `#local-ai`, `#ai-business`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [鸿蒙高校创新赛发布高校应用孵化计划](https://sspai.com/post/119291) ⭐️ 6.0/10

2026 鸿蒙高校创新赛总决赛在南京大学举行颁奖典礼，赛事已被列入全国普通高校学科竞赛排行榜；本届赛事吸引 800 多所高校、近 5000 支队伍和近万名学生，收到 2800 多份有效作品，并安排了 10 余场线上线下技术辅导。华为现场发布“鸿蒙高校创新孵化计划”，拟为获奖且成功上架华为应用市场的学生作品提供技术支持、上架辅导和流量扶持。文章重点呈现视障出行、养老院卧床护理和独居长辈关怀等场景中的作品，团队将缺测保留、防止障碍误判、区分操作状态及确认后才执行等规则写入设计；但现有材料没有给出完整工作流、实际产品表现或可复核成效。

rss · 少数派 · 11月21日 04:00

**「为何值得关注」** 赛事把高校开发教育、比赛辅导和上架孵化放在同一条路径上，且参赛项目集中于视障出行、养老照护和独居关怀等对误判与错误动作更敏感的场景。现在适合讨论的不是“AI 已经替代照护”，而是这些原型如何通过拒答规则、状态区分和人工确认约束自动化边界；计划能否转化为稳定上架和可验证的用户效果，材料尚未说明。

**「内容切入点」** 可做角度：围绕《灵触随行》《卧安智护》《银龄心语》中的“系统不做什么”，具体拆解视障导航、卧床压力监测和独居关怀如何处理缺测、误判、状态确认与隐私边界，而不是把 AI 描述成已经可靠地替代人的照护者。

**标签**: `#ai-agents`, `#harmonyos`, `#product-development`, `#creator-tools`, `#case-study`

---