---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 144 items, 10 important content pieces were selected

---

**Technology News**
1. [Lean and Mathlib Endorse Alpöge’s Formalized Riemann Proof](#item-tech-news-1) ⭐️ 8.0/10
2. [Tencent Hunyuan Details Hy4 Roadmap, Costs, Deployment, and Weaknesses](#item-tech-news-2) ⭐️ 8.0/10
3. [Creatify Max adds AI-assisted ad management for e-commerce merchants](#item-tech-news-3) ⭐️ 7.0/10
4. [Jimeng AI’s Three Studios Connect Short-Drama Workflows in the Browser](#item-tech-news-4) ⭐️ 7.0/10
5. [Qwen3.8-27B Pi LoRA Improves Coding Accuracy Without Thinking](#item-tech-news-5) ⭐️ 7.0/10
6. [Kling Image 4.0 tests e-commerce long images and 8K output](#item-tech-news-6) ⭐️ 7.0/10
7. [Tether invests in four stablecoin payment and liquidity firms](#item-tech-news-7) ⭐️ 7.0/10
8. [Cyber Investigates CYBER Minting Anomaly; Exchanges Pause Transfers](#item-tech-news-8) ⭐️ 7.0/10
9. [Chainflip Halts Operations Over Potential Vault Vulnerability](#item-tech-news-9) ⭐️ 7.0/10
10. [ECB Opens Appia Tokenization Experiments to Industry Consortia](#item-tech-news-10) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lean and Mathlib Endorse Alpöge’s Formalized Riemann Proof](https://www.panewslab.com/zh/articles/01a2010d-7fa0-7032-bd06-92025f3c8730) ⭐️ 8.0/10

Lean and Mathlib jointly announced that Anthropic mathematician Levent Alpöge formalized a proof of the Riemann hypothesis in approximately 17 million lines of Lean code and confirmed that the proof and its stated equivalence to the conjecture were correct. The reported validation included expert review of the mathematical formulation, successful compilation, equivalence checks using two independent tools, and cross-validation by multiple independent checkers, some with set-theoretic proofs of their own formal correctness. The announcement does not explain Claude’s precise role or provide reproduction steps, and the result is presented here as a joint-statement claim rather than an independently measured outcome.

rss · PANews · Nov 22, 02:19

**「What Lean’s certification means」** Lean is a theorem-proving language with a trusted checker: it can validate a formal derivation, but successful compilation alone would not establish that the formalized target is the standard Riemann hypothesis. Alpöge released the archive on November 20, 2026, and the Lean FRO and Mathlib Initiative issued their joint certification on November 21 after equivalence checks and cross-checking by independent checkers; this concerns the proof’s formal correctness, while mathematicians still need to study and explain its underlying ideas.

**「Reproducible verification」** For researchers and formal-verification teams, the actionable artifact is the released 175,187-file Lean archive: they can inspect it and rerun the reported compilation, statement-equivalence, and kernel checks against that exact release rather than rely on media summaries. The certification supports treating the formalization as machine-checked, but it does not complete peer review of the underlying mathematical ideas, which the joint statement says will require further study.

**「Community discussion」** Commenters disagreed over what the validation establishes: one argued that cross-kernel checks make an artifact exploiting a shared flaw vanishingly unlikely, while another cited a previously reported fake Collatz refutation to question whether the checkers are truly independent. Other participants credited Alpöge’s ability to direct the AI system and noted that a human expert remained in the loop, making a checker-evading explanation less likely.

<details><summary>References</summary>
<ul>
<li><a href="https://casrai.org/news/anthropic-levent-alpoge-claude-lean-riemann-hypothesis-claim-2026">175,000-File Lean Riemann Hypothesis Proof Claim — CASRAI</a></li>
<li><a href="https://www.datastudios.org/post/claude-riemann-hypothesis-proof-lean-community-certifies-levent-alpoge">Claude-assisted Riemann hypothesis proof certified by Lean ...</a></li>
<li><a href="https://officechai.com/ai/lean-community-certifies-levent-alpoges-claude-assisted-proof-of-the-riemann-hypothesis-as-correct/">Lean Community Certifies Levent Alpöge’s Claude-Assisted ...</a></li>
<li><a href="https://casrai.org/news/anthropic-levent-alpoge-claude-lean-riemann-hypothesis-claim-2026">175,000-File Lean Riemann Hypothesis Proof Claim — CASRAI</a></li>
<li><a href="https://www.datastudios.org/post/claude-riemann-hypothesis-proof-lean-community-certifies-levent-alpoge">Claude-assisted Riemann hypothesis proof certified by Lean ...</a></li>
<li><a href="https://www.unite.ai/lean-and-mathlib-communities-certify-claude-assisted-riemann-proof/">Lean and Mathlib Communities Certify Claude-Assisted Riemann ...</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#engineering`

---

<a id="item-tech-news-2"></a>
### [Tencent Hunyuan Details Hy4 Roadmap, Costs, Deployment, and Weaknesses](http://www.geekpark.net/news/374301) ⭐️ 8.0/10

At Tencent Hunyuan’s first public global-developer Reddit AMA, chief AI scientist Yao Shunyu said the next-generation model will substantially increase its parameter count while Hunyuan continues developing both larger models and smaller edge models; Hy4-mini and Flash-Lite are planned, and a 24–31B dense model is under evaluation. Hy4 flash builds on Hy4’s iHC, gated-MLA and DSA stack with hybrid SWA, LatentMoE and Engram; the team says SWA reduces KV-cache size to one quarter, while Hy4 flash can run with 96GB of VRAM plus 128GB of system memory, is usable in OpenCode, Claude Code and Cline, and is undergoing llama.cpp adaptation. The team claims Hy4 ranked first among open models on Agent Arena and second among Chinese models on Artificial Analysis, while Hy4 flash costs one-twentieth as much per task and exceeded 50 trillion token calls on its launch day, although the article provides insufficient benchmark methodology for independent interpretation. Hunyuan self-rates Hy4 at “AGI level 2.5” but acknowledges long chains of thought, creative-writing and readability weaknesses, early-stage recursive self-improvement, and excessive refusals as unresolved issues.

rss · 极客公园 · Nov 22, 01:56

**「Earlier groundwork」** GeekPark reports that Tencent Hunyuan rebuilt its pretraining and reinforcement-learning infrastructure in February 2026, then followed a dense release schedule with Hy4 on November 4 and Hy4 flash one week later. The team described this as a preview-before-final-release cycle in which feedback from real business scenarios fed back into model development, providing context for the AMA’s emphasis on both larger models and lower-cost deployment.

**「Practical deployment impact」** Agent developers can use Hy4 and Hy4 Flash directly in OpenCode, Claude Code, and Cline, while Hy4 Flash offers teams a lower-cost option: Tencent lists 224B total parameters, 12B active per token, native multimodality, and significantly lower API pricing. Self-hosting remains hardware-intensive: the AMA cites 96 GB of VRAM plus 128 GB of system memory for Hy4 Flash, and llama.cpp support is still forthcoming, so local adopters should verify their hardware and inference-engine compatibility before deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4-flash">Introducing Hy4 flash: Ultimate cost ... - hy.tencent.ai</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#agent-coding`, `#open-source-models`, `#model-engineering`, `#product`

---

<a id="item-tech-news-3"></a>
### [Creatify Max adds AI-assisted ad management for e-commerce merchants](https://www.woshipm.com/chuangye/6497546.html) ⭐️ 7.0/10

Creatify released Creatify Max on November 18, 2026, giving e-commerce merchants and agencies one assistant for ad research, video creation, campaign management, and performance analysis. Max can connect Shopify, Google Analytics, CRM systems, and Meta, Google, and TikTok ad accounts; it can diagnose campaigns, generate follow-up creatives, create campaigns, send Slack reports, and request approval before launches, pauses, or budget changes. Creatify reported that sellers using its embedded Alibaba.com tool produced more than 200,000 videos in three months, with over 80% used in live campaigns, but that figure and Max’s internal efficiency examples are vendor-reported. Because Max is newly released and lacks substantial third-party customer evidence, its long-term reliability in managing live advertising budgets remains unverified.

rss · 人人都是产品经理 · Nov 22, 05:32

**「From creative generation to ad management」** Creatify began with a product-link-to-video generator, then used AdMax in May 2025 and Creatify Agent in May 2026 to add creative analysis and performance-data-based recommendations. Creatify Max, launched on November 18, 2026, extends that progression by monitoring ad accounts, generating ads from successful creatives, and setting up campaigns across Meta, Google, TikTok, and other platforms.

**「A guarded ad-management workflow」** Advertisers and agencies using Creatify Max can connect Shopify, Google Analytics, CRM, and Meta, Google, and TikTok ad accounts to monitor performance, generate follow-up creative, and propose campaign or budget changes within one assistant. Teams must still approve go-live, pause, and budget operations and account for inconsistent cross-platform attribution; the available results are primarily company-reported examples, with limited third-party evidence of long-term performance gains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.prweb.com/releases/creatify-launches-creatify-max-an-ai-teammate-that-runs-paid-ads-from-insight-to-creative-to-launch-302943718.html">Creatify launches Creatify Max, an AI teammate that ... - PRWeb</a></li>
<li><a href="https://creatify.ai/blog/meet-creatify-max-ai-marketing-agent">Meet Creatify Max: The AI Marketing Agent for Ads</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#product`, `#ecommerce`, `#adtech`

---

<a id="item-tech-news-4"></a>
### [Jimeng AI’s Three Studios Connect Short-Drama Workflows in the Browser](https://www.woshipm.com/ai/6497998.html) ⭐️ 7.0/10

ByteDance’s Jimeng AI launched the browser-based Short Drama Studio on October 26, joining scriptwriting, character and scene assets, storyboards, video generation, previsualization, voice, subtitles, music, and editing; Motion Studio for text and graphic animation followed on November 10, and Marketing Studio for product and advertisement videos on November 16. The short-drama workflow combines DreamScript for scripts, Anycook for images, DreamShot for storyboards, Seedance 2.5 for video, and a conversational Agent that can guide most steps; Agent conversations and text edits consume no points, while model generation does. In Z Finance’s hands-on test, an inexperienced creator turned a vague idea into a complete web-based short, but judged the output below showcase quality because character motion remained weak; storyboard prompts still required manual adjustment for framing, movement, and composition, and one scene was repeatedly rejected by moderation. The review also noted browser-performance and stability issues, while Seedance 2.5 permits clips up to 30 seconds versus 15 seconds for version 2.0; overly long clips can overload instructions, while overly fragmented edits can weaken continuity.

rss · 人人都是产品经理 · Nov 22, 02:26

**「Background」** The article presents the studio as a consolidation of a fragmented production chain: scripts, reusable assets, storyboards, generation, post-production, and handoff to Jianying \(CapCut\) now live within one project, while ByteDance’s earlier Xiaoyunque short-drama Agent has been incorporated into Jimeng. This also extends ByteDance’s broader ecosystem linking Seedance and Seedream models, Jimeng, CapCut, and distribution through Douyin and the Hongguo short-drama app.

**「Impact」** For non-specialists and small teams, the practical result is a lower operational barrier to producing a complete first cut: shared assets support character consistency, low-cost previews and segment-level regeneration can reduce wasted work, and projects can continue in CapCut. Production judgment and budgeting remain necessary, however; creators still must review storyboards, plan around 15- to 30-second generation limits, pay for repeated model calls, account for moderation rejections, and test performance on heavier browser-based timelines.

**Tags**: `#ai-tools`, `#creator`, `#product`, `#ai-video`

---

<a id="item-tech-news-5"></a>
### [Qwen3.8-27B Pi LoRA Improves Coding Accuracy Without Thinking](https://www.woshipm.com/ai/6497995.html) ⭐️ 7.0/10

harness-hub has released Qwen3.8-27B-pi-adapted, a roughly 319 MB LoRA that adds Pi Agent-specific reinforcement learning to the unchanged Qwen3.8-27B base without requiring thinking mode. According to the official results cited by the article, the adapter raised the SWE-bench Pro hard-51 pass rate from 39.2% to 64.7% and the Terminal-Bench 2.1 rate from 41.0% to 56.6% under Pi, single-attempt evaluations; these figures were not independently reproduced here. With \`enable\_thinking: false\`, median generated output reportedly fell from 48.8K to 9.4K tokens on SWE-bench Pro and from 16.5K to 3.7K on Terminal-Bench 2.1 compared with the base model using xhigh thinking. The adapter was trained using asynchronous GRPO inside Pi v1.5.2 and is documented for llama.cpp, Llama.app, vLLM dynamic-LoRA, and PEFT-merged Transformers deployments; Pi requires Node.js 22.19 or newer, and Q8\_0 or BF16 is recommended over more aggressive quantization for fidelity to training.

rss · 人人都是产品经理 · Nov 22, 01:26

**「How the Pi-specific adapter works」** LoRA \(Low-Rank Adaptation\) is a compact trainable adapter that can be mounted on a frozen base model, allowing Qwen3.8-27B-pi-adapted to change Pi-specific tool-use behavior without retraining or replacing the 27B model. The release materials describe reinforcement learning directly inside Pi’s agent environment, with task success and tool-use efficiency contributing to the reward, rather than training against a simplified imitation of the agent loop.

**「Impact」** Pi Agent users can add a small adapter to an existing Qwen3.8-27B deployment and potentially reduce coding-agent token use, tool calls, and latency. Reproducing the published behavior requires thinking to remain disabled and the correct integration path: vLLM users must enable the rank-32 dynamic LoRA and configure Pi with the \`openai-completions\` API, while llama.cpp users need the converted GGUF adapter. Lower-precision Q4 quantization may behave less consistently than the BF16-trained original, so resource-constrained users should validate Q4\_K\_M or Q4\_K\_XL results before switching from a higher-precision setup.

<details><summary>References</summary>
<ul>
<li>Datasets used to train harness-hub/Qwen3.8-27B-pi ...</li>
<li>Hugging Face Releases Qwen3.8-27B-pi-adapted LoRA ...</li>
<li>Model tree for harness-hub/Qwen3.8-27B-pi ...</li>

</ul>
</details>

**Tags**: `#ai-tools`, `#coding-agents`, `#vibecoding`, `#local-llm`, `#qwen`

---

<a id="item-tech-news-6"></a>
### [Kling Image 4.0 tests e-commerce long images and 8K output](https://www.woshipm.com/ai/6497881.html) ⭐️ 7.0/10

According to a third-party hands-on article, Kling AI’s newly launched Kling Image 4.0 can generate an e-commerce detail page in one pass from a white-background product image and a plain-language prompt, including a hero image, feature icons, product-use imagery, and a specification table, with short, medium, and long page lengths. The author also reports a multi-image mode that produces up to 10 visually consistent images, localized text editing that preserves surrounding textures, and a font panel with more than 70 preset styles plus custom-font creation from a reference image. The article describes 8K output as a native feature and a first for the product, but provides no primary release documentation, independent measurements, or complete source material to substantiate those two claims.

rss · 人人都是产品经理 · Nov 22, 00:44

**「From Kling 3.0 to 4.0」** Kling’s official comparison positions version 4.0 as an expansion of Kling 3.0, adding up to 30-second native generation, 10 keyframes, richer Omni Reference, stronger Dynamic Motions, and more flexible video editing. These documented changes concern video production and do not independently verify this article’s third-party claims about native 8K image output or its claimed “first” for that resolution.

**「Potential workflow gains require quality checks」** The tested workflow could reduce the need to assemble long product pages, campaign sets, and social assets through separate image-generation and layout steps. Before production use, teams should still inspect generated copy, specifications, product geometry, and brand details, because the evidence consists of selected examples from a third-party test rather than a documented evaluation of output accuracy or failure rates.

<details><summary>References</summary>
<ul>
<li><a href="https://klingai.com/blog/kling-4-vs-3">Kling 4.0 vs 3.0: What’s Different in the New Model?</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#image-generation`, `#product`, `#creator`

---

<a id="item-tech-news-7"></a>
### [Tether invests in four stablecoin payment and liquidity firms](https://www.panewslab.com/zh/articles/01a201c1-0a33-75d3-b6ed-44c5c1eec5be) ⭐️ 7.0/10

Between November 16 and 19, Tether invested in four stablecoin account, payment, and liquidity firms: a $15 million Series C lead for Brazil’s Nomad, an undisclosed investment in Stables, roughly $10 million alongside Abu Dhabi’s Further Asset Management in Singapore-based MetaComp, and an undisclosed investment in Swiss provider SCRYPT. The report says Stables processes more than $2 billion in annual USDT volume, while MetaComp holds a Singapore major payment-institution license and SCRYPT operates under Swiss FINMA and VQF oversight. Tether’s reported $191.5 billion in reserves and $4.5 billion in nine-month net operating profit coincided with USDT supply remaining near $184 billion, leading the article to frame these stakes as a strategy for expanding real-world USDT use as reserve income slows; however, Nomad’s USDT and XAUT integration has no announced launch date, and no terms were disclosed for the Stables or SCRYPT investments. Regulatory approval remains outside Tether’s control: USDT lacks EU MiCA authorization, Ualá has not integrated it, and Tether’s US strategy relies on Anchorage-issued USA₮ rather than USDT.

rss · PANews · Nov 22, 05:36

**「Background」** PANews describes the four-company investment push as an extension of a strategy Tether began in April 2024, when it reorganized into Data, Finance, Power and Edu and gave investments an explicit industrial purpose. That June, Tether invested $18.75 million in Taipei-based XREX for compliant cross-border B2B USDT payments, establishing the channel-investment model the latest deals extend. The approach also followed regulatory constraints: MiCA’s stablecoin provisions began applying on June 30, 2024, but USDT did not receive EU authorization, prompting Tether to invest in licensed third-party platforms.

**「Integration and availability constraints」** The investments create potential new USDT distribution paths, but they do not guarantee immediate product availability: Nomad’s USDT and XAUT integration remains exploratory with no announced launch date, so its 3.8 million customers should not be treated as newly enabled USDT users. Payment providers and enterprises should verify each partner’s license and each token’s regulatory eligibility before integration; in the EU, MiCA imposes strict issuer rules, and Binance’s removal of non-MiCA-compliant pairs while retaining USDC and EURI shows why USDT exchange support cannot be assumed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chainalysis.com/blog/stablecoins-most-popular-asset/">Stablecoins 101: Behind crypto’s most popular asset - Chainalysis</a></li>
<li><a href="https://www.binance.com/en/support/announcement/detail/bcaa1f68d6a6450099056ff694ad6c46">Binance Will Delist Non- MiCA Compliant Stablecoin Trading Pairs For...</a></li>

</ul>
</details>

**Tags**: `#web3`, `#stablecoins`, `#payments`, `#investment`

---

<a id="item-tech-news-8"></a>
### [Cyber Investigates CYBER Minting Anomaly; Exchanges Pause Transfers](https://www.panewslab.com/zh/articles/01a20124-7f44-721b-9fca-d6ba733287ae) ⭐️ 7.0/10

Cyber, the social-focused L2 network, said it is investigating an anomalous mint of CYBER on Solana and the transfer of CYBER from its cross-chain bridge’s Ethereum locked pool, while verifying the affected assets and cross-chain paths. The project asked users to stop using the CYBER bridge and not deposit CYBER into exchanges; it also said users do not need to migrate tokens, connect wallets, or sign transactions. South Korean exchanges Upbit and Bithumb suspended CYBER deposits and withdrawals, citing a suspected security incident, while the cause remains under investigation.

rss · PANews · Nov 22, 02:45

**「Background」** Cyber is a social-focused Layer 2 network whose cross-chain bridge connects CYBER on Ethereum and Solana, with an Ethereum locked pool supporting transfers between chains. The reported anomalous Solana mint and withdrawals from that pool therefore affect both token issuance and the bridge’s asset pathway, although Cyber has not yet established the cause or the affected cross-chain route.

**「CYBER transfers are temporarily restricted」** CYBER holders currently cannot deposit or withdraw through Upbit or Bithumb because both exchanges suspended those functions amid a suspected security incident. Cyber advises users to avoid its cross-chain bridge and sending CYBER to exchanges, and specifically says they do not need to migrate tokens, connect wallets, or sign requests while affected assets and transaction paths are being verified.

<details><summary>References</summary>
<ul>
<li><a href="https://bingx.com/en/flash-news/post/cyber-investigating-suspected-million-bridge-exploit-as-upbit-bithumb-freeze-transfers">Cyber investigates suspected $1 million bridge exploit as Upbit and...</a></li>

</ul>
</details>

**Tags**: `#web3`, `#security`, `#bridges`, `#L2`

---

<a id="item-tech-news-9"></a>
### [Chainflip Halts Operations Over Potential Vault Vulnerability](https://www.panewslab.com/zh/articles/01a1fed7-9ee1-7480-b8d3-c5b72dff8a12) ⭐️ 7.0/10

Chainflip has placed its cross-chain trading protocol into “Full Safe Mode” after discovering a potential vulnerability that could affect its vaults. The team has paused deposits, withdrawals, swaps, and quote services while investigating, but has not disclosed the vulnerability’s cause, scope, or potential losses. A separate earlier report alleged that an attack caused about $4.86 million in losses and that the stolen ETH was laundered through Tornado Cash, though Chainflip’s current statement does not confirm those figures. Users should avoid depositing funds or initiating transactions until the protocol provides further technical details.

rss · PANews · Nov 21, 16:01

**「Background」** The reported figure of roughly $4.86 million came from a security monitor’s estimate of Ethereum vault outflows, while Chainflip itself had only confirmed that it was investigating a possible exploit; it was therefore not an official determination of lost funds. Chainflip’s Full Safe Mode disabled deposits, withdrawals, swaps, and quotes as a containment measure while the root cause, scope, and potential losses remained undisclosed.

**「Protocol operations and fund access」** Chainflip’s Full Safe Mode currently blocks deposits, withdrawals, swaps, and quote requests, so users cannot move funds into or out of the protocol through its normal functions while the investigation continues. On-chain analysts estimate roughly $4.86 million in ETH, USDC, and USDT was drained, with most assets reportedly converted to ETH and sent to Tornado Cash, although Chainflip has not officially confirmed that loss figure.

<details><summary>References</summary>
<ul>
<li>Chainflip Halts Swaps Over Potential Vault Exploit - The Defiant</li>
<li>Chainflip investigates possible exploit, halts deposits, withdrawals ...</li>
<li><a href="https://bingx.com/en/flash-news/post/chainflip-ethereum-vault-drained-of-m-in-minutes-as-flip-drops">Cointelegraph: REKT: $ 4 . 86 M exits Chainflip Ethereum vault via...</a></li>
<li><a href="https://forklog.com/en/chainflip-halts-operations-due-to-potential-hack/">Chainflip Halts Operations Due to Potential Hack | ForkLog</a></li>

</ul>
</details>

**Tags**: `#web3`, `#security`, `#chainflip`, `#defi`

---

<a id="item-tech-news-10"></a>
### [ECB Opens Appia Tokenization Experiments to Industry Consortia](https://www.panewslab.com/zh/articles/01a1fd83-e9df-75ef-8e69-36035d0ac11d) ⭐️ 7.0/10

The European Central Bank is inviting financial-sector participants to apply, as consortia of independent legal entities, for Appia experiments covering tokenized deposits and payments, tokenized securities, and shared network governance. Teams may propose one or more workflows, which will be evaluated for expertise, practical experience, technical readiness, and expected contribution; first-round applications close on December 11, with later submissions reviewed on a rolling basis. The ECB plans to publish a blueprint in 2028 summarizing the findings and proposed frameworks, so the initiative remains at the experimental solicitation stage rather than representing a deployed tokenization capability.

rss · PANews · Nov 21, 09:50

**「Appia’s Consortium Testing Model」** Appia’s experiments focus on the operational prerequisite for tokenized finance: coordinating payment and asset workflows across several financial institutions while defining rules for shared network governance. Participation is organized around collective initiatives made up of independent legal entities, with the trials intended to provide findings and recommendations for an ECB framework blueprint planned for 2028.

**「What institutions must do」** Banks and other financial institutions seeking to test tokenized deposits, tokenized securities, or shared network governance must apply as a collective initiative composed of independent legal entities; the first application deadline is December 11, while later submissions are assessed on a rolling basis. Teams may propose one or more workflows and will be evaluated on expertise, technical readiness, and expected contribution, with findings intended to inform the ECB’s planned 2028 blueprint and recommended framework. Appia’s official roadmap also requires central bank money to remain central to the tokenized financial ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ecb.europa.eu/press/pr/date/2026/html/ecb.pr260311~14ddf51a77.en.html">Eurosystem Unveils Appia Roadmap for Europe’s Tokenised Finance</a></li>
<li><a href="https://finance-monthly.com/ecb-appia-tokenisation-initiative/">ECB Opens Appia Tokenisation Initiative to Financial Firms</a></li>

</ul>
</details>

**Tags**: `#web3`, `#tokenization`, `#regulation`, `#infrastructure`

---