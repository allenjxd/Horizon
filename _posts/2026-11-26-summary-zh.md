---
layout: default
title: "Horizon Summary: 2026-11-26 (ZH)"
date: 2026-11-26
lang: zh
---

> 从 196 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [HungerG 编程与办公能力实测](#item-tech-news-1) ⭐️ 7.0/10
2. [MAGI-2：480B MoE 视频模型低价发布](#item-tech-news-2) ⭐️ 7.0/10
3. [小鹏计划 2027 年 1 月量产 IRON 人形机器人](#item-tech-news-3) ⭐️ 7.0/10
4. [LayerZero 新增三星卡、Kakao Pay 和 ZAN 为 Zero 创世验证者](#item-tech-news-4) ⭐️ 7.0/10

**科技博客**
1. [tacit.wei 的隐私池借力设计](#item-tech-blog-1) ⭐️ 8.0/10

**AI 创作者雷达**
1. [Claude Artifacts 桌面应用安装进入 Beta](#item-ai-creator-1) ⭐️ 8.0/10
2. [用 AI 开发交互式中国历史地图：200 多次迭代记录](#item-ai-creator-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [HungerG 编程与办公能力实测](https://www.woshipm.com/ai/6500809.html) ⭐️ 7.0/10

匿名多模态模型 HungerG 已免费上线 AI 编程平台 Qoder 和 OpenCode；平台页面称其支持约 100 万上下文、原生多模态并不使用用户数据训练，但模型身份和正式 model card 尚未确认。作者在 Qoder 实测中让它用 13 分钟交付 1331 行 Three.js 收割机代码，并完成可连续拆解的机械蜻蜓、交互式黑洞网页和 675KB 单文件环西湖游戏；其 Three.js 建模、动画和交互完成度较高，办公场景也能生成经作者人工核对后数据基本无明显问题的 Word、Excel、PPT 三份报告。作者认为其 Coding 和 Working 质量已站稳其所称的“新一线”水平，但收割机缺少音效且只能沿固定路线运行，游戏仍偏原型、任务深度有限，三份办公文档的美观度也有待提升。

rss · 人人都是产品经理 · 11月26日 07:13

**「HungerG 的匿名试用背景」** HungerG 并非以正式命名的模型发布，而是以匿名条目出现在 OpenCode 模型目录中；开发者记录显示，\`hungerg-free\` 条目曾短暂上线、约 20 分钟后撤下，标称 100 万 token 上下文。外部报道还称该模型在 Qoder 免费开放至 11 月 30 日，因此本文的实测属于平台早期试用，而非已有正式 model card 的稳定版本。指向 StepFun Step 5 的线索目前仅来自分词器检查，尚不能视为厂商确认。

**「试用价值与落地风险」** 对需要在 Qoder 或 OpenCode 中快速生成可运行网页的开发者，HungerG 目前可免费试用；作者实测其能交付单文件 Three.js 场景及可编辑的 Word、Excel、PPT 文件。不过，生成物仍存在缺少音效、手动驾驶控制有限和办公文档设计偏粗糙等问题，且模型身份、正式 model card 及“不使用用户数据训练”的承诺尚未得到确认，因此生产接入前应先验证功能完整度与交付稳定性，不宜将其当作已确定的长期模型依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.orcarouter.ai/ru/blog/hungerg-stealth-model-leak">HungerG Stealth Model : что показывают данные StepFun</a></li>
<li>HungerG 隐身模型：StepFun 证据揭示了什么 - OrcaRouter</li>

</ul>
</details>

**标签**: `#ai-tools`, `#vibecoding`, `#3d`, `#product`

---

<a id="item-tech-news-2"></a>
### [MAGI-2：480B MoE 视频模型低价发布](https://www.woshipm.com/ai/6500800.html) ⭐️ 7.0/10

Sand.ai 推出面向视频创作者与开发者的 MAGI-2，采用 480B 总参数、约 28B 激活参数的 MoE 架构，并以 Multi-Head Latent MoE 将跨卡通信与 top-k 路由解耦；团队称在总 FLOPs 相同且各自采用最优配置时，其训练速度比 LatentMoE 快约 22%。模型支持单次生成 4–30 秒、1080p、25fps 的音画同步视频，可混用最多 20 份图片、视频和音频参考，按时间点控制切镜，并在生成后通过文字指令修改；1080p 视频最低价格为 0.05 元/秒。文章还展示了关闭提示词扩写（PE）后，模型从缺失 45 格的 9×9 数独起始帧中逐步填满答案的案例，但该结果来自团队访谈和演示，尚未得到独立验证。现有材料缺少可复核的完整基准和一手文档，且作者指出其复杂声场下的音效层次仍弱于 Seedance，后训练也会降低关闭 PE 时的数独复现率。

rss · 人人都是产品经理 · 11月26日 06:39

**「从 Preview 到 MAGI-2」** MAGI-2 沿用了 Sand.ai 数月前发布的 Preview 版路线：后者以 114B 总参数、6B 激活参数打通了视频 MoE 的算法与基础设施，并验证了文本、视频和音频 token 在同一序列中交互。MAGI-2 将其扩展至 480B 总参数、约 28B 激活参数，并采用 Multi-Head Latent MoE，将各 head 的本地 top-k 路由与跨卡通信解耦；官方资料称，每个 head 都拥有独立的路由器和专家池。

**「创作者与开发者的成本与接入影响」** 按 Sand.ai 在访谈中给出的定价，1080p 视频生成最低为 0.05 元/秒，团队可以更低成本地批量试错、筛选生成片段；Higgsfield 已提供 MAGI-2 入口，支持最长 30 秒、1080p、25 fps，并同步生成对白、音效和配乐。接入方仍应使用自有素材测试端到端延迟和成片质量，因为采访方称 MoE 推理通常比 Dense 模型慢 20% 至 30%，现有材料也未提供可复核的完整性价比基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sand.ai/blog/magi-2/">MAGI - 2 : A 480 B Frontier Video Generation Model</a></li>
<li><a href="https://higgsfield.ai/magi-2-intro">MAGI - 2 AI Video Generator with Sound | Higgsfield</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#video-generation`, `#model-architecture`, `#generative-ai`

---

<a id="item-tech-news-3"></a>
### [小鹏计划 2027 年 1 月量产 IRON 人形机器人](https://www.woshipm.com/share/6500701.html) ⭐️ 7.0/10

小鹏在第八届科技日发布贯通汽车与机器人的图灵具身智能架构 VLA 3.0，并称第一台 IRON 人形机器人已完成生产验证，计划于 2027 年 1 月进入硬件量产，2027 年第一季度先在部分中国门店实习、第二季度才正式对外发布。IRON 的公布参数包括身高 170 厘米、76 个自由度、3 颗自研图灵芯片和最高 2250 TOPS 端侧有效算力，并计划以导购、导览等室内岗位切入；这些量产时间、性能与商业化能力目前主要来自小鹏发布会自述，尚无实际工位部署、客户订单或成本数据可独立验证。小鹏正将智能汽车、Robotaxi、飞行汽车与机器人统一到物理 AI 技术栈，但对外可用能力仍取决于 2027 年的量产、门店实习和正式发布节点。

rss · 人人都是产品经理 · 11月26日 05:56

**「从舞台验证到量产准备」** 在上一届小鹏科技日上，小鹏曾现场剪开 IRON 的腿部外皮，以证明机器人并非真人替身；此后一年多，公司重启了机器人的硬件、软件与 AI 架构，并建设自动化产线和数据工厂。此次完成首台生产验证意味着 IRON 已从舞台演示推进到制造准备阶段，但硬件量产、门店实习和正式发布仍分别计划于 2027 年 1 月、第一季度和第二季度。

**「先在门店验证，再开放商用」** 对小鹏门店、零售客户和生态开发者，IRON 将先以导购、导览等岗位进入小鹏中国门店实习，再于 2027 年第二季度正式对外发布；合作伙伴可从开放平台下载 Skills，并通过语音、App 或简易编程二次开发。不过，“2 人 48 小时跑通中等复杂度场景”仍是小鹏给出的部署目标，且目前缺少实际客户、成本和长期运行数据，潜在客户宜先开展现场概念验证，不宜将其视为已经验证的规模化交付能力。

<details><summary>参考链接</summary>
<ul>
<li>先门店试用，再对外商用：小鹏IRON现在能干哪些实际工作？_智能机器人</li>

</ul>
</details>

**标签**: `#physical-ai`, `#robotics`, `#embodied-ai`, `#product`, `#manufacturing`

---

<a id="item-tech-news-4"></a>
### [LayerZero 新增三星卡、Kakao Pay 和 ZAN 为 Zero 创世验证者](https://www.theblock.co/news/business/2026-11-25-layerzero-kakaopay-samsung-446770) ⭐️ 7.0/10

LayerZero 宣布将三星卡、Kakao Pay 和 ZAN 新增为即将上线的 Zero 区块链创世验证者，三者将在主网启动时协助保障网络共识和证明验证，其中 Four Pillars 将代表三星卡运营验证节点。Zero 使用零知识证明将交易执行与验证分离，让验证者只需验证证明，从而减少一层冗余。网络计划于 11 月 30 日与 LayerZero 的 ATLAS 交易基础设施同步上线，质押的 ZRO 将在 2027 年 3 月 31 日前平均分配给创世验证者；这些上线和分配安排仍属于官方计划。

rss · The Block · 11月26日 02:22

**「Zero 的验证架构」** Zero 利用零知识证明将交易执行与验证分离：验证者只需检查证明，无须重复执行交易，从而减少一层冗余。三家支付相关机构此次将以创世验证者身份加入，Four Pillars 则将代表三星卡运营验证节点；据报道，Zero 主网计划于 11 月 30 日与 LayerZero 的 ATLAS 交易基础设施同步上线。

**「创世验证者加入」** Zero 的初始验证层将新增三星卡、Kakao Pay 和 ZAN，三者将作为创世验证者参与主网共识维护和 ZK 证明验证，其中三星卡的节点由 Four Pillars 运营。由于验证者只需验证证明而无须重复执行交易，支付相关机构此次加入的是 Zero 的证明验证与共识环节。由于 Zero 计划与 LayerZero 的 ATLAS 基础设施于 11 月 30 日同步上线，集成方仍需以主网实际启动和节点运行状态为准，不能将当前公告视为已经交付的上线能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theblock.co/news/business/2026-11-25-layerzero-kakaopay-samsung-446770">LayerZero adds Samsung Card, Kakao Pay, ZAN as validators for ...</a></li>
<li><a href="https://www.chaincatcher.com/en/article/2308127">LayerZero incorporates Samsung Card, Kakao...</a></li>

</ul>
</details>

**标签**: `#web3`, `#layerzero`, `#zk-proofs`, `#validators`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [tacit.wei 的隐私池借力设计](https://www.bankless.com/read/inside-tacit-wei-the-app-behind-tacits-breakout) ⭐️ 8.0/10

rss · Bankless · 11月26日 05:23

**「背景」** 多链隐私项目 Tacit 从比特币扩展至 Ethereum，tacit.wei 是其私密 ETH 前端；TAC 随之在一周内由约 0.16 美元涨至一度近 1.46 美元。

**「方案」** tacit.wei 是 Tacit Pay 前端：一次交易内把存款拆成 Tornado Cash 的 0.1 或 1 ETH 固定份额，余数进入 Tacit 自有池；提款默认由 Tacit 中继提交，以免可关联钱包为新地址补 gas，也可自行中继，v0.2 还加入了私密换币。作者称关键在于借 Tornado 约 5.66 亿美元 TVL 的深度立即扩大匿名集合，并让自有池承接余数、逐步成长，而非与 Tornado 竞争。链上界面可经 tacit.wei.limo 等网关访问，比 2022 年 Tornado 网站被关停更难整体下线；但仍依赖默认中继和负责名称、端点的 Z DAO。应用会在 Tornado 存款后不足 20 笔入账时警告不要过早提款；比特币方向的 Praxis 则以见证加密把密钥使用权绑定到可证明条件，满足者可用普通签名花费而无需改链，可望支撑无托管桥。不过 Praxis 的可信设置要求至少一方销毁随机性，公钥仪式沿用 Succinct 设置并让浏览器贡献随机性（最多奖励 5 TAC）；作者提醒，这些项目仍是早期实验、似乎仅做过 AI 安全审查，TAC 流动性也薄。

**「启示」** 作者认为，tacit.wei 以成熟流动性嫁接链上前端和隐私护栏，展示了实用化路径，但安全与流动性仍待验证。

**标签**: `#web3`, `#product`, `#privacy`, `#defi`, `#bitcoin`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [Claude Artifacts 桌面应用安装进入 Beta](https://sspai.com/post/119560) ⭐️ 8.0/10

Anthropic 于 11 月 25 日宣布，Claude 的交互式 Artifacts 支持以“安装为应用”方式安装到 macOS 和 Windows 桌面。安装后可从独立图标启动，并可选择默认权限，或开放通知、快捷键拦截、窗口置顶及完整计算机访问权限。该功能目前处于 Beta 阶段，正逐步向桌面用户开放，但具体开放范围和推送节奏尚未明确。

rss · 少数派 · 11月26日 00:08

**「工作流与权限边界待验证」** 这一变化使 Claude 生成的应用从浏览器标签页进一步走向独立桌面工具，值得关注安装与交付流程是否更顺畅。已确认的变化是桌面安装功能进入 Beta；完整计算机访问等权限的实际边界与稳定性仍需实测。

**「实测桌面权限」** 可做角度：围绕 Claude Artifacts 的“安装为应用”做一次桌面工作流与权限边界实测，分别记录默认模式、通知、快捷键、窗口置顶和完整计算机访问权限下的使用体验。

**标签**: `#ai-tools`, `#creator`, `#workflow`, `#product`

---

<a id="item-ai-creator-2"></a>
### [用 AI 开发交互式中国历史地图：200 多次迭代记录](https://sspai.com/post/117510) ⭐️ 7.0/10

程序员 DeanChen 借助 AI 开发了交互式中国历史地图「江山时序」，最初仅用一句“帮我做一个能够拖动时间轴的中国历史地图”提示词生成粗糙初版，随后在两周半内进行了两百多次代码修改。项目逐步加入时间轴、城市历史沿革、人物行迹和自然语言查询等功能，并参考开源数据集、《资治通鉴》及各朝正史人工纠正边界问题。GitHub star 数从几十增长至 1400，传播主要始于 X 上的一次转发；不过文章尚未完整说明数据来源、史实校验方法、技术栈、成本及后续转化方式。

rss · 少数派 · 11月26日 03:13

**「个人兴趣借 AI 加速成形」** 作者表示，Vibe Coding 的流行让他首次有了把长期兴趣落实为网站的机会，并在 10 月重新启动项目。这已经是一个可验证的创作过程，但“模型能力又上了一个台阶”仍是作者的主观感受，不能等同于 AI 已能可靠生成历史事实。

**「从兴趣原型到垂直工具」** 可做角度：复盘一句提示词如何演变为包含时间轴、人物与城市交互的历史地图工具，同时明确区分 AI 对开发效率的帮助与疆界、事件等史实内容仍需查证和人工纠错的责任边界。

**标签**: `#ai-tools`, `#creator`, `#vibe-coding`, `#interactive-map`, `#product`

---