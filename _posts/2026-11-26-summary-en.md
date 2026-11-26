---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 196 items, 7 important content pieces were selected

---

**Technology News**
1. [HungerG’s Anonymous Coding Trial on Qoder and OpenCode](#item-tech-news-1) ⭐️ 7.0/10
2. [Sand.ai’s MAGI-2 brings a 480B-parameter MoE to video generation](#item-tech-news-2) ⭐️ 7.0/10
3. [XPeng Sets January 2027 IRON Production and VLA 3.0 Roadmap](#item-tech-news-3) ⭐️ 7.0/10
4. [LayerZero Adds Payment Firms as Zero Validators](#item-tech-news-4) ⭐️ 7.0/10

**Technology Blog**
1. [How tacit.wei Combines Privacy Liquidity and Resilience](#item-tech-blog-1) ⭐️ 8.0/10

**AI Creator Radar**
1. [Claude Artifacts Enter Desktop App Beta](#item-ai-creator-1) ⭐️ 8.0/10
2. [Building an AI-Assisted Map of Two Millennia of Chinese History](#item-ai-creator-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [HungerG’s Anonymous Coding Trial on Qoder and OpenCode](https://www.woshipm.com/ai/6500809.html) ⭐️ 7.0/10

HungerG, an unidentified model available for free testing on the Qoder and OpenCode coding platforms, is described as having approximately 1M tokens of context, native multimodal support, and a promise not to train on user data; no formal model card or vendor identity has been disclosed. In the author&\#x27;s tests, it produced a 1,331-line, single-file Three.js harvester in Qoder in 13 minutes, along with a disassemblable mechanical dragonfly, an interactive black-hole website, and a 675KB single-HTML game set around West Lake. The review found its coding and research output generally strong, but highlighted missing mechanical audio, no manual harvester control, low-polygon and arcade-like game limitations, primitive styling in the Word, Excel, and PowerPoint deliverables, and unresolved model provenance as reasons to assess its long-term value cautiously.

rss · 人人都是产品经理 · Nov 26, 07:13

**「Background」** HungerG first appeared anonymously in OpenCode’s catalog under the entry \`hungerg-free\`, which listed a 1,000,000-token context window and was withdrawn about 20 minutes later; it then became available for free testing in Qoder and OpenCode. Its vendor remained unconfirmed because no formal model card had been published, although OrcaRouter reported that tokenizer evidence points toward StepFun’s Step 5 family rather than proving the identity.

**「Practical impact for developers」** Developers can currently test HungerG free in Qoder and OpenCode on real tasks, with the reported trials producing interactive Three.js scenes, a single-file game, and three Office deliverables. However, teams should treat these outputs as prototypes rather than production-ready assets: the harvester lacked audio and manual steering, the game remained low-poly with shallow NPC behavior, and the Office files needed aesthetic refinement, so hands-on testing and review remain necessary.

<details><summary>References</summary>
<ul>
<li><a href="https://www.orcarouter.ai/ru/blog/hungerg-stealth-model-leak">HungerG Stealth Model : что показывают данные StepFun</a></li>
<li>HungerG 隐身模型：StepFun 证据揭示了什么 - OrcaRouter</li>

</ul>
</details>

**Tags**: `#ai-tools`, `#vibecoding`, `#3d`, `#product`

---

<a id="item-tech-news-2"></a>
### [Sand.ai’s MAGI-2 brings a 480B-parameter MoE to video generation](https://www.woshipm.com/ai/6500800.html) ⭐️ 7.0/10

Sand.ai has released MAGI-2, a 480B-total-parameter MoE video model with about 28B active parameters, using a Multi-Head Latent MoE design that decouples inter-GPU traffic from top-k routing; the team reports roughly 22% faster training than LatentMoE under its own equal-FLOP comparison. It generates 4–30-second, 1080p, 25-fps synchronized video, accepts as many as 20 mixed image, video, and audio references, and starts at RMB 0.05 per second, according to an interview with co-founder Zhang Zheng. The most striking demonstration was visual reasoning: with prompt expansion disabled, the model filled a Sudoku grid with 45 blanks, though the article notes that post-training makes successful reproduction less likely and that early reasoning and translation results include failures. The article says MAGI-2 ranked first on Artificial Analysis’s image-to-video leaderboard, but provides no benchmark scores or independent evaluations; its 4T-token pretraining corpus and data-pipeline claims likewise come from the team rather than reproducible testing.

rss · 人人都是产品经理 · Nov 26, 06:39

**「The MoE path to MAGI-2」** MAGI-2 extends a 114B-total-parameter, 6B-active preview that had already validated Sand.ai’s MoE training infrastructure and allowed text, video, and audio tokens to interact within one sequence; the new model scales that route to 480B total and about 28B active parameters. Sparse MoE reduces computation by activating only selected experts, but conventional routing can make cross-device communication grow with top-k and vary sharply with token distribution, so MAGI-2 uses Multi-Head Latent MoE to give independently routed heads and fixed head-parallel dispatch, keeping communication separate from local top-k selection.

**「Practical impact」** For creators and platform integrators, MAGI-2 supports up to 30 seconds of 1080p, 25 fps video with synchronized dialogue, sound effects, and music at a vendor-listed minimum of ¥0.05 per second, giving short-form production teams a substantially lower stated unit cost. Production adopters should still test representative prompts and audio mixes: the source says post-training reduced the reproducibility of the sudoku completion and that effects in complex soundscapes remain weaker than Seedance, so the advertised price and capabilities do not guarantee uniform output quality.

<details><summary>References</summary>
<ul>
<li><a href="https://sand.ai/blog/magi-2/">MAGI - 2 : A 480 B Frontier Video Generation Model</a></li>
<li><a href="https://higgsfield.ai/magi-2-intro">MAGI - 2 AI Video Generator with Sound | Higgsfield</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#video-generation`, `#model-architecture`, `#generative-ai`

---

<a id="item-tech-news-3"></a>
### [XPeng Sets January 2027 IRON Production and VLA 3.0 Roadmap](https://www.woshipm.com/share/6500701.html) ⭐️ 7.0/10

At XPeng’s eighth Tech Day, the company said its first IRON humanoid had completed production validation and autonomously delivered a bilingual presentation and audience Q&amp;A onstage. The 170 cm, 62 kg, 76-degree-of-freedom robot uses three XPeng-developed Turing AI chips with a claimed 2,250 TOPS of on-device computing power; XPeng plans hardware mass production in January 2027, followed by internships in its Chinese stores in Q1 and a broader external release in Q2. XPeng also introduced VLA 3.0, a shared embodied-AI architecture intended to connect its cars, Robotaxi, flying car and robots, and opened a platform through which commercial partners can download or develop robot skills. These are vendor-reported demonstrations and planned milestones rather than independently verified deployments, and XPeng acknowledged that IRON is not yet rain-resistant and that its tool-use capabilities remain under development.

rss · 人人都是产品经理 · Nov 26, 05:56

**「From prototype to production validation」** At the previous edition of XPeng’s technology day, the company cut open IRON’s leg casing onstage to verify that no person was inside, highlighting that the robot was still a prototype being presented through a live demonstration. XPeng says it subsequently restarted IRON’s hardware, software, and AI architecture while extending its second-generation VLA into a shared physical-AI stack for vehicles and robots; the announced production validation and January 2027 mass-production schedule remain vendor-reported milestones rather than independently documented deployments.

**「Deployment and compatibility impact」** IRON is not yet generally available: XPeng’s announced sequence is hardware mass production in January 2027, internships in company stores during Q1, and broader external release in Q2, so prospective users and integrators should plan for a staged pilot rather than immediate deployment. Buyers should also validate scene-specific Skills, charging, and offline operation, while noting that the launch hardware is only splash-resistant, tool use remains unfinished, and cloud compute, paid Skills, and Token subscriptions are proposed future services. This also shifts beyond XPeng’s previously reported 2026 production target, making the SOP milestone and real-store trial results important checkpoints for any earlier deployment plan.

<details><summary>References</summary>
<ul>
<li>先门店试用，再对外商用：小鹏IRON现在能干哪些实际工作？_智能机器人</li>
<li>小鹏人形机器人Iron投入工厂使用，何小鹏透露量产计划-中关村在线</li>

</ul>
</details>

**Tags**: `#physical-ai`, `#robotics`, `#embodied-ai`, `#product`, `#manufacturing`

---

<a id="item-tech-news-4"></a>
### [LayerZero Adds Payment Firms as Zero Validators](https://www.theblock.co/news/business/2026-11-25-layerzero-kakaopay-samsung-446770) ⭐️ 7.0/10

LayerZero announced that Samsung Card, Kakao Pay and ZAN will join Zero as genesis validators, helping secure the network’s consensus and proof-verification systems at launch; Four Pillars will operate the Samsung Card node. Zero is planned to launch on November 30 in sync with LayerZero’s ATLAS transaction infrastructure. Its ZK-proof design separates execution from verification, while staked ZRO is slated to be distributed equally among the genesis validators by March 31, 2027.

rss · The Block · Nov 26, 02:22

**「Zero’s validation model」** Zero separates transaction execution from verification using zero-knowledge proofs, so validators check validity proofs rather than re-execute every transaction. The chain is planned to launch on November 30 alongside LayerZero’s ATLAS transaction infrastructure, with the participating payment companies serving as genesis validators; Four Pillars is designated to operate Samsung Card’s node, while staked ZRO is scheduled for distribution to genesis validators through March 31, 2027.

**「Validator and launch implications」** The immediate consequence is operational: at Zero’s planned November 30 launch, Samsung Card, Kakao Pay, and ZAN will be responsible for consensus and proof verification as genesis validators, with Four Pillars operating Samsung Card’s node. Prospective integrators should treat November 30 as a planned launch date, not confirmation that Zero is already available.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theblock.co/news/business/2026-11-25-layerzero-kakaopay-samsung-446770">LayerZero adds Samsung Card, Kakao Pay, ZAN as validators for ...</a></li>
<li><a href="https://www.chaincatcher.com/en/article/2308127">LayerZero incorporates Samsung Card, Kakao...</a></li>

</ul>
</details>

**Tags**: `#web3`, `#layerzero`, `#zk-proofs`, `#validators`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [How tacit.wei Combines Privacy Liquidity and Resilience](https://www.bankless.com/read/inside-tacit-wei-the-app-behind-tacits-breakout) ⭐️ 8.0/10

rss · Bankless · Nov 26, 05:23

**「Background」** Tacit expanded from confidential DeFi on Bitcoin into Ethereum and other EVMs with tacit.wei, a shielded-ETH frontend built around Tacit Pay. Its product problem is liquidity: new privacy pools have small anonymity sets, so eligible deposits are routed into mature Tornado Cash pools.

**「Solution」** Each ETH deposit is split into Tornado-compatible fixed-size chunks, with the remainder sent to Tacit’s own shielded pool in one transaction, drawing on Tornado’s roughly $566 million in cited TVL while Tacit’s pool grows. Tacit’s relay handles withdrawal gas by default, self-relaying remains available, and v0.2 added private token swaps in the app. The frontend runs from contract code via gateways, making takedown harder than a normal site, but ETHBEAT still found reliance on Tacit’s relay and the Z DAO, which controls the app name and endpoints; the app also warns when fewer than 20 later deposits sit behind a deposit. For Bitcoin, Praxis uses witness encryption so a key can be unlocked by proof of a condition without forking Bitcoin, but its trusted setup requires at least one participant to discard secret randomness; a key ceremony offered browser contributions for up to 5 TAC.

**「Takeaway」** The author calls this promising but experimental: TAC reportedly rose from about $0.16 to a $1.46 peak before easing near $0.95 on Nov. 25, while trading stayed thin and the newest projects had, to the author’s knowledge, only AI security reviews. The larger argument is that mature-pool routing, resilient delivery, and privacy guardrails can make onchain privacy more practical, though trusted-setup, dependency, and audit risks remain.

**Tags**: `#web3`, `#product`, `#privacy`, `#defi`, `#bitcoin`

---

## AI Creator Radar

<a id="item-ai-creator-1"></a>
### [Claude Artifacts Enter Desktop App Beta](https://sspai.com/post/119560) ⭐️ 8.0/10

On November 25, Anthropic announced an “Install as app” option for Claude’s interactive Artifacts, allowing users to install generated applications as standalone software on macOS and Windows. Installed Artifacts can be launched from a desktop toolbar icon and may run with browser-like permissions or receive broader access for notifications, keyboard shortcuts, always-on-top display, and full computer access. The feature is in beta and rolling out gradually; the source does not specify the precise rollout scope or schedule.

rss · 少数派 · Nov 26, 00:08

**「Why Now」** This beta moves Claude-generated applications beyond browser tabs toward desktop workflows, creating an opportunity to examine how installation, delivery, and permissions work in practice. Its optional access to computer-wide controls also makes permission boundaries directly reviewable, although wider effects remain unverified while access is still rolling out.

**「Content Angle」** Content angle: A hands-on review of how installing a Claude Artifact changes launching, notifications, shortcuts, window overlays, and full-computer access on macOS and Windows, with observed behavior clearly separated from untested possibilities.

**Tags**: `#ai-tools`, `#creator`, `#workflow`, `#product`

---

<a id="item-ai-creator-2"></a>
### [Building an AI-Assisted Map of Two Millennia of Chinese History](https://sspai.com/post/117510) ⭐️ 7.0/10

In a first-person retrospective, programmer DeanChen describes turning the prompt “create a Chinese history map with a draggable timeline” into an interactive project called 江山时序. Over two and a half weeks, he says he and AI tools completed more than 200 code changes, adding city and historical-figure timelines, natural-language map queries, an English edition, GeoJSON export, and a mobile-installable version; he also manually checked open datasets and histories such as the Zizhi Tongjian and imperial records to correct boundary and city-placement errors. The author reports that the GitHub repository rose from a few dozen stars to 1,400 within days after an account on X shared it, followed by contributions focused on rendering performance, export support, and Traditional Chinese. The account does not provide a systematic data-provenance audit, an independent accuracy assessment, the technical stack, development costs, or evidence of long-term usage.

rss · 少数派 · Nov 26, 03:13

**「Why It Matters Now」** The project has already attracted noticeable open-source attention and outside contributors, giving the creator’s personal-interest experiment a visible audience beyond Chinese social platforms. However, the article does not establish the map’s overall historical accuracy or demonstrate whether its initial surge will translate into sustained use.

**「Content Angle」** A useful angle is to document the iterative workflow behind an AI-assisted vertical website: one prompt produced a rough prototype, while repeated coding and manual historical verification shaped the finished map. The clearest tension is between rapid AI-assisted development and the labor-intensive correction of data and geography.

**Tags**: `#ai-tools`, `#creator`, `#vibe-coding`, `#interactive-map`, `#product`

---