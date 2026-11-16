---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 154 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Qwen4-Max 上线：2.4T MoE 与百万上下文](#item-tech-news-1) ⭐️ 8.0/10
2. [DeepSeek 聊天 Demo 实测：接近官方 App，但并非完全复刻](#item-tech-news-2) ⭐️ 8.0/10
3. [美团开源 LongCat-2.5 智能体模型](#item-tech-news-3) ⭐️ 8.0/10
4. [豆包 App 上线对话式地图找店](#item-tech-news-4) ⭐️ 7.0/10
5. [Qwen4-Max-Preview 转向编程与 Agent](#item-tech-news-5) ⭐️ 7.0/10
6. [terminal-mac 为 AI Agent 提供隔离的 Mac 桌面](#item-tech-news-6) ⭐️ 7.0/10
7. [21 家机构拟投 2.7 亿美元布局美元稳定币](#item-tech-news-7) ⭐️ 7.0/10

**AI 创作者雷达**
1. [Claude 设计工作流：减少“AI 味”的五个方法](#item-ai-creator-1) ⭐️ 7.0/10
2. [复古播放器《不卡带》上架 vivo 应用商城](#item-ai-creator-2) ⭐️ 6.0/10
3. [黄仁勋复职联署与微软全球故障](#item-ai-creator-3) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen4-Max 上线：2.4T MoE 与百万上下文](https://qwen.ai/blog?id=qwen4-max) ⭐️ 8.0/10

阿里巴巴发布新一代基座模型 Qwen4，并在千问 AI 平台首发上线 Qwen4-Max；其 API 服务和 Token Plan 已同步支持该模型调用，面向开发者与企业开放。Qwen4-Max 采用基于 Qwen 稀疏注意力（QSA）的新 MoE 架构，总参数量为 2.4T，原生支持视觉和百万 token 上下文；官方称其具备长程任务稳定交付能力。Simon Willison 的演示使用了 none、low、high、xhigh 四档推理强度，但现有材料尚未提供模型速度、价格或基准成绩的独立验证。

hackernews · ilreb · 11月16日 02:14 · [社区讨论](https://news.ycombinator.com/item?id=50513215)

**「架构与推理档位背景」** 理解 Qwen4-Max 的关键是其架构组合：混合专家（MoE）按 token 路由至部分参数，Qwen 稀疏注意力（QSA）则减少长上下文中的注意力计算。社区此前已使用带默认推理档的 Qwen3.8 Max，并将 Qwen4-Max 的 none、low、high、xhigh 四档与之对照；这使调用方可以更显式地权衡推理深度、延迟与成本。

**「选型与接入影响」** Qwen4-Max 已面向开发者和企业通过 API 与 Token Plan 开放；官方称其采用 2.4 万亿参数 MoE 骨干，支持原生视觉和 100 万 token 上下文，可纳入长文档、图像输入及工具调用工作流的评估清单，而 Artificial Analysis 记录的可用上下文为 984k，智能指数为 43 分（同价位可比模型中位数为 41）。接入时应按完整任务成本比较，而不是只看 token 单价：第三方选型汇总指出，token 用量、缓存和计费方式都会影响结果，部分得分更高的竞品每项任务成本反而更低。

**「社区权衡质量、成本与速度」** maplet 援引 Artificial Analysis 称 Qwen4-Max 得分 43、平均成本为 3.27 美元，而“GPT-6.1 Sol \(medium\)”分别为 46 和 0.36 美元；这些数字在所给材料中未经独立核验。seizethecheese 表示，此前 Qwen 3.8 约 30 token/s 的速度拖累了代理编码评测中的投票流程，而排除投票后表现较好，说明实际服务吞吐可能直接影响此类工作流的有效性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen4-max">Qwen4 Max: Intelligence, Performance &amp; Price Analysis</a></li>
<li><a href="https://qwen.ai/blog?id=qwen4-max">Qwen4-Max: Your New Teammate Has Arrived</a></li>
<li><a href="https://kingy.ai/blog/qwen-4-release-date-status/">Qwen4-Max benchmarks, pricing and specs: How it compares</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-coding`, `#agents`, `#models`

---

<a id="item-tech-news-2"></a>
### [DeepSeek 聊天 Demo 实测：接近官方 App，但并非完全复刻](https://www.woshipm.com/ai/6494311.html) ⭐️ 8.0/10

DeepSeek 新开放了可组合的聊天应用 API，并开源 chat-demo，让开发者用自有 Key 搭建接近官方 App 的自托管聊天界面；相关能力覆盖联网搜索、深度思考搜索、链接与文件读取，以及语音合成和识别，可通过 Messages、Responses 或 Chat Completions 三种协议接入。DeepSeek 官方称可用这些接口“1:1 复刻”完整 App，但作者实测发现搜索轮次、工具调用和价格核对仍可能不同：同一道深度搜索题，直接调用 API 时约花费 2.8 分，本次 Demo 则约花费 6.7 分。作者还两次复现到扫描件 PDF 的兼容入口问题：Demo 使用的 /anthropic/v1/files 路径未将图中内容送入模型并误报文件为空，改用 /files 后则能正确识别“8 月、17,900 杯、红色柱”，普通纯文字 PDF 不受影响。

rss · 人人都是产品经理 · 11月16日 03:10

**「官方 App 能力如何拆解为 API」** 此前，DeepSeek 官方网页端主要通过为文件上传和网页搜索分别设计专用提示词来改善体验，而不是依赖一套冗长的通用系统提示词。此次开放新 API 和 chat-demo 的技术背景，是把官方 App 原有的搜索、文件读取、深度思考、语音及安全校验链路拆解为显式请求参数，让开发者能够自行组合这些能力。

**「自建应用的实际注意事项」** 开发者处理扫描件或图片型 PDF 时应优先使用 /files 上传入口；若将 Demo 作为静态站点部署，还应把 API Key 放在后端，否则密钥会暴露在前端。联网搜索按关键词计费，而搜索轮次由模型自行决定，同一任务成本可能相差一倍以上，因此应按实际调用量评估预算；仅用于日常聊天时，继续使用免费的官方 App 更合适。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/langgptai/awesome-deepseek-prompts/blob/main/README.md">awesome- deepseek -prompts/README.md at main...</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#vibecoding`, `#product`, `#api`, `#deepseek`

---

<a id="item-tech-news-3"></a>
### [美团开源 LongCat-2.5 智能体模型](https://www.panewslab.com/zh/articles/01a1def9-753a-76a6-93ee-c7391db07d2b) ⭐️ 8.0/10

美团 LongCat 团队发布 LongCat-2.5 模型权重，并采用 MIT 许可证。该模型采用混合专家（MoE）架构，总参数量为 1.6 万亿，每个 token 激活约 480 亿参数，支持 100 万 token 上下文；美团称模型全程在中国硬件上训练，并同步提供 4-bit 量化权重及基于 194 块华为升腾芯片的自托管指南，未给出英伟达 GPU 方案。美团公布的 Terminal Bench v2.1 得分为 88.4，接近其列出的 Claude Opus 5（89.1）和 GPT-5.6 Sol（88.8）；限时 API 价格约为每百万输入 token 0.27 欧元、输出 token 1.07 欧元。基准成绩来自公司披露，仍需独立验证。

rss · PANews · 11月15日 11:30

**「MoE 与部署背景」** 理解这组参数时，需要区分混合专家（MoE）模型的总参数规模与每个 token 实际激活的参数量：来源给出的 1.6 万亿是前者，而每个 token 约激活 480 亿，后者才更接近单次推理的计算负担。4-bit 量化版本和基于 194 块华为升腾芯片的自托管指南则构成具体的国产硬件部署条件；报道明确称未提供英伟达 GPU 方案。

**「国产算力部署与兼容性」** 对已使用华为升腾算力的企业，LongCat-2.5 的 4-bit 权重和以 194 块升腾芯片为基础的自托管指南提供了可执行的国产硬件部署路径，也带来了百万 token 上下文的测试选项；但报道未提供英伟达 GPU 方案，依赖 CUDA 的现有部署不能直接视为兼容。Terminal Bench v2.1 的 88.4 分属于美团公布数据，采用前仍需在自身代码库和代理任务上复测；API 的每百万输入 token 约 0.27 欧元、输出 token 约 1.07 欧元为限时价格，不宜据此承诺长期成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/models/longcat-2.5">LongCat-2.5: Benchmarks, Pricing &amp; Context Window</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-agents`, `#vibecoding`, `#open-source`, `#ai-hardware`

---

<a id="item-tech-news-4"></a>
### [豆包 App 上线对话式地图找店](https://www.woshipm.com/ai/6494326.html) ⭐️ 7.0/10

豆包 App 已上线“找店”：用户以自然语言提出附近用餐等需求后，系统会筛选匹配商户并批量标注在地图上，显示人均消费、营业状态、评分和团购套餐或代金券。用户可补充人数、用餐时段和预算进行二次筛选，也可主动检索景点、酒店、加油站及休闲娱乐场所，并在豆包内进入商家页购买团购、查看详情或一键发起导航。报道将其视为本地生活入口从独立应用向 AI 对话整合的尝试，但未披露具体上线范围、技术实现、用户规模或交易转化数据，实际效果仍待验证。

rss · 人人都是产品经理 · 11月16日 03:25

**「从出行入口到本地生活」** 此前，豆包已上线“出行用豆包”超级入口，将打车、导航和酒店预订接入助手。此次“找店”在此基础上扩展本地生活场景，把周边商户检索从文字推荐推进到地图标注，并连接团购购买与导航。

**「找店功能压缩本地消费操作链路」** 用户可在豆包内输入人数、预算、正餐或宵夜等条件，由 AI 筛选附近商户并在地图上批量标注，随后比较人均、营业状态和位置，直接购买团购套餐或发起导航，从而省去在地图与团购应用间反复切换、逐店搜索的操作。对抖音系商家而言，这也会增加在豆包内的曝光入口，但来源未提供实际流量或转化数据。

**标签**: `#ai-tools`, `#product`, `#local-commerce`, `#conversational-ai`

---

<a id="item-tech-news-5"></a>
### [Qwen4-Max-Preview 转向编程与 Agent](https://www.woshipm.com/evaluating/6494229.html) ⭐️ 7.0/10

阿里为开发者和办公用户推出仅开放 15 天的 Qwen4-Max-Preview 预览版，通过 Token Plan、千问 App、千问办公和 Qoder 等入口直接承接订阅使用，但没有发布参数规模、技术报告或公开跑分。官方信息称该模型支持文本、图像和视频输入，提供 100 万 Token 上下文窗口，单次最大输出约 39 万 Token。Z Finance 的 12 项实测显示，它在长文档检索、公式型 Excel、可编辑 PPT、多轮修改和代码修复方面表现较稳，修复后的代码包通过了 57 项测试，但仍出现将误差下降过度表述为收敛、漏列一条产品线等错误。相关结论来自单篇二次实测，尚无官方基准或完整技术资料可交叉验证。

rss · 人人都是产品经理 · 11月16日 03:12

**「预览版的产品定位」** Qwen4-Max-Preview 是 Qwen4 序列中的最高档模型，千问官方模型页已将其单独列为支持深度思考的调用模型；开发者资料记录其于 2026 年 11 月 11 日上线，提供 100 万 Token 上下文窗口和约 39 万 Token 的最大输出。此次采用持续 15 天、锁定权重的预览方式，期满后模型下线而订阅关系保留；报道据此将评测重点放在真实任务完成度和订阅工作流，而非公开跑分。

**「采用影响与注意事项」** 对重度编程和 Agent 开发者而言，Qwen4-Max-Preview 的实际价值主要体现在长上下文检索、代码维护和文件交付：本次实测中，它通过了 57 项测试，并能从约 50 万字节工单中串联跨行信息，但生成 PPT 时仍遗漏了一项产品线。计划接入 API 的团队需注意，OpenRouter 条目显示该模型可接收文本、图像和视频、仅返回文本，并提供 100 万 Token 上下文；同时它只是为期 15 天的预览版，各入口的计费和文件输出能力不一，定性结论及最终交付仍需人工复核，不宜将其作为唯一的生产依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qianwenai.com/models/qwen4-max">Qwen 4 - Max - 千 问 AI平台</a></li>
<li><a href="https://oneaiapikey.com/resources/blog/qwen4-max-preview-context-window">Qwen 4 Max Preview Context Window: the 1M- Token Window and...</a></li>
<li><a href="https://openrouter.ai/qwen/qwen4-max">Qwen 4 Max - API Pricing &amp; Providers | OpenRouter</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#agentic-coding`, `#qwen`, `#product`, `#vibecoding`

---

<a id="item-tech-news-6"></a>
### [terminal-mac 为 AI Agent 提供隔离的 Mac 桌面](https://www.woshipm.com/ai/6494316.html) ⭐️ 7.0/10

开源项目 terminal-mac 使用苹果 Virtualization 框架，在 Apple Silicon Mac 上为 AI Agent 创建一台拥有独立桌面、文件系统和账户的 macOS 虚拟机，并将其画面通过 Kitty 或 iTerm2 图形协议嵌入终端。它内置 MCP 服务器，支持截图、点击、拖拽、滚动和键盘输入；Claude Code 可安装插件，Cursor、VS Code、Codex 与 Windsurf 等客户端也可通过 MCP 配置接入。据文章作者实测，安装和 macOS 初始化约需十分钟，但还需手动授予屏幕录制和辅助功能权限，且 App Store 无法在虚拟机中使用。该方案目前仅支持 Apple Silicon；不支持图形协议的终端会回退到独立窗口模式，仍可能影响焦点，虚拟机外层 Agent 的宿主机权限也不会被自动取消。

rss · 人人都是产品经理 · 11月16日 03:12

**「隔离式桌面控制的技术基础」** 让 Agent 操作完整的 macOS 界面，需要的不只是命令执行能力，还包括隔离的客户机桌面、捕获屏幕并注入点击与键盘事件的辅助程序，以及显示客户机画面的传输通道。terminal-mac 的项目说明显示，它通过 Apple Virtualization 运行真实 macOS 客户机，由客户机内的辅助程序采集画面并发送输入事件，再通过 Kitty 或 iTerm2 图形协议呈现在终端中；该项目目前仍标为面向 Apple Silicon 的早期候选版本，因此应按预发布工具理解其成熟度。

**「实际影响与使用条件」** 对使用 Apple Silicon Mac 的开发者，terminal-mac 让 Agent 能通过 MCP 执行截图、点击、拖拽、滚动和键盘输入，在独立的 macOS 虚拟机中操作桌面应用，从而减少误改宿主电脑文件、剪贴板或当前焦点的风险，可用于桌面应用测试和 GUI 回归自动化。团队采用前需确认兼容性：该项目暂不支持 Windows；若要在终端内观察且避免独立窗口切换影响焦点，应使用 Kitty、iTerm2 或 Ghostty 等支持图形协议的终端，否则会回退到窗口模式。此外，虚拟机内无法使用 App Store，外层 Agent 原有的宿主权限仍需单独限制，不能因启用虚拟机就视为已完成安全隔离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/govijr/terminal-mac">GitHub - govijr/terminal-mac: Entire MacOS running in your ...</a></li>
<li><a href="https://github.com/govijr/terminal-mac">GitHub - govijr / terminal - mac : Entire MacOS running in your terminal.</a></li>
<li><a href="https://gitnova.dev/en/r/govijr/terminal-mac">govijr / terminal - mac — what it is and what it’s for | GitNova</a></li>

</ul>
</details>

**标签**: `#ai-tools`, `#ai-agents`, `#vibecoding`, `#developer-tools`, `#macos`

---

<a id="item-tech-news-7"></a>
### [21 家机构拟投 2.7 亿美元布局美元稳定币](https://www.panewslab.com/zh/articles/01a1dff9-1212-7390-b479-43499460d8eb) ⭐️ 7.0/10

高盛、花旗、桑坦德、德意志银行等 21 家机构组成的联盟承诺投入约 2.7 亿美元，用于代号“Project Faro”的美元稳定币项目未来五年运营。发行方计划在美国注册，项目目标于 2027 年上线，拟与 Tether 和 Circle 竞争。该项目目前尚无最终名称、CEO 或代币，因此仍属于筹资与筹备计划，而非已经发行的稳定币。

rss · PANews · 11月15日 16:10

**「现有市场由两家主导」** 稳定币是锚定美元等资产的代币，可用于转账和支付结算。据该报道援引的数据，Tether 与 Circle 合计约占 2900 亿美元稳定币市场的 85%。

**「暂时无法接入或部署」** 金融机构目前只能将 Faro 视为一项未来发行计划，不能把约 2.7 亿美元承诺视为已有资产或可用支付渠道；实际注册、治理团队确定、代币发行及 2027 年上线仍待落实。

**标签**: `#web3`, `#stablecoins`, `#payments`, `#institutional-adoption`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [Claude 设计工作流：减少“AI 味”的五个方法](https://creatoreconomy.so/p/how-to-fix-ai-slop-with-claude-design-nate-parrott) ⭐️ 7.0/10

节目介绍了一期对 Anthropic 设计师 Nate Parrott 的访谈，主题是借助 Claude 设计功能、交互式仪表盘和动态视频。材料列出的演示包括把手机便签中的 Duet 功能想法做成原型、把电子表格转成动态仪表盘，再将仪表盘转为 Claude Motion 视频；文中还摘录了五项减少“AI 味”的方法，包括预先提供上下文、研究成熟 UX 模式、记录并约束模型设计偏好、先做线框，以及生成多个方案后重新组合。现有材料主要是节目导览和经验总结，未提供完整对话、前后效果对照或独立验证，适合使用 Claude 进行产品原型和视觉设计的创作者参考，而非视为一次重大产品更新。

rss · Creator Economy So · 11月15日 14:05

**「整理可复用的去模板化方法」** 可做角度：把五项建议整理成一份“Claude 设计去模板味”实操清单，沿手机便签原型、表格转仪表盘、线框迭代和多方案混搭三个步骤展开，并明确这些是访谈中的工作方法，而非已经验证的通用效果。

**标签**: `#creator`, `#ai-tools`, `#design`, `#workflow`, `#anthropic`

---

<a id="item-ai-creator-2"></a>
### [复古播放器《不卡带》上架 vivo 应用商城](https://sspai.com/post/119012) ⭐️ 6.0/10

作者西鸽用 Antigravity 起步、后转由 Codex 接手，开发了本地媒体播放器《不卡带》，并于 2026 年 11 月 16 日在 vivo 应用商城上架。文章称，项目始于 10 月 20 日，AI 可快速完成约 80% 的初始功能需求，但后续增加功能、适配多款折叠屏和打磨 UI 细节会迅速消耗模型额度。应用支持音视频播放、WebDAV 接入 NAS、EQ、WinAMP 皮肤与自制主题导入，以及多种复古设备噪声滤镜；作者同时注明，滤镜听感带有个人想象、皮肤适配未经充分测试，版本更新也较慢。

rss · 少数派 · 11月16日 02:52

**「为什么值得关注」** 截至文章发布，《不卡带》已从 AI 快速原型进入应用商店和真实设备试用阶段，也具体展示了快速生成功能之后仍需投入适配、测试与界面打磨。不过，这只是单个独立开发者的经验，不能据此判断 AI 编程工具或行业效率已经发生普遍变化。

**「内容切入」** 可做角度：以《不卡带》从 Antigravity 切换到 Codex、继续适配多款折叠屏为例，梳理 AI 辅助开发中“快速做出原型”与“反复打磨、适配和测试”之间的落差，并明确这是单一项目经验。

**标签**: `#ai-tools`, `#indie-apps`, `#product-design`, `#creator`

---

<a id="item-ai-creator-3"></a>
### [黄仁勋复职联署与微软全球故障](https://sspai.com/post/119119) ⭐️ 6.0/10

这期早报以黄仁勋去留和 Microsoft 365 全球故障为主，并收录模型取证、航班停飞、流媒体调查、Cybercab 协议及苹果新品传闻等简讯。据文中转引 Business Insider，公开信 Stand with Jensen 截至 11 月 14 日下午已有逾 10.8 万个签名，其中包括逾 5.8 万名股东和 5600 多名现员工，主办方正清理其中的虚假签名；《金融时报》称黄仁勋正与亲信探讨重返公司，但所给材料没有复职已获确认的官方信息。Microsoft 365 因近期升级引入的技术问题，自 11 月 12 日中午起在 70 多个国家和地区影响 Outlook、Teams、Copilot 等约 20 项服务，约 19 小时后于 11 月 14 日全面恢复，微软称已排除网络攻击或 AI 智能体因素。其他条目多依赖媒体、研究机构或公司协议文本，适合作为仍待核实的行业观察素材。

rss · 少数派 · 11月15日 23:24

**「为何值得关注」** 联署已达到逾 10.8 万个签名，而黄仁勋是否回归仍处于讨论阶段；前者是已经发生的规模变化，后者尚未得到确认。Microsoft 365 故障对政务、医疗、司法和企业办公的影响已经发生并已恢复，分析师所称长期可能促使企业考虑替代方案，则仍不是确定结果。

**「内容切入」** 可做角度：用“逾 5.8 万名股东、5600 多名现员工参与联署”观察英伟达在黄仁勋离任后的治理压力，重点讲清员工与股东公开施压和董事会是否行动之间的差别，不把媒体所称的复职探讨写成既定结果。

**标签**: `#ai-tools`, `#NVIDIA`, `#Microsoft-365`, `#Copilot`, `#service-outage`

---