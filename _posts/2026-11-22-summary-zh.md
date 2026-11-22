---
layout: default
title: "Horizon Summary: 2026-11-22 (ZH)"
date: 2026-11-22
lang: zh
---

> 从 144 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Lean 与 Mathlib 称 Anthropic 黎曼猜想证明通过核验](#item-tech-news-1) ⭐️ 8.0/10
2. [腾讯混元公开 Hy4 架构与路线](#item-tech-news-2) ⭐️ 8.0/10
3. [Creatify Max 将 AI 视频生成延伸至广告投放管理](#item-tech-news-3) ⭐️ 7.0/10
4. [即梦 AI 三大工作室打通短剧创作流程](#item-tech-news-4) ⭐️ 7.0/10
5. [harness-hub 推出 Qwen3.8-27B 的 Pi Agent 专用 LoRA](#item-tech-news-5) ⭐️ 7.0/10
6. [Kling Image 4.0 电商长图与原生 8K 实测](#item-tech-news-6) ⭐️ 7.0/10
7. [Tether 四笔投资押注 USDT 跨境通道](#item-tech-news-7) ⭐️ 7.0/10
8. [Cyber 调查 CYBER 异常铸造，两家韩国交易所暂停充提](#item-tech-news-8) ⭐️ 7.0/10
9. [Chainflip 因潜在金库漏洞暂停核心服务](#item-tech-news-9) ⭐️ 7.0/10
10. [欧洲央行征集代币化资产实验伙伴](#item-tech-news-10) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Lean 与 Mathlib 称 Anthropic 黎曼猜想证明通过核验](https://www.panewslab.com/zh/articles/01a2010d-7fa0-7032-bd06-92025f3c8730) ⭐️ 8.0/10

据 PANews 转述的 Lean 与 Mathlib 联合声明，Anthropic 数学研究员 Levent Alpöge 以约 1700 万行 Lean 代码实现了黎曼猜想的形式化证明。联合声明称，该成果满足四项核验：数学表述经过专家审查、代码能够成功编译、两种独立工具确认所证命题与黎曼猜想完全一致，以及 Lean 证明通过多个独立检查器交叉验证，其中部分检查器还带有基于集合论的形式化正确性证明。声明未说明 AI 参与证明的具体方式和复现步骤；数学界下一步将研究并解释该证明蕴含的新思路。

rss · PANews · 11月22日 02:19

**「形式化验证与发布背景」** 这里的“Lean 验证”是指把黎曼猜想的数学陈述和证明步骤写成可由编译器及独立证明检查器核验的代码；Mathlib 是其中使用的 Lean 数学库。联合声明还单独核验了代码所证明的命题与黎曼猜想完全一致。此前报道显示，Levent Alpöge 于 11 月 20 日发布了约 1700 万行的证明库，Lean FRO 与 Mathlib Initiative 于 11 月 21 日公布社区认证，因此本次消息是此前发布及核验工作的后续确认。

**「对形式化验证开发者的直接影响」** 形式化数学开发者现在可以获得一个包含 175,187 个文件、约 1700 万行的 Lean 归档，并将其作为超大证明自动化流程的研究样本；Lean 与 Mathlib 社区称，该成果通过了命题匹配、编译及多个证明内核的交叉检查。对于依赖可复现验证的团队，现有材料仍未说明 Claude 的具体参与方式和完整复现步骤，因此该归档应先作为研究型证明成果审阅，不宜未经验证便接入关键工作流。

**「检查器独立性与人类把关受到关注」** Hacker News 评论者认为，不同语言和不同一致性保证构成的多个检查内核，使利用漏洞伪造证明的可能性很低；但也有人以曾有伪造的 Collatz 反例通过单个检查器为例，质疑这些工具是否真正独立。另有评论者指出，本次有人类数学专家把关可降低 Claude 钻漏洞的风险，并将更大功劳归于 Levent 善于运用 Claude；其关于成果还会影响数学基础的判断仍只是评论者推测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datastudios.org/post/claude-riemann-hypothesis-proof-lean-community-certifies-levent-alpoge">Claude-assisted Riemann hypothesis proof certified by Lean ...</a></li>
<li><a href="https://officechai.com/ai/lean-community-certifies-levent-alpoges-claude-assisted-proof-of-the-riemann-hypothesis-as-correct/">Lean Community Certifies Levent Alpöge’s Claude-Assisted ...</a></li>
<li><a href="https://casrai.org/news/anthropic-levent-alpoge-claude-lean-riemann-hypothesis-claim-2026">175,000-File Lean Riemann Hypothesis Proof Claim — CASRAI</a></li>
<li><a href="https://www.datastudios.org/post/claude-riemann-hypothesis-proof-lean-community-certifies-levent-alpoge">Claude-assisted Riemann hypothesis proof certified by Lean ...</a></li>
<li><a href="https://www.unite.ai/lean-and-mathlib-communities-certify-claude-assisted-riemann-proof/">Lean and Mathlib Communities Certify Claude-Assisted Riemann ...</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#engineering`

---

<a id="item-tech-news-2"></a>
### [腾讯混元公开 Hy4 架构与路线](http://www.geekpark.net/news/374301) ⭐️ 8.0/10

腾讯混元团队首次面向全球开发者在 Reddit LocalLLaMA 举行公开 AMA，介绍 11 月 4 日发布的 Hy4、随后推出的 Hy4 flash，以及 Hy4-mini、Flash-Lite、24–31B 稠密模型和 5–12B 开源图像模型等规划。报道援引团队说法称，Hy4 登上 Agent Arena 开源模型榜首、位列 Artificial Analysis 中国模型第二，Hy4 flash 的单任务成本约为 Hy4 的二十分之一，首日 Token 调用量超过 50 万亿；但榜单方法、评测细节和可复现信息仍不充分。Hy4 flash 继承 iHC、门控 MLA 和 DSA，并加入混合 SWA、LatentMoE 与 Engram，团队称 SWA 可将 KV cache 压缩至原方案的四分之一；运行 Hy4 flash 需要 96GB 显存和 128GB 系统内存，llama.cpp 适配仍在推进，目前已可在 OpenCode、Claude Code、Cline 中使用。姚顺雨及团队承认 Hy4 存在思维链过长、创意写作可读性不足和递归自我改进仍处早期等问题，Hy4 flash 则通过强化学习控制思维链长度；团队将 Hy4 自评为 AGI 2.5 级，但这属于内部判断而非外部验证。

rss · 极客公园 · 11月22日 01:56

**「Hy4 系列的研发基础」** 极客公园的报道回顾了 Hy4 系列的研发基础：混元团队今年 2 月完成预训练与强化学习基础设施重建，随后于 11 月 4 日发布 Hy4，并在一周后推出主打成本的 Hy4 flash。Hy4 对应扩大模型与数据规模、探索能力上限的路线，Hy4 flash 则对应压缩推理成本的路线；此次 AMA 讨论的 Scaling Law、MoE 稀疏度、量化和端侧部署，均是这一“双线并行”架构与产品取舍的延伸。

**「对代理开发的实际影响」** 对代理编码和长上下文工作流，Hy4 flash 提供了可落地的降本选项：据第三方汇总的腾讯内部 WorkIndex 数据，其平均单任务成本约为完整版 Hy4 的二十分之一；官方资料确认该模型拥有 224B 总参数、每 token 激活 12B，并支持原生多模态和 1M-token 上下文。开发者目前已可在 OpenCode、Claude Code 和 Cline 中使用；若选择本地运行，报道给出的硬件门槛是 96GB 显存加 128GB 系统内存，并需将部分专家层和 Engram 表卸载到主机内存，而 llama.cpp 适配仍在推进，因此现阶段更适合先通过 API 验证工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4-flash">Introducing Hy4 flash: Ultimate cost ... - hy.tencent.ai</a></li>
<li><a href="https://www.mindstudio.ai/blog/tencent-hy4-flash-benchmarks">Tencent Hy4-Flash Benchmarks: How It Stacks Up on Cost vs ...</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#agent-coding`, `#open-source-models`, `#model-engineering`, `#product`

---

<a id="item-tech-news-3"></a>
### [Creatify Max 将 AI 视频生成延伸至广告投放管理](https://www.woshipm.com/chuangye/6497546.html) ⭐️ 7.0/10

Creatify 于 11 月 18 日推出 Creatify Max，将广告研究、视频脚本与素材生成、投放管理和效果分析整合进同一 AI 助手。商家连接 Shopify、Google Analytics、CRM 以及 Meta、Google、TikTok 广告账户后，可用自然语言排查异常、比较广告表现、生成新素材并创建广告系列，但上线、暂停或调整预算等关键操作仍需用户审批。公司披露的案例显示，阿里巴巴卖家三个月累计制作逾 20 万条视频，其中逾 80% 被投入真实广告活动；Designrr 案例则称获客成本从 55 美元降至 30 美元，广告支出回报率从 0.77 升至 1.33。由于 Max 刚发布，这些效果数据主要来自公司案例，其长期稳定性、跨平台判断能力及真实客户回报仍缺少第三方验证。

rss · 人人都是产品经理 · 11月22日 05:32

**「从视频生成走向投放管理」** Creatify 最初以“从商品链接生成视频广告”为核心，2025 年推出 AdMax 以扩展到创意分析与测试，2026 年 5 月又发布 Creatify Agent，加入基于历史投放表现的创意建议。Creatify Max 延续了这一产品演进路线；Creatify 官方将其描述为能够监控广告账户、复用有效创意，并跨 Meta、Google 和 TikTok 创建广告的“AI teammate”。

**「跨平台投放整合与预算风险」** 对同时经营 Meta、Google 和 TikTok 广告的商家，Creatify Max 可把 Shopify、Google Analytics、CRM 与广告账户接入同一助手，集中诊断异常、迭代素材，并将上线、暂停或调整预算等关键操作提交人工审批；但商家目前不宜取消审批，因为错误建议会直接造成预算损失，不同平台的归因口径和接口权限也可能不一致。外部资料显示，Google Performance Max 已提供 AI 素材生成与预测分析，Meta Advantage+ 也支持把静态照片转成视频广告，因此企业评估 Creatify 时应同时比较平台原生能力、跨平台数据完整性和接口兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://creatify.ai/blog/meet-creatify-max-ai-marketing-agent">Meet Creatify Max: The AI Marketing Agent for Ads</a></li>
<li><a href="https://htbusinessgroup.com/ai-in-digital-marketing-online-advertising/">AI in Digital Marketing: How It&#x27;s Changing Online Ads</a></li>
<li><a href="https://tinyhousemarketing.beehiiv.com/p/ai-advertising-week-of-nov-6-2026">AI + Advertising : week of Nov 6, 2026</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#product`, `#ecommerce`, `#adtech`

---

<a id="item-tech-news-4"></a>
### [即梦 AI 三大工作室打通短剧创作流程](https://www.woshipm.com/ai/6497998.html) ⭐️ 7.0/10

即梦 AI 已把短剧、动效和营销制作整合为三个网页工作室：短剧工作室于 10 月 26 日上线，动效与营销工作室分别于 11 月 10 日和 16 日上线，面向希望用自然语言完成低门槛视频制作的个人创作者和机构。短剧链路由 DreamScript、Anycook、DreamShot 与 Seedance 2.5 分别处理剧本、图片、分镜和视频，官方称 DreamScript 可解析 10 万字小说、最多连续生成 100 集；项目还支持 3D 导演台、智能预演、样片转成片、多轨后期及导入剪映。作者实测能从模糊想法推进到完整短片，但人物动作细节仍有不足，分镜控制、平台审核和生成随机性也需要人工处理；复杂 Web 项目的卡顿与稳定性同样构成限制。

rss · 人人都是产品经理 · 11月22日 02:26

**「从短剧 Agent 到一体化工作台」** 此前字节先以小云雀短剧 Agent 跑通短剧创作，再将其并入即梦；视频模型 Seedance 也从单段最长 15 秒的 2.0 迭代到单段最长 30 秒的 2.5。此次更新的重点不只是增加生成入口，而是把剧本、资产一致性、分镜编排、视频生成和后期串进同一项目，并进一步扩展到动效及商品营销工作流。

**「降低工具与试错成本」** 积分只在调用生成模型时消耗，创作者可先通过智能预演和样片模式试错，再生成高画质片段；局部重拍能只处理最短 4 秒的区间，定稿后还能导入剪映继续精剪。与此同时，用户仍需人工复审分镜和提示词，并按 Seedance 2.5 单段最长 30 秒的限制设计片段切分；处理复杂多轨项目的机构还应考虑 Web 端卡顿和稳定性波动。

**标签**: `#ai-tools`, `#creator`, `#product`, `#ai-video`

---

<a id="item-tech-news-5"></a>
### [harness-hub 推出 Qwen3.8-27B 的 Pi Agent 专用 LoRA](https://www.woshipm.com/ai/6497995.html) ⭐️ 7.0/10

harness-hub 发布了面向 Pi Agent 的 Qwen3.8-27B-pi-adapted LoRA，体积约 319 MB，无需修改原 27B 基座，也可选择 28.6 GB 的合并 Q8\_0 权重。文章转述官方模型卡与评测称，该适配器直接在 Pi v1.5.2 容器中以异步 GRPO 训练；在 Pi、关闭思考、单次 pass@1、100 步上限和 131,072 上下文条件下，SWE-bench Pro hard 51 通过率由基座的 39.2% 提升到 64.7%，Terminal-Bench 2.1 的 83 题通过率由 41.0% 提升到 56.6%。相较开启 xhigh 思考的基座，生成 Token 中位数据称分别从 48.8k 和 16.5k 降至 9.4k 和 3.7k，但这些仍是文章整理的官方结果，尚非独立复现。

rss · 人人都是产品经理 · 11月22日 01:26

**「在真实 Pi 环境中训练适配器」** Harness Adapter 的关键不是另行模拟 Agent 循环，而是把实际使用的 Agent harness——此处为 Pi v1.5.2——置于强化学习环境中，让模型在真实的工具调用、上下文和停止条件下完成代码修复，从而减少训练与部署环境不一致的问题。Hugging Face 的发布说明将 Qwen3.8-27B-pi-adapted 描述为“在 Pi 内以强化学习训练”的 LoRA，GGUF 模型树也确认其适配器形态，这正是该版本无需替换 27B 基座即可针对 Pi 优化的技术背景。

**「实际影响」** 对于使用 Pi Agent 的本地开发团队，可在保留基座权重的情况下挂载该 LoRA，并通过 llama.cpp、Llama.app、vLLM 动态 LoRA，或 PEFT 合并权重后接入，以减少代码修复任务的生成开销。接入时需要关闭思考并匹配训练接口：vLLM 的 LoRA rank 应设为 32，Pi 的 provider 需将 api 指定为 openai-completions 而非默认的 Responses API；官方还建议优先使用更接近 BF16 训练分布的 Q8\_0，较低精度量化可能带来更大偏移。

<details><summary>参考链接</summary>
<ul>
<li>Hugging Face Releases Qwen3.8-27B-pi-adapted LoRA ...</li>
<li>Model tree for harness-hub/Qwen3.8-27B-pi ...</li>

</ul>
</details>

**标签**: `#ai-tools`, `#coding-agents`, `#vibecoding`, `#local-llm`, `#qwen`

---

<a id="item-tech-news-6"></a>
### [Kling Image 4.0 电商长图与原生 8K 实测](https://www.woshipm.com/ai/6497881.html) ⭐️ 7.0/10

据第三方实测文章，可灵 AI 已上线 Kling Image 4.0，用户可选择“电商详情页”或“网页设计”技能，输入白底商品图和自然语言需求，直接生成长图；文章称其能够一次完成图标、复杂文字排版和规格表，并提供短、中、长三种页面长度。组图模式一次最多可输出 10 张风格统一且前后关联的图片，该版本还支持原生 8K 直出、局部智能改字，以及 70 多款预设字体和上传参考图新建字体。作者称在二十多组、五类案例中取得了较好效果，但这是第三方体验，来源内容不完整，“首次支持原生 8K”等主张也缺少原始发布资料佐证。

rss · 人人都是产品经理 · 11月22日 00:44

**「理解 Image 4.0 的产品定位」** 可灵官方对 Kling 4.0 与 3.0 的比较主要涉及视频生成，包括最长 30 秒原生生成、10 个关键帧、Omni Reference 和 Dynamic Motions；本文讨论的 Kling Image 4.0 属于图像生成产品线，不应把上述视频规格与其长图、8K 输出能力混用。作者回顾称，早期模型连手指数量都需要靠抽卡，后来虽能生成光影较好的单张图片，却常在加入文字后出现乱码，因此此次电商长图、规格表和中文排版测试，实质是在检验模型能否从“单张图好看”进一步走向“整页信息可交付”。

**「实际影响」** 对电商运营、独立站设计和营销素材创作者而言，“商品图加一句需求”的生成路径可直接用于页面草稿，组图、局部改字和字体切换也可能减少重复排版工作；不过在用于商品上线或广告投放前，仍应逐张核对规格文字、品牌字样、商品与人物一致性以及 8K 输出效果，因为文中结果属于第三方体验，未提供可复现的测试条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://klingai.com/blog/kling-4-vs-3">Kling 4.0 vs 3.0: What’s Different in the New Model?</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#image-generation`, `#product`, `#creator`

---

<a id="item-tech-news-7"></a>
### [Tether 四笔投资押注 USDT 跨境通道](https://www.panewslab.com/zh/articles/01a201c1-0a33-75d3-b6ed-44c5c1eec5be) ⭐️ 7.0/10

据 PANews/深潮 TechFlow 11 月 22 日报道，Tether 在 11 月 16 日至 19 日连续投资四家稳定币支付与流动性公司：领投巴西美元账户服务商 Nomad 的 C 轮并出资 1500 万美元，投资年处理逾 20 亿美元 USDT 交易的 Stables，与阿布扎比 Further Asset Management 合计向新加坡持牌支付机构 MetaComp 投入约 1000 万美元，以及投资受瑞士 FINMA 和 VQF 监管的 SCRYPT。Nomad 此轮融资总额为 1.72 亿雷亚尔、投后估值 40 亿雷亚尔；该报道未披露 Stables 和 SCRYPT 的投资金额。报道将这组动作解读为战略转向：在截至 9 月 30 日储备资产达 1915 亿美元、前九个月净经营利润为 45 亿美元且 USDT 发行量停在约 1840 亿美元后，Tether 试图通过入股本地金融应用、支付基础设施和持牌机构，扩大 USDT 在工资、汇款和跨境贸易中的实际使用。不过，入股不等于产品已经上线：Nomad 的 USDT 和 XAUT 接入仍在探索且没有时间表，MetaComp 的资金计划用于扩充合规及跨境通道，Stables 和 SCRYPT 的成效亦未披露，因此目前更适合将其视为尚待验证的战略布局。

rss · PANews · 11月22日 05:36

**「此前的渠道布局」** Tether 的经常性利润主要来自 USDT 储备资产投资短期美债和回购所获利息；当流通规模与利率同时承压时，把稳定币接入真实支付和结算场景便成为扩大储备规模的一条路径。PANews 将这一战略追溯至 2024 年 4 月的四大板块重组，以及同年 6 月对台北 XREX 的 1,875 万美元投资；本次四笔交易属于该既有布局的延续，而非首次转向。

**「接入前需核验落地与牌照」** 对计划接入 USDT 的支付机构、跨境商户和开发者而言，Tether 投资某家公司并不等于该渠道已支持 USDT：Nomad 的 USDT 接入仍处探索阶段且未公布上线时间，Ualá 也因当地监管限制尚未接入，因此项目方应逐项确认牌照、代币可交易性和实际上线日期。MiCA 对发行方设有消费者保护、市场诚信和金融稳定要求，而 Binance 已下架不合规稳定币交易对、保留合规稳定币和欧元交易对，同一套接入方案可能因平台和司法辖区而不可用。

<details><summary>参考链接</summary>
<ul>
<li>Tether Invests in Four Companies to Expand Global Payment Channels</li>
<li>Tether News</li>
<li>Tether on X</li>
<li><a href="https://www.chainalysis.com/blog/stablecoins-most-popular-asset/">Stablecoins 101: Behind crypto’s most popular asset - Chainalysis</a></li>
<li><a href="https://www.binance.com/en/support/announcement/detail/bcaa1f68d6a6450099056ff694ad6c46">Binance Will Delist Non- MiCA Compliant Stablecoin Trading Pairs For...</a></li>

</ul>
</details>

**标签**: `#web3`, `#stablecoins`, `#payments`, `#investment`

---

<a id="item-tech-news-8"></a>
### [Cyber 调查 CYBER 异常铸造，两家韩国交易所暂停充提](https://www.panewslab.com/zh/articles/01a20124-7f44-721b-9fca-d6ba733287ae) ⭐️ 7.0/10

L2 网络 Cyber 正在调查 CYBER 代币在 Solana 上被异常铸造，以及 CYBER 从跨链桥的以太坊锁定池中被转出的事件，受影响资产和具体跨链路径仍有待核实。Cyber 要求用户暂时停止使用 CYBER 跨链桥、不要向交易所充值，也无需迁移代币、连接钱包或签名。Upbit 和 Bithumb 已因疑似安全事件暂停 CYBER 充值和提现；由于原因尚未查清，目前不能将相关异常定性为已确认的协议级失窃。

rss · PANews · 11月22日 02:45

**「背景」** Cyber 是面向社交功能的 L2 网络，报道中的异常分别涉及 Solana 上的代币铸造端和跨链桥的以太坊锁定池端。理解此类事件需要区分“异常铸造”与“锁定池资产流出”；两者同时被调查并不等于已确认存在同一攻击路径或协议级失窃，Cyber 仍在核实受影响资产及具体跨链路径。

**「充提与跨链暂时受限」** Upbit 和 Bithumb 已暂停 CYBER 充值与提现，Cyber 同时要求用户暂停使用 CYBER 跨链桥且不要将 CYBER 充值至交易所，因此相关用户目前无法通过两家韩国交易所或该桥正常充提、跨链。Cyber 表示用户无需迁移代币、连接钱包或签名，但事件原因、受影响资产和资金路径仍在核实，用户应等待官方进一步确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bingx.com/en/flash-news/post/cyber-investigating-suspected-million-bridge-exploit-as-upbit-bithumb-freeze-transfers">Cyber investigates suspected $1 million bridge exploit as Upbit and...</a></li>

</ul>
</details>

**标签**: `#web3`, `#security`, `#bridges`, `#L2`

---

<a id="item-tech-news-9"></a>
### [Chainflip 因潜在金库漏洞暂停核心服务](https://www.panewslab.com/zh/articles/01a1fed7-9ee1-7480-b8d3-c5b72dff8a12) ⭐️ 7.0/10

跨链交易协议 Chainflip 表示，团队发现一个可能影响金库（Vaults）的潜在漏洞，已预防性启动“全面安全模式（Full Safe Mode）”，暂停存款、提现、兑换和报价服务。官方正在调查，但尚未披露漏洞成因、影响范围或潜在损失；此前关于协议遭攻击、损失约 486 万美元且 ETH 被 Tornado Cash 洗白的说法仍待核实。用户现阶段应避免与协议进行资金交互，并等待后续技术公告。

rss · PANews · 11月21日 16:01

**「前序安全警报」** 此前已有安全监控标记 Chainflip 的以太坊金库出现约 486 万美元的流出，The Defiant 报道称这是监控系统给出的估值；另有消息称资金经 Tornado Cash 洗白为 ETH，但这并非 Chainflip 已确认的损失结论。官方当时仍只表示正在调查“潜在漏洞”，具体成因、影响范围及损失均待后续技术说明。

**「核心服务全面暂停」** Chainflip 启用 Full Safe Mode 后已暂停存款、提现、兑换和报价服务，依赖这些功能的用户及集成方需要停止操作并等待官方公布调查结果。外部链上报道估算约 486 万美元资产被盗并流向 Tornado Cash，但官方尚未披露漏洞原因、最终损失或影响范围，因此该金额仍属于待进一步核实的估算。

<details><summary>参考链接</summary>
<ul>
<li>Chainflip Halts Swaps Over Potential Vault Exploit - The Defiant</li>
<li><a href="https://bingx.com/en/flash-news/post/chainflip-ethereum-vault-drained-of-m-in-minutes-as-flip-drops">Cointelegraph: REKT: $ 4 . 86 M exits Chainflip Ethereum vault via...</a></li>
<li><a href="https://forklog.com/en/chainflip-halts-operations-due-to-potential-hack/">Chainflip Halts Operations Due to Potential Hack | ForkLog</a></li>

</ul>
</details>

**标签**: `#web3`, `#security`, `#chainflip`, `#defi`

---

<a id="item-tech-news-10"></a>
### [欧洲央行征集代币化资产实验伙伴](https://www.panewslab.com/zh/articles/01a1fd83-e9df-75ef-8e69-36035d0ac11d) ⭐️ 7.0/10

欧洲央行正通过“Appia”倡议邀请金融行业以联合倡议形式参与实验，探索代币化存款及相关支付、代币化证券和共享网络治理三类工作流；申请方须由独立法律实体组成，可申请其中一个或多个工作流。首批申请截止日期为 12 月 11 日，后续申请将滚动评估，方案将依据专业知识、实践经验、技术准备情况和预期贡献等标准遴选。欧洲央行计划于 2028 年发布蓝图，汇总实验发现并提出框架建议；目前仍处于征集与试验阶段，并非已经落地的代币化产品或监管规则。

rss · PANews · 11月21日 09:50

**「实验背景」** “Appia”是欧洲央行用于探索代币化金融工作流和共享网络治理的实验倡议，已划定代币化存款及支付、代币化证券和共享网络治理三个优先领域。参与者须由独立法律实体组成联合倡议，可申请一个或多个工作流；首批申请截止日期为 12 月 11 日，后续申请将滚动评估，欧洲央行计划于 2028 年根据实验发现提出相关框架建议。

**「参与门槛与申报时间表」** 银行及其他金融机构若要参加首轮 Appia 实验，必须由独立法律实体组成集体倡议，共同申报代币化存款与支付、代币化证券或共享网络治理中的一个或多个工作流；首批申请截止 12 月 11 日，之后滚动评估，筛选依据包括专业知识、实践经验、技术准备和预期贡献。因此，申请方需要先完成法律实体协作并证明技术准备度；在欧洲央行计划于 2028 年发布相关发现和建议框架蓝图之前，该机制仍属试验，而非已落地的生产网络或确定规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ecb.europa.eu/press/pr/date/2026/html/ecb.pr260311~14ddf51a77.en.html">Eurosystem Unveils Appia Roadmap for Europe’s Tokenised Finance</a></li>
<li><a href="https://finance-monthly.com/ecb-appia-tokenisation-initiative/">ECB Opens Appia Tokenisation Initiative to Financial Firms</a></li>

</ul>
</details>

**标签**: `#web3`, `#tokenization`, `#regulation`, `#infrastructure`

---