---
layout: default
title: "Horizon Summary: 2026-11-23 (ZH)"
date: 2026-11-23
lang: zh
---

> 从 151 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [Lean 与 Mathlib 称 Claude 协助的黎曼猜想证明正确](#item-tech-news-1) ⭐️ 8.0/10
2. [VMEG AI 推出企业级视频本地化工作流](#item-tech-news-2) ⭐️ 7.0/10
3. [智谱 GLM-5.4 上线 Coding Plan](#item-tech-news-3) ⭐️ 7.0/10
4. [Visa 扩展可信代理协议并推出 Visa CLI 实验钱包](#item-tech-news-4) ⭐️ 7.0/10
5. [Blur 失效多签后约 545.6 枚 ETH 被锁死](#item-tech-news-5) ⭐️ 7.0/10
6. [Fusionist 跨链桥疑被利用，超 6 万亿枚 ACE 遭铸造](#item-tech-news-6) ⭐️ 7.0/10
7. [帕霍茨基提议先进模型统一安全门槛](#item-tech-news-7) ⭐️ 7.0/10

**AI 创作者雷达**
1. [Charles Lamanna 谈 AI 代理时代的工程角色](#item-ai-creator-1) ⭐️ 6.0/10
2. [Claude 参与黎曼猜想证明，正式审查尚未完成](#item-ai-creator-2) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Lean 与 Mathlib 称 Claude 协助的黎曼猜想证明正确](https://www.panewslab.com/zh/articles/01a20261-882e-73d5-af92-7fb26f4a6cd2) ⭐️ 8.0/10

Lean 与 Mathlib 联合声明称，他们对 Levent Alpöge 借助 Claude 完成的黎曼猜想形式化证明正确“完全有信心”，约 1700 万行、175,187 个模块的 Lean 源码也已公开供他人重建。MIT 数学家 Andrew Sutherland 据报已用 Lean 与 Mathlib v4.33.1 独立编译，其中 5 个模块提高默认计算步数上限后通过，并核对 8322 个 Mathlib 编译文件与官方缓存逐字节一致；约 61.6GB 的导出物另由 nanoda、con-leche、con-ron 等检查器交叉复核。现有命题与公理检查据称确认代码对应 Mathlib 的 RiemannHypothesis 定义，Main.lean 的五个定理仅依赖 propext、Classical.choice 和 Quot.sound，且不含 sorryAx；但联合声明未公布比较器和官方内核的具体版本及完整日志，Lean v4.36.0 的部分端到端测试截至 11 月 21 日 12:55 UTC 仍在运行，旧版 con-leche 与 con-ron 则因不支持一种返回类型以退出码 2 中止，报道称这不代表证明被拒绝。因此，这仍是社区背书和机器可复核证据，并非学界已经理解整套证明或千禧年大奖获得正式认可；主定理与四个狄利克雷 L 函数定理应否统称 GRH 仍有口径差异，获奖仍需正式发表、至少两年公开检验及国际数学界普遍接受。

rss · PANews · 11月23日 01:00

**「形式化验证与前期进展」** Lean/Mathlib 的形式化验证，是把目标命题的定义、公理依赖和每一步推导写成可由 Lean 内核检查的代码；因此，机器能逐步检查代码中的推导，却仍需确认代码表达的正是标准黎曼猜想、未使用 \`sorry\` 占位符，并信任验证内核。此次工作并非从零起步：Anthropic 今年 8 月曾公布 Claude 配合 Lean 将关键线上零点比例下界从 41.6% 提高到 67.2%，但当时明确不预期这些技术最终证明黎曼猜想；MIT 数学家 Andrew Sutherland 随后公开的验证文件则分别记录了独立重建、命题比对和公理检查。

**「对 AI 科研与形式化验证团队的影响」** 这项工作给 AI 科研团队提供了一套可复用的验收流程：锁定 Lean 与 Mathlib 版本、从源码重建 175,187 个模块、核对目标定义与公理依赖，再通过多个独立内核交叉检查约 61.6GB 的证明导出文件。组织不应把“Claude 生成完成”直接标记为“解决黎曼猜想”：虽然 Lean 与 Mathlib 已公开背书，但部分收尾测试和公开审查仍未完成，克雷数学研究所也将黎曼猜想列为尚未解决的千禧年难题，100 万美元奖金尚不能申领。

<details><summary>参考链接</summary>
<ul>
<li>The AI Riemann hypothesis proof is true, independent mathematicians ...</li>
<li>RH Lean proof: verification files - MIT Mathematics</li>
<li><a href="https://www.claymath.org/events/millennium-prize-problems-lecture-series/">Millennium Prize Problems Lecture Series - Clay Mathematics Institute</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#ai-research`

---

<a id="item-tech-news-2"></a>
### [VMEG AI 推出企业级视频本地化工作流](https://www.woshipm.com/chuangye/6497922.html) ⭐️ 7.0/10

VMEG AI 已将视频翻译服务扩展为企业级工作流：平台可将中文视频翻译为 170 多种语言，并提供音色克隆、多说话人识别和口型同步；2026 年 6 月推出的 Glass Box Dubbing Workflow 还允许用户查看原文、译文、配音和时间轴，通过术语表、发音词典及局部重新生成修改内容，而不必重做整段视频。公司披露，平台累计注册用户已超过 200 万、服务 1200 多家企业，2025 年团队不足 20 人，年度经常性收入超过 200 万美元；这些数字来自公司披露，不代表 200 万付费用户或已实现同额年度收入。企业客户案例显示，其价值主要来自跨平台分发、专业术语审核、批量交付和可修改流程，例如 TELUS Health 的 360 分钟英法双语医学内容在一周内交付，但项目节省约 60%成本的结论同样由 VMEG 公布，且目前缺少第三方质量对比、付费率和留存率数据。

rss · 人人都是产品经理 · 11月23日 02:44

**「从营销视频到企业本地化」** VMEG 最初以 Clip to Video 广告素材生成为主，2024 年转向海外市场后于同年 5 月上线视频翻译，并随创作者和企业需求逐步加入多语言配音、声音克隆与口型同步。2026 年，公司又推出 Glass Box Dubbing Workflow，让企业检查转写、译文、人物配音和时间轴，并只修改、重新生成有问题的片段，以适应专业术语审核和按期交付。

**「采购与授权影响」** 企业在 HeyGen、ElevenLabs Dubbing v2 与 VMEG 之间选型时，不能仅凭“支持 170 多种语言、声音克隆和口型同步”认定 VMEG 具备差异化：HeyGen 已提供 175 种以上语言及方言的翻译、声音保留与口型同步，ElevenLabs Dubbing v2 也支持 90 种以上语言和口音并自动克隆原说话者音色，因此应针对实际语言和场景测试译文、节奏、口型及局部返工成本。涉及主持人、演员或高管声音时，企业还应把授权范围、使用期限和人工审核写入项目流程，不能仅凭拥有原视频版权就默认具备跨语言声音克隆权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businesswire.com/news/home/20260626000999/en/VMEG-AI-Surpasses-$2M-ARR-Launches-Glass-Box-Dubbing-Workflow-for-Enterprise-Video-Localization">VMEG AI Surpasses $ 2 M ARR , Launches Glass Box Dubbing ...</a></li>
<li><a href="https://www.vmeg.ai/enterprise/">Enterprise AI Video Localization &amp; Dubbing Platform | VMEG . AI</a></li>
<li><a href="https://www.heygen.com/translate">AI Video Translator : Translate Videos into 175 + Languages</a></li>
<li><a href="https://elevenlabs.io/dubbing-studio">Dubbing v 2 : Dub content across 90 + languages and accents.</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#creator`, `#product`, `#ai-video`

---

<a id="item-tech-news-3"></a>
### [智谱 GLM-5.4 上线 Coding Plan](https://www.panewslab.com/zh/articles/01a20706-2ea1-74db-b899-b4f20f4cd322) ⭐️ 7.0/10

智谱官方运营人员称，GLM-5.4 已接入 Coding Plan，用户将模型名设置为 glm-5.4 即可使用；该版本新增视觉能力，并强化通用编码能力。V2、V3 和团队版用户使用 GLM-5.4 的额度已提升至原来的 1.5 倍。报道未提供基准测试、完整套餐规则或官方文档，实际能力提升与额度适用条件仍待验证。

rss · PANews · 11月23日 06:09

**「既有 GLM 模型的多模态基础」** 此次更新并非 GLM 系列首次支持视觉输入：OpenRouter 此前已将 GLM-5.3-Flash 标为原生多模态模型。不过，智谱称 GLM-5.4 是在过去三个月同步推进 Scaling Loop 与模型规模后的版本，并新增视觉及泛 Coding 能力；由于报道未提供基准测试，其相对 GLM-5.3-Flash 的提升幅度尚无法量化。

**「Coding Plan 额度与可用性变化」** 智谱 Coding Plan 的 V2、V3 和团队版用户现在可将模型名设置为 \`glm-5.4\`，使用其视觉能力与通用编码能力，并获得提升至 1.5 倍的 GLM-5.4 模型额度。由于报道未提供基准测试、详细套餐规则或官方文档，额度的具体计算方式及实际效果仍需以官方说明和实测为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/z-ai/glm-5.3-flash">GLM 5 .3 Flash - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#vibecoding`, `#coding-agents`, `#product`

---

<a id="item-tech-news-4"></a>
### [Visa 扩展可信代理协议并推出 Visa CLI 实验钱包](https://www.panewslab.com/zh/articles/01a205ee-c563-7109-9307-765cdd7344b6) ⭐️ 7.0/10

Visa 宣布扩展可信代理协议（Trusted Agent Protocol，TAP）和 Visa Agent Directory，使美国用户能够通过连接钱包并安全添加银行卡来验证代理并将其注册到目录。经 Visa 验证的代理可承接有偿任务并赚取 OUSD，任务涵盖视频创作、音乐作曲、游戏、付费调查和市场研究等类型。Visa 还面向美国用户推出实验性 Visa CLI 代理钱包，该钱包基于 Tempo 和机器支付协议（MPP），用于连接主流代理平台。

rss · PANews · 11月23日 01:04

**「可信代理协议的验证基础」** Visa 于 2025 年 10 月 14 日首次公布可信代理协议（TAP）时，将其定位为代理商务的基础框架；该协议采用代理专属的加密签名，帮助商户在结账过程中验证代理身份和凭证，并降低恶意机器人干扰交易的风险。此次扩展是在原有可信代理验证机制之上接入代理钱包、Visa Agent Directory 与任务市场，使 TAP 从识别和授权可信代理进一步延伸至代理接单与支付。

**「开发者获得代理接单路径」** 开发者可通过 TAP 和 Visa Agent Directory 打通代理验证、目录注册、任务承接及 OUSD 收款流程；若要使用 Visa CLI，则需注意其目前仅面向美国用户，且仍属基于 Tempo 和 MPP 构建的实验性产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx">Visa - Visa Introduces Trusted Agent Protocol: An Ecosystem ...</a></li>
<li><a href="https://usa.visa.com/about-visa/newsroom/press-releases.releaseId.21716.html">Visa Introduces Trusted Agent Protocol: An Ecosystem-Led ...</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#web3`, `#ai-tools`, `#payments`, `#product`

---

<a id="item-tech-news-5"></a>
### [Blur 失效多签后约 545.6 枚 ETH 被锁死](https://www.panewslab.com/zh/articles/01a205dd-70bf-7444-bdc7-80822b8f743a) ⭐️ 7.0/10

据 PANews 转述 Yuga Labs 区块链副总裁 Quit 的检查，Blur 已通过交易使控制 Blur、Blend 和 BlurPool 的 Safe 多签失效，相关合约无法再升级，约 545.6 枚 ETH 因此永久锁定在 Blur Pool。Quit 检查约 12.5 万个 Blur Pool 持有地址后发现，889 个合约共持有 1,216 枚 ETH，其中 315 个不可变合约因未实现 withdraw\(\) 提款函数而无法取回资金，涉及 Moonbirds（173.2 ETH）、Milady（85 ETH）和 0xSplits（82.6 ETH）；另有 558 个合约持有的约 550.9 枚 ETH 仍可提取，但尚未完成提款。Blur 交易界面已于 11 月 12 日关闭，但协议仍在链上运行，Upbit 则计划于 11 月 30 日下架 BLUR。

rss · PANews · 11月23日 00:45

**「背景：合约升级与退出机制」** 在此次锁仓发生前，Blur 已于 11 月 12 日关闭交易界面，但协议本身仍保持链上运行；Upbit 此前宣布将于 11 月 30 日下架 BLUR。可升级合约原本可由 Safe 多签修改逻辑，而永久不可升级的合约必须内置可用的提款路径，否则即使协议仍运行，合约中的 ETH 也无法取出。

**「不可升级且缺少提款函数的合约资金无法找回」** 持有 Blur Pool 余额的合约若已不可升级且未实现 withdraw\(\) 函数，项目方或持有者便无法提取其中的 ETH；核查发现，315 个此类合约共锁定约 545.6 ETH，Moonbirds、Milady 和 0xSplits 均涉及其中。继续使用 Blur Pool 的团队应在上线前审查合约升级权限和提款路径，并区分已永久锁仓的资产与尚可提取但尚未提款的余额。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coingabbar.com/en/blur-eth-locked-545-6-eth-trapped-315-immutable-contracts">Blur ETH Locked: 545.6 ETH Trapped in 315 Contracts</a></li>
<li><a href="https://en.coin-turk.com/blur-pool-locks-545-6-eth-as-contract-upgrade-path-permanently-closed/">Blur Pool locks 545.6 ETH as contract upgrade path ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/approximately-545-6-eth-permanently-locked-in-blur-pool-affecting-multiple-projects">Approximately 545.6 ETH permanently locked in Blur Pool ...</a></li>

</ul>
</details>

**标签**: `#web3`, `#ethereum`, `#nft`, `#protocol-governance`

---

<a id="item-tech-news-6"></a>
### [Fusionist 跨链桥疑被利用，超 6 万亿枚 ACE 遭铸造](https://www.panewslab.com/zh/articles/01a204d5-66bf-75a7-9719-0d8e39ab8fa4) ⭐️ 7.0/10

Fusionist 的 BNB Chain 跨链桥铸币者权限疑遭利用，攻击者据报道铸造了超过 6 万亿枚无抵押 ACE，将其兑换为 USDT 后经多个钱包跨链转移。PANews 援引消息称，攻击者还通过 Tornado Cash 转移了 1091.5 枚 ETH，约合 187 万美元；但另一则消息称被铸造的 ACE 为 10 千万亿枚、抽走约 104 万美元 USDT，数量与损失金额存在不一致。现有报道未说明权限失守的根因，也未提供项目方的修复方案。

rss · PANews · 11月22日 19:56

**「跨链桥铸币权限与损失口径」** Fusionist Bridge 的特权铸币者权限可在 BNB Chain 上生成 ACE；若该权限被接管，攻击者便能绕过正常抵押或发行约束，直接制造无抵押代币。本文还援引早前消息称铸造规模为 10 千万亿枚、约抽取 104 万美元 USDT，这一数字与本文所称超过 6 万亿枚及 1091.5 枚 ETH（约合 187 万美元）不一致，事件规模仍需核实。

**「ACE 供应与跨链桥风险」** 对 ACE 持有者和做市方而言，超过 6 万亿枚无抵押 ACE 被铸出并兑换为 USDT，已对代币供应和价格可信度造成冲击；报道中的“6 万亿”与“10 千万亿”两种数量，以及约 104 万美元与 187 万美元两种资金口径尚未统一，不能据此确认最终损失。事件调查完成前，项目方应限制被利用的 BNB Chain 跨链桥特权铸币权限并核对链上记录，交易所、桥接用户和交易者也应审慎处理 Fusionist Bridge 及 ACE 的充值和交易。

**标签**: `#web3`, `#security`, `#bridge`, `#tokenomics`, `#gaming`

---

<a id="item-tech-news-7"></a>
### [帕霍茨基提议先进模型统一安全门槛](http://www.geekpark.net/news/374304) ⭐️ 7.0/10

OpenAI 首席科学家雅库布·帕霍茨基于当地时间 2026 年 11 月 22 日发文，提议 AI 企业共同制定先进模型的评测、透明度和安全红队测试标准，并承诺在达到明确的安全监控里程碑前不突破限制；CEO 萨姆·奥尔特曼公开支持，但该方案目前仍是个人倡议，尚非已执行的行业标准。帕霍茨基建议以可跨企业追踪的困惑度作为首个门槛，并披露 OpenAI 内部数据：GPT-3.5 和 GPT-4 的对数困惑度约为 0.99 和 0.91，低于 0.8 时曾观察到网络安全和数学领域的新能力，约 0.76 时则在部分开放数学问题上取得突破。他预计模型最早可能在 2027 年加速预训练进展，而对齐和行为监控可能无法同步跟上；0.68 至 0.7 区间或出现更多变革性能力，但具体能力仍不确定，因此相关阈值和时间判断属于其预测，而非经验证的性能保证。

rss · 极客公园 · 11月23日 01:22

**「困惑度与前沿训练暂停的背景」** 这里的“困惑度”指模型预测下一个 Token 的对数困惑度，可作为追踪预训练进展的连续指标；OpenAI 给出的参照是 GPT-3.5 约 0.99、GPT-4 约 0.91，并称约 0.76 时模型在部分开放数学问题上开始取得突破（tool-2-1, tool-2-2）。要求前沿训练暂停或设限已有既有讨论，已有研究专门评估“硬暂停”的可行性，而帕霍茨基的方案进一步把可跨企业追踪的数值门槛与安全监控条件结合起来（tool-2-3）。

**「模型发布流程与合规影响」** 若各实验室采纳这项提案，前沿模型在首次投入使用前将需要提供跨企业可比的困惑度（或交叉熵损失）评测、透明度和安全红队测试证据，并以达到新的行为监控能力为放行条件；这将增加模型发布审计与安全工程工作，也改变下游采购方需要索取的证明材料。帕霍茨基提出的 0.68—0.70 困惑度区间只是其预测的潜在能力跃迁区，并非已经生效的监管或行业强制门槛；在共识形成前，开发者不应将其视为合规要求，但可提前整理可跨模型比较的评测与监控记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/openais-pachocki-urges-frontier-pause-at-068-07-perplexity">OpenAI&#x27;s Pachocki urges frontier pause at 0 . 68 - 0 . 7 perplexity</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>
<li><a href="https://hardwired-pause.ai/paper">The Feasibility of a Hardwired Pause of Frontier AI Training</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#ai-safety`, `#model-evaluation`, `#ai-development`, `#standards`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [Charles Lamanna 谈 AI 代理时代的工程角色](https://creatoreconomy.so/p/what-should-engineers-do-when-ai-writes-all-the-code-charles-lamanna) ⭐️ 6.0/10

Peter Yang 于 2026 年 11 月 22 日整理了对微软 Copilot 与 Agents 业务执行副总裁 Charles Lamanna 的访谈。受访者认为，当编码成本下降时，工程师会少写代码，但将更多精力投入架构、测试、扩缩容以及与 AI 代理对齐。文章还转述 Satya Nadella 的看法，即个人贡献者更像“带着 token 预算管理代理的人”，并以 Copilot Cowork 由 11 名工程师打造、GitHub Copilot runtime 由 1 名工程师维护等案例加以说明。访谈还讨论了多代理协作、Copilot 与 Office 的关系及微软围绕 Copilot 重构 Office 的方向，但材料没有提供明确的产品发布、版本变化、可复核数据或操作步骤。

rss · Creator Economy So · 11月22日 15:03

**「为何值得关注」** 材料将讨论重点从 AI 辅助写代码推进到工程师如何管理代理、对齐结果和承担更高层面的设计问题，也涉及多代理协作与 Office/Copilot 调整。不过，这些内容目前主要属于访谈观点和个例，尚不足以证明工程岗位或产品形态已经发生确定性变化。

**「可做角度」** 可做角度：从“个人贡献者更像带着 token 预算管理代理的人”这一访谈比喻切入，解释受访者所说的工程重心变化——少写代码，更多投入架构、测试、扩缩容和对齐，同时注明这并非已经验证的岗位趋势。

**标签**: `#ai-agents`, `#ai-tools`, `#creator-workflows`, `#microsoft-copilot`

---

<a id="item-ai-creator-2"></a>
### [Claude 参与黎曼猜想证明，正式审查尚未完成](https://sspai.com/post/119418) ⭐️ 6.0/10

据 11 月 20 日发布的信息，Anthropic 数学研究员 Levent Alpöge 宣称使用 Claude 找到黎曼猜想及广义黎曼猜想的证明，并完成 Lean 形式化；Andrew Sutherland 等人的初步核查显示，全部 Lean 模块已通过编译与多项检查。完整论文仍待整理，核心理论和完整验证尚未完成；Lean 与 Mathlib 社区确认提交的形式化证明正确，但数学界仍需解析其思路并开展进一步审查。形式化核验可以检查证明逻辑是否成立，但不能替代人类对数学思想的理解，因此目前不能将黎曼猜想视为已获正式认定。

rss · 少数派 · 11月22日 23:34

**「新声明引发关注」** 研究人员的公开声明、初步编译核查以及 Lean 与 Mathlib 社区的后续确认，使这项成果在 11 月 20 日至 21 日迅速受到关注。不过，完整论文、完整验证和学界广泛审查仍在进行，已经发生的是形式化证明通过检查，尚未证实的是黎曼猜想获得正式解决。

**「解释形式化验证的边界」** 可做角度：以“Lean 通过编译检查”与“学界正式认定猜想获解”的差别为主线，解释形式化验证能够检查什么，以及为什么它仍不能替代论文审查和数学家对证明逻辑的理解。

**标签**: `#ai-tools`, `#formal-verification`, `#ai-research`, `#creator-workflow`, `#mathematics`

---