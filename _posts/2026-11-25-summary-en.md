---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 199 items, 15 important content pieces were selected

---

**Technology News**
1. [DeepSeek Super-agent Adds Router–Worker Coordination for Multi-Channel Agents](#item-tech-news-1) ⭐️ 8.0/10
2. [Claude Artifacts Gain Desktop App Installation Beta](#item-tech-news-2) ⭐️ 8.0/10
3. [GPT-6.2 generates code-driven 3D minibinder designs](#item-tech-news-3) ⭐️ 7.0/10
4. [Ternary Bonsai 2.5 targets efficient local agentic coding](#item-tech-news-4) ⭐️ 7.0/10
5. [ByteDance launches Xiaodou personal-agent app in invite-only beta](#item-tech-news-5) ⭐️ 7.0/10
6. [Sand.ai launches MAGI-2 with low per-second video pricing](#item-tech-news-6) ⭐️ 7.0/10
7. [GPT-6.2 Astra Leads Benchmarks but Struggles with Reliable Delivery](#item-tech-news-7) ⭐️ 7.0/10
8. [Ledn launches U.S. multi-asset custody account](#item-tech-news-8) ⭐️ 7.0/10
9. [Neuberger Berman Launches HINC on Aave Horizon](#item-tech-news-9) ⭐️ 7.0/10
10. [Jensen Huang Resigns From Nvidia and Returns After 11 Days](#item-tech-news-10) ⭐️ 7.0/10

**Technology Blog**
1. [The Fear Trade](#item-tech-blog-1) ⭐️ 8.0/10
2. [Aave Horizon Adds HINC High-Yield Collateral](#item-tech-blog-2) ⭐️ 8.0/10
3. [Three LLM Inflection Points in Twelve Months](#item-tech-blog-3) ⭐️ 6.0/10
4. [Astra and an Anonymous 1808 Sketchbook](#item-tech-blog-4) ⭐️ 6.0/10
5. [Neon’s Uptake Signals Google DeepMind’s Frontier Return](#item-tech-blog-5) ⭐️ 5.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek Super-agent Adds Router–Worker Coordination for Multi-Channel Agents](https://www.woshipm.com/ai/6500050.html) ⭐️ 8.0/10

The DeepSeek Harness team open-sourced DSH Super-agent in late October as a prototype for coordinating always-on agents across channels such as Feishu, DingTalk, GitHub, email, and document systems. Its two-tier architecture uses a resident Router to classify inbound events and coordinate work, while isolated Workers execute tasks, bind their sessions to the originating channel for accurate result delivery, and can create their own Sub-Agents for parallel work. The prototype combines code-based Fast Path filtering with model-based Slow Path analysis and asynchronous Worker execution so users can interact while long-running tasks continue. The code and technical design are available, but Super-agent remains a prototype that is disabled in DeepSeek Harness by default, and the supplied account is a secondary architectural analysis rather than an independent performance evaluation.

rss · 人人都是产品经理 · Nov 25, 03:22

**「Architectural Context」** Super-agent builds on DeepSeek Harness, which the DeepSeek Harness team describes as the foundation for its approach to Agent development. Its structure also responds to existing Multi-Agent and Agent Team patterns: Multi-Agent commonly uses direct hand-offs, while an Agent Team orchestrator may both plan and execute work; Super-agent instead keeps a persistent Router focused on coordination and assigns execution to Workers with isolated contexts.

**「Practical impact」** For developers building agents across IM, GitHub, email, and other asynchronous channels, Super-agent’s Router/Worker split provides a concrete implementation pattern: route incoming events through a persistent Router, isolate execution in Worker sessions, bind each session to its originating thread or pull request, and run long tasks asynchronously so the agent can continue accepting messages. The limitation is equally concrete: DSH Super-agent remains a research prototype and is not enabled in DeepSeek Harness’s default configuration, so teams should validate their channel adapters, permissions, and result-routing behavior rather than assume it is a supported, drop-in production service.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseekv4pro.com/guides/deepseek-superagent-adoption">DeepSeek Super - agent : GitHub Adoption Guide</a></li>
<li><a href="https://www.mindstudio.ai/blog/deepseek-super-agent-harness-design">DeepSeek &#x27;s Super Agent Harness : Fixing the Attention... | MindStudio</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#agents`, `#product`, `#tech`

---

<a id="item-tech-news-2"></a>
### [Claude Artifacts Gain Desktop App Installation Beta](https://www.panewslab.com/zh/articles/01a2100a-3d06-72bb-9933-84ddfa3bd742) ⭐️ 8.0/10

Anthropic announced a beta of Claude’s “Install as app” feature, allowing users to install AI-generated Artifacts as standalone Mac or Windows applications without manually packaging, signing, or obtaining a separate API key. Installed apps can call Claude models and connected external services, update when the underlying Artifact changes, and integrate with the desktop through notifications, menu bar or tray icons, global shortcuts, and always-on-top windows. The beta is gradually rolling out to all Claude plans, with default, app-specific, and full-computer-access permission levels; permissions apply only to the current app version and must be renewed after updates.

rss · PANews · Nov 25, 00:10

**「Claude and Artifacts」** Claude, Anthropic’s AI assistant, was released as a chatbot in March 2023 and is also used for AI-assisted software development. The reported update builds on Claude’s Artifacts—interactive creations generated in the assistant—by adding a way to deliver those creations as Mac or Windows desktop applications.

**「Impact」** Users can deliver interactive Artifacts as installable desktop applications with less setup work, but full-computer access permits those apps to run programs and read, modify, or delete local files. Because permissions expire with each app version, users should review an Artifact and its requested access before installation and again whenever an update triggers renewed authorization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#claude`, `#desktop-apps`, `#product`, `#ai-agents`

---

<a id="item-tech-news-3"></a>
### [GPT-6.2 generates code-driven 3D minibinder designs](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 7.0/10

OpenAI reports that GPT-6.2 was given the three-dimensional structures of five target proteins and specified minibinder attachment sites, then wrote code that proposed 3D minibinder designs without using specialized protein-design models. The workflow was not fully autonomous: OpenAI used SolubleMPNN to suggest amino-acid sequences and other specialized models to select candidates predicted to fold as designed and bind at the intended site. The five-protein demonstration therefore shows GPT-6.2 orchestrating part of a protein-design pipeline, but not replacing specialist models or independently validating the resulting proteins.

hackernews · OpenAI News · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**「How the protein-design workflow was divided」** Protein design can separate creation of a three-dimensional geometry from supplying the amino-acid sequence that will fold into that geometry. In this test, GPT‑6.2 generated code for the geometric minibinder designs, while specialist models such as SolubleMPNN proposed sequences and other protein models checked predicted folding and target binding.

**「Effect on protein-design workflows」** OpenAI reports that GPT-6.2 can serve as the code-writing and three-dimensional design stage of a minibinder workflow, with lab tests finding evidence of binding across five target proteins. The practical constraint is that this does not remove specialist-model stages: SolubleMPNN was still used to generate sequences that fold into the proposed structures, and other protein models were used to select and validate candidates, so researchers must keep those tools in the loop rather than treat GPT-6.2 as an end-to-end replacement.

**「Community discussion」** Commenters disagreed over what GPT-6.2 actually designed: gopalv emphasized the model’s ability to advance tasks through code, while fabian2k questioned whether producing geometry counts as protein design when specialist models supply the sequences. plaidfuji described GPT-6.2 as a useful “glue layer” between specialized tools, and joe-esquibel said the presented evidence appeared more computational than laboratory-controlled.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/">GPT - 6 models demonstrate intrinsic protein - design ... | OpenAI</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#engineering`, `#ai-research`

---

<a id="item-tech-news-4"></a>
### [Ternary Bonsai 2.5 targets efficient local agentic coding](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 7.0/10

Ternary Bonsai 2.5 27B is a ternary-quantized model designed for efficient local inference, including agentic coding workloads. Early users testing its Q2 GGUF build report roughly 22–25 tokens per second on a 24GB Mac Mini M5 Pro and say a 128K context fits in memory. Claims of SWE-bench Verified parity and improved agentic performance remain anecdotal, and the supplied announcement does not provide enough benchmark methodology to establish broader results.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**「Ternary model basics」** Ternary computing represents values with three states; balanced ternary uses −1, 0, and +1, allowing subtraction through digit inversion and ordinary addition. Applied to a 27B-parameter language model, this three-value weight representation is the basis of Bonsai 2.5’s efficiency-focused local-inference pitch: the parameter count remains high while the representation is designed to reduce storage and computation requirements.

**「Effect on local coding agents」** Bonsai 2.5 27B gives local-agent developers a more practical iteration target: PrismML reports improvements in agentic execution, coding, and multi-turn tool use over Bonsai 2, while retaining the same ternary format, storage accounting, and rotated weight basis, reducing format-migration concerns for existing Bonsai 2 deployments. Early tests are encouraging rather than conclusive—one tester reports 22.3 tokens per second and 128k context fitting on a 24-GB M5 Pro, while another reports unchanged pass rates but a 29% reduction in completion time—so teams should benchmark their own tool-use workloads and memory budgets before relying on vendor benchmark claims.

**「Early community results」** Testers offer mixed evidence beyond throughput: one reports 17% fewer steps and 29% less completion time than Bonsai 2 on a personal eight-task benchmark, while another says the displayed scores appear worse than Qwen and asks whether memory use and speed are the real advantage. A commenter also asserts SWE-bench Verified parity with Opus 4.6, but the supplied material does not substantiate that claim.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ternary_computer">Ternary computer - Wikipedia</a></li>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic Coding and...</a></li>
<li><a href="https://huggingface.co/prism-ml/Ternary-Bonsai-2.5-27B-GGUF">prism-ml/ Ternary - Bonsai - 2 . 5 - 27 B -GGUF · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding-agents`, `#local-models`, `#model-efficiency`

---

<a id="item-tech-news-5"></a>
### [ByteDance launches Xiaodou personal-agent app in invite-only beta](https://www.woshipm.com/ai/6500095.html) ⭐️ 7.0/10

ByteDance began an invitation-only public beta on November 24 of Xiaodou, a standalone iOS and Android personal-agent app that shares accounts, memory, and subscription benefits with Doubao while adding proactive follow-up and background task execution. According to the report, the beta provides a task-management view and up to 10 scheduled tasks, connectors for services including Douyin, Feishu, Calendar, and Apple Health, and AI-initiated calls for restaurant, hotel, and store enquiries; the cited examples come from ByteDance demonstrations and media testing rather than independent benchmarks. Call handling is currently limited to those everyday service scenarios and excludes overseas and private numbers. Users currently require an invitation code, Xiaodou has no web app or desktop chat interface, and ByteDance has not announced general availability, although it says the capabilities will eventually be integrated into the main Doubao app.

rss · 人人都是产品经理 · Nov 25, 07:11

**「Product context」** Personal Agents differ from conventional prompt-and-response assistants by retaining long-term context, monitoring ongoing matters, and executing tasks proactively in the background. The article places Xiaodou after earlier domestic efforts such as Ant&\#x27;s Lingguang, Alibaba&\#x27;s Qwen Go, and Tencent&\#x27;s Xiaowei, positioning it as a standalone interface that reuses Doubao&\#x27;s account, memory, and membership allowance.

**「Practical impact for users」** Users cannot treat 小豆 as a broadly available replacement for 豆包: as of November 24, it was an invite-only public beta with no desktop or web version, a 10-task limit for scheduled jobs, and outbound calling restricted to restaurant, hotel, and store scenarios rather than overseas or private numbers. Existing 豆包 users should expect limited functionality until more invitation quotas are released and its capabilities are gradually integrated into 豆包; PC users could view 小豆 conversations in 豆包 but could not yet converse with it there.

**Tags**: `#ai-tools`, `#ai-agents`, `#product`, `#tech`

---

<a id="item-tech-news-6"></a>
### [Sand.ai launches MAGI-2 with low per-second video pricing](https://www.woshipm.com/ai/6500084.html) ⭐️ 7.0/10

Sand.ai has launched MAGI-2, a video-generation model that produces clips up to 30 seconds long at 1080p for an official list price of CNY 0.5 per second—CNY 15 for a 30-second video—with the source claiming this is about one-tenth of Seedance 2.5’s price for equivalent specifications. The model uses Sand.ai’s MagiMoE architecture, accepts prompts of roughly 20,000 characters and up to 20 multimodal references comprising 10 images, five videos and five audio files, and supports native audiovisual generation, although its audio-reference capability reportedly still needs improvement. Individual users can currently access it exclusively through LibTV, while Sand.ai says it plans to open the model weights subject to applicable legal and compliance requirements, without announcing a release schedule or implementation plan. The article presents prompts for difficult tests involving style changes, action continuity, dialogue and lip synchronization, but the supplied text provides no reproducible output measurements to establish those capabilities, leaving the pricing comparison and complex-shot stability claims unverified.

rss · 人人都是产品经理 · Nov 25, 07:07

**「From MAGI-2 Preview to MAGI-2」** MAGI-2 builds on MAGI-2 Preview, which Sand.ai released and open-sourced on August 5, 2026, according to a DeepTech report published on Tencent the following day. Sand.ai describes the full model as a 480B-scale video generator using finer-grained MagiMoE expert specialization, targeted post-training, and 1080p upscaling; unlike the Preview’s published weights, a full-model weight release remains a future plan without a specified timetable.

**「Lower trial costs, production caveats」** At MAGI-2’s stated 1080p list price of RMB 0.5 per second, a creator can request ten 30-second clips for RMB 150 in listed generation charges, reducing the cost of prompt-and-reference iteration. Production teams should benchmark those renders for character and action consistency, lip sync, and audio-reference quality before switching: the article excerpt provides no measured stability results, notes limitations in audio referencing, and says consumer access is currently exclusive to LibTV, while open weights remain a compliance-conditional plan with no timetable. Seedance 2.5 is also built for 30-second audio-video generation and reference control, so comparisons should use equivalent briefs rather than clip duration alone.

<details><summary>References</summary>
<ul>
<li><a href="https://sand.ai/blog/magi-2/">MAGI - 2 : A 480B Frontier Video Generation Model</a></li>
<li><a href="https://news.qq.com/rain/a/20260806A061ZB00">10 秒 1080 P 视频只要五毛钱： Sand . ai 开源首个千亿MoE...</a></li>
<li><a href="https://seed.bytedance.com/en/seedance2_5">Seedance 2 . 5</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#generative-video`, `#creator`, `#product`

---

<a id="item-tech-news-7"></a>
### [GPT-6.2 Astra Leads Benchmarks but Struggles with Reliable Delivery](https://www.woshipm.com/ai/6499923.html) ⭐️ 7.0/10

The article reports that GPT-6.2 Astra posted higher agent and specialist-task benchmark scores—5.2 points above its predecessor and 5.5 points above Claude Fable 5.2 on Agents’ Last Exam—while the cited evaluation put one task at about $3 versus $60. Developer reports nevertheless describe poor long-task usability: in an 11-day Rust compiler optimization, the first seven days reportedly reduced compilation speed by 56%, and after the objective was clarified, the final four days produced no effective code changes. For coding-agent teams, the practical lesson is to separate capability from delivery reliability by enforcing fixed goals, per-round benchmarks, obstacle reporting, budgets, and automatic stops after repeated failures or no improvement; the article also cites 22.28% obstacle underreporting and 22% fewer output tokens. These figures are secondary-source claims, and the supplied material does not include the original release or reproducible evidence.

rss · 人人都是产品经理 · Nov 25, 03:07

**「Context」** Agent benchmarks generally measure capability on bounded tasks, while production coding agents must also preserve goals across long sessions, recover from tool failures, report blockers, and stop safely; this distinction separates Astra’s benchmark performance from its delivery reliability. GPT-6.2 Astra continues the GPT-6 Astra line: Artificial Analysis listed its API pricing at $8/$40 per million tokens, 20% below its predecessor, with cached input reduced from $1.00 to $0.40 per million tokens, providing context for the debate over token savings versus total task cost.

**「Require external controls for agent delivery」** For teams piloting GPT-6.2 Astra, the article’s reported 22.28% obstacle-omission rate and a Rust-compiler run whose first seven days slowed compilation by 56% mean that benchmark gains alone are insufficient for production acceptance. Agent workflows should preserve baselines and rollback points, validate measurable metrics after each change, log commands, tool results, and skipped or inaccessible resources, and stop when progress stalls or time, cost, and permission limits are reached. Although Astra reportedly emits 22% fewer tokens than its predecessor, deployments should include retries, debugging, manual verification, and failed side effects in total cost; otherwise apparent token savings may simply shift work back to human reviewers.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/openai-has-the-2-model-in-the-intelligence-index-with-the-release-of-gpt-6-2-astra-and-gpt-6-2-sol">OpenAI has the #2 model in the Intelligence Index... | Artificial Analysis</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#ai-agents`, `#engineering`

---

<a id="item-tech-news-8"></a>
### [Ledn launches U.S. multi-asset custody account](https://www.theblock.co/news/business/2026-11-24-ledn-launches-us-custody-account-bitcoin-gold-stablecoins-lending-445411) ⭐️ 7.0/10

Ledn has launched a U.S. custody account that lets eligible customers hold bitcoin, gold, stablecoins, and dollars, swap among them without trading fees, and borrow against bitcoin without selling it. Assets are held by an independent qualified custodian and segregated from Ledn’s own assets, while bitcoin purchases carry a 0.50% spread. The launch moves Ledn’s U.S. business onshore and expands its lending coverage to additional states, a market of roughly 55 million people. Detailed eligibility, rollout timing, collateral requirements, liquidation terms, and other risk conditions were not provided, leaving important constraints unclear.

rss · The Block · Nov 24, 14:00

**「Bitcoin-backed lending」** Ledn’s underlying product is a bitcoin-backed loan that provides USD liquidity without requiring borrowers to sell their BTC; the company also describes holding or trading bitcoin, gold, and supported stablecoins. The U.S. account packages that collateralized-borrowing model with domestic custody and fee-free swaps, extending an existing Ledn workflow rather than introducing a fundamentally new lending mechanism.

**「Practical impact」** Eligible U.S. customers can now obtain USD-denominated liquidity without selling bitcoin by using it as loan collateral, while an independent qualified custodian holds the account assets separately from Ledn’s own holdings. Borrowing is bitcoin-only, and the economics are material: Ledn lists rates starting at 11.9% APR and falling to 9.25% for loans of $2 million or more, while bitcoin purchases carry a 0.50% spread; customers should confirm state eligibility and compare these costs before relying on the account.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ledn.io/">Ledn | Borrow Against your Bitcoin Securely</a></li>
<li><a href="https://www.ledn.io/bitcoin-backed-loans">Bitcoin - backed Loans from 9.25% APR | Borrow USD Today without...</a></li>
<li><a href="https://www.ledn.io/">Ledn | Borrow Against your Bitcoin Securely</a></li>

</ul>
</details>

**Tags**: `#web3`, `#product`, `#bitcoin`, `#lending`

---

<a id="item-tech-news-9"></a>
### [Neuberger Berman Launches HINC on Aave Horizon](https://www.theblock.co/news/markets/2026-11-24-neuberger-berman-tokenized-hinc-fund-aave-horizon-collateral-445391) ⭐️ 7.0/10

Neuberger Berman and Securitize launched the tokenized HINC high-yield credit fund on Aave Horizon, according to Securitize. Eligible investors can use HINC as collateral to borrow USDC, GHO, or RLUSD, with the fund providing exposure to actively managed high-yield credit; the announcement did not specify eligibility requirements, borrowing terms, or adoption figures.

rss · The Block · Nov 24, 14:00

**「From proposal to launch」** Before the launch, Aave governance was considering HINC as supply-only collateral on Horizon, with USDC, GHO, and RLUSD intended to be borrowable against it. The proposal required technical and risk reviews, oracle work, and pre-onboarded liquidators before activation.

**「Impact」** Eligible investors can now use HINC as collateral on Aave Horizon to borrow USDC, GHO, or RLUSD, giving institutional borrowers a tokenized high-yield credit asset to secure loans. Aave generally requires collateral to exceed the borrowed amount, so investors must verify HINC’s eligibility and collateral parameters before transacting; the announcement does not disclose those terms.

<details><summary>References</summary>
<ul>
<li><a href="https://bingx.com/en/flash-news/post/aave-governance-proposal-would-add-neuberger-berman-s-tokenized-high-income-fund-hinc-as-supply-only-collateral-on-aave-horizon">Aave Horizon Set to List Neuberger Berman &#x27;s Tokenized...</a></li>
<li><a href="https://www.assettokenization.com/intelligence/assets/6615/gho-gho">GHO | Tokenized Asset | Tokenization Intelligence</a></li>
<li><a href="https://aave.com/">Aave — Onchain Savings, Lending and Borrowing</a></li>

</ul>
</details>

**Tags**: `#web3`, `#defi`, `#tokenized-rwa`, `#institutional-finance`

---

<a id="item-tech-news-10"></a>
### [Jensen Huang Resigns From Nvidia and Returns After 11 Days](http://www.geekpark.net/news/374431) ⭐️ 7.0/10

According to GeekPark, Nvidia founder Jensen Huang resigned as CEO, president, and director on November 12, 2026, following allegations of two extramarital affairs. The board initially accepted his resignation, rejected any immediate return, and engaged Heidrick &amp; Struggles to seek a successor, but unanimously restored all three positions on November 23 after 11 days of employee, customer, investor, and market pressure. GeekPark reports that Nvidia shares fell about 28% over seven trading sessions, losing roughly $1.16 trillion in market value, before rising 31.48% on the reinstatement day and adding about $954.4 billion. The supplied article does not include the complete primary-source record for these events, and it says an independent investigation into Huang’s conduct continued after his reinstatement.

rss · 极客公园 · Nov 24, 09:58

**「The leadership reversal」** Nvidia had officially announced Jensen Huang’s immediate resignation as president, CEO and director on Nov. 12, with CFO Colette Kress becoming interim CEO. The Nov. 23 unanimous vote restoring Huang to all three positions therefore reversed the board’s earlier decision rather than completing a planned leadership transition.

**「Investors face extreme event-gap risk」** After Huang’s reported reinstatement, Nvidia rose 31.48% in one session, adding roughly $954.4 billion in market value, while GraniteShares’ three-times-short Nvidia ETP fell 92% and Leverage Shares’ NV3S fell 80% \[tool-3-1\]. For investors in leveraged inverse Nvidia products, the episode demonstrates acute event-gap risk: a sudden leadership announcement can erase most of a position’s value even when its longer-term bearish thesis remains unchanged.

<details><summary>References</summary>
<ul>
<li><a href="https://ludepress.com/news/zhongbang/75684/">ludepress.com/news/zhongbang/75684</a></li>
<li><a href="https://www.guancha.cn/CaiJing/2026_11_24_909741.shtml">英 伟 达 惊人反转：有人浮盈近9000%，有人做空巨亏92%</a></li>
<li><a href="https://www.guancha.cn/CaiJing/2026_11_24_909741.shtml">英 伟 达 惊 人 反转：有 人 浮盈近9000%，有 人 做空巨亏92%</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-infrastructure`, `#nvidia`, `#leadership`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [The Fear Trade](https://www.bankless.com/read/the-fear-trade) ⭐️ 8.0/10

rss · Bankless · Nov 24, 20:47

**「Background」** The author describes a “fear trade” in which distrust of AI intermediaries appears to lift demand for Venice’s VVV token: VVV rose roughly 30% around the latest disclosures and 40% after an earlier Codex scare, though the causal link is the author’s belief. The focus has shifted to hosting providers and routers, where developers may be unable to verify prompt retention or which model answers.

**「Solution」** Dragos planted canaries in about two million prompts and found attackers copying requests inside three providers, including prompts marked never to be stored; OpenRouter then dropped three providers and removed the zero-retention label from 125 endpoints. Separately, Prime Intellect said an intruder served a doctored “abliterated” DeepSeek V4.1 Flash for more than two days, with benchmark-like performance making the substitution hard to detect. Venice’s strictest encrypted mode encrypts prompts on-device, decrypts them only in sealed hardware, and lets clients check attestations, while private models run on Venice-controlled GPUs or contract-bound partner infrastructure. The author stresses the limits: Venice does not claim attestations prove the exact loaded weights, its default zero-retention mode remains contractual, Claude and GPT sessions are anonymized rather than private, and partner Phala exposed production DeepSeek traffic without required controls while nobody checked its attestation before launch. The proposed endpoint is verifiable inference—cryptographic proof of model identity and stronger data-handling guarantees—especially as open-weight models rose from 7% to 56% of tokens on Vercel’s gateway; sealed hardware works today, but Anthropic’s model-proof prototype requires 70–95 times conventional GPU time.

**「Takeaway」** The article argues that AI infrastructure must move from contractual assurances toward independently checked cryptographic proof, although today the market is buying the promise it distrusts least.

**Tags**: `#ai-tools`, `#web3`, `#product`, `#security`, `#ai-infrastructure`

---

<a id="item-tech-blog-2"></a>
### [Aave Horizon Adds HINC High-Yield Collateral](https://www.bankless.com/read/news/aave-horizon-adds-neubergers-high-yield-hinc-fund-as-collateral) ⭐️ 8.0/10

rss · Bankless · Nov 24, 20:43

**「Background」** Aave Horizon, Aave’s permissioned market for tokenized real-world assets, had mostly accepted tokenized Treasury bills and highly rated credit, with yields close to stablecoin borrow rates, so borrowing was mainly a liquidity move. The listing proposal calls Neuberger and Securitize’s tokenized HINC fund Horizon’s first sub-investment-grade collateral, introducing a carry opportunity alongside unfamiliar credit and liquidation risks.

**「Solution」** HINC’s holdings were roughly 87% high-yield corporate bonds, 8% BB-rated CLO tranches, and cash, with 12–20% rated CCC or below depending on the agency in LlamaRisk’s review; eligible HINC holders can borrow USDC, RLUSD, or GHO. Horizon assigns HINC a 55% LTV, 67% liquidation threshold, 8% liquidation bonus, and a 10,000-HINC \(about $10M\) cap, compared with 88% LTV for tokenized T-bills; a dedicated GHO E-Mode permits borrowing up to 57% LTV. By Tuesday, roughly 6,160 HINC \(about $6M, 62% of the cap\) had been supplied, and the onchain oracle valued it at $977.27 against its $1,000 issue price. Only pre-approved HINC holders can liquidate positions, and they must then redeem through the fund, targeting T+1 settlement but potentially taking longer without an instant-redemption buffer; at maximum LTV, a 17.9% HINC fall reaches liquidation, slightly below the proposal’s illustrative index blend’s 18.25% one-month drop in March 2020. The author’s central warning is that this creates a real carry trade while permissionless stablecoin lenders indirectly back credit they cannot hold or liquidate themselves; the $10M cap limits exposure for now, but the first credit selloff will test the approved-holder liquidation model.

**「Takeaway」** Adding HINC moves Horizon from relatively safe, liquid collateral toward sub-investment-grade yield, making liquidation access and redemption timing the decisive questions for protecting lenders.

**Tags**: `#web3`, `#defi`, `#tokenized-rwa`, `#protocol-risk`, `#product`

---

<a id="item-tech-blog-3"></a>
### [Three LLM Inflection Points in Twelve Months](https://simonwillison.net/2026/Nov/24/llm-inflection-points/) ⭐️ 6.0/10

rss · Simon Willison · Nov 24, 23:02

**「Background」** Simon Willison argues that frontier models and coding agents passed three meaningful capability thresholds in twelve months: dependable daily coding, proactive tool use, and support for complete interactive projects. His account is a personal field report rather than a standardized benchmark.

**「Solution」** First, in November 2025, reliability crossed a practical threshold: Willison says Opus 4.5 was the first Claude Code model whose default result was generally right, while GPT-5.1 variants made Codex similarly dependable for many tasks. Second, June and July’s “Fable class” models were relentlessly proactive: Fable created a pyobjc-Quartz screenshot mechanism and CORS logging server to diagnose a Safari glitch, and Fable 5.2 used five microphones to locate a beep within about 40 cm. Willison’s mechanism here is simple: give an agent a goal and the right tools, then let it build investigative aids and iterate rather than merely return code. Third, by September and October, models had become strong at Blender and Three.js 3D work and complete games; most strikingly, Opus 5.5 spent 12 hours playtesting and rebalancing a dull Command &amp; Conquer-style RTS until it was deeply entertaining. He is less certain whether Fable 5.2 constitutes a fourth inflection point, but reports a rapid release cadence across Datasette and LLM and says clearly described software can now often be built.

**「Takeaway」** Willison’s larger claim is that software development has shifted from typing code toward directing agents that can investigate, test, and refine their own work, making human goal-setting and taste more important. Because his evidence is experiential rather than benchmarked, the boundaries—and especially the possible fourth inflection point—remain provisional.

**Tags**: `#ai-tools`, `#vibecoding`, `#coding-agents`, `#game-development`

---

<a id="item-tech-blog-4"></a>
### [Astra and an Anonymous 1808 Sketchbook](https://simonwillison.net/2026/Nov/24/astra-historical-mystery/) ⭐️ 6.0/10

rss · Simon Willison · Nov 24, 16:53

**「Background」** Identifying the creator of an anonymous historical document can require connecting scattered diaries, travel accounts, archival catalogs, and contextual evidence. Simon Willison relays a case study from history professor Mark Humphries in which an AI agent is said to have conducted that kind of source investigation autonomously.

**「Solution」** According to the account, GPT-6.2 Astra was given only minimal prompting and reportedly identified the creator of an anonymous 1808 sketchbook at Yale’s Beinecke Library in 22 minutes by searching publicly available primary and secondary sources. Its decisive lead was a diary reference to a visit by the vicomte de Chabot five days before a date mentioned in the sketchbook near a river; Astra predicted that Chabot’s travel journal, obtainable by order from Cleveland State University, would confirm the attribution, and the journal did. The source itself was also described as a major find for Canadian and fur-trade historians. Humphries compares the disruption to mathematics facing systems that can solve problems beyond human ability, but argues that historians continually reinterpret the past rather than pursue a single universal truth, leaving an essential role for human interpretation. As presented here, however, the case is a secondhand account without the prompt, tool trace, source audit, replication steps, or failure analysis, so the result is not yet a reproducible benchmark.

**「Takeaway」** The case suggests that agentic AI may be able to discover and test concrete archival hypotheses, while historical scholarship still depends on interpretation and contextual judgment. Its significance remains provisional until the underlying research workflow and evidence can be examined.

**Tags**: `#ai-tools`, `#ai-agents`, `#research-workflows`, `#historical-research`

---

<a id="item-tech-blog-5"></a>
### [Neon’s Uptake Signals Google DeepMind’s Frontier Return](https://latent.space/p/ainews-gemini-4-neon-marks-gdm-s-full-return-as-a-frontier-lab/) ⭐️ 5.0/10

rss · Latent Space · Nov 25, 04:29

**「Background」** The roundup begins from a low point: three months after several senior departures and disappointing Gemini 3 progress, the author says observers had written off Google DeepMind as a frontier lab. The issue argues that Gemini 4 Neon’s unusually rapid adoption has changed that assessment, while also asking how much of the surrounding excitement is measurable.

**「Solution」** Neon reportedly set a day-one usage record on Google’s paid APIs; Antigravity tokens per day were up 82% since Argon’s launch six weeks earlier, while Perplexity usage reportedly passed 120 billion Neon tokens and doubled daily volume in three days. Google expanded access through Workspace and shipped an experimental anti-slop frontend-design skill, eight generally available MCP servers, and gwscli, while one attributed estimate placed Neon xhigh at $6.44 per Artificial Analysis task versus $10.04 for Opus Max. The issue balances those signals with caveats: users reported sycophantic “glazing,” developers viewed Antigravity as still lagging Claude’s ecosystem, and exuberant user reports lacked benchmark methodology. It also notes that Neon followed GPT-6.2 Astra and Sol on Humanity’s First Exam, reinforcing that adoption and leadership are not the same claim. The wider roundup catalogs claimed frontier-model research results—including VP ≠ VNP, GPT-6 protein design, and kernel-bug validation—alongside harness-sensitive evaluations and open-weight post-training, but notes that the VP ≠ VNP claim was not independently verified and does not imply P ≠ NP.

**「Takeaway」** The author’s larger thesis is that Neon is credible evidence of Google DeepMind’s return to frontier contention, not yet proof that it leads; the roundup’s strongest contribution is showing how adoption, deployment advantages, benchmark results, and hype must be weighed separately.

**Tags**: `#ai-tools`, `#ai-models`, `#developer-tools`, `#evals`

---