---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 151 items, 9 important content pieces were selected

---

**Technology News**
1. [Lean and Mathlib endorse Alpöge’s Claude-assisted Riemann proof](#item-tech-news-1) ⭐️ 8.0/10
2. [VMEG AI expands video dubbing into an enterprise localization workflow](#item-tech-news-2) ⭐️ 7.0/10
3. [Zhipu Adds GLM-5.4 to Coding Plan](#item-tech-news-3) ⭐️ 7.0/10
4. [Visa expands agent verification and pilots a CLI wallet](#item-tech-news-4) ⭐️ 7.0/10
5. [Blur Disables Upgrade Paths, Locking 545.6 ETH](#item-tech-news-5) ⭐️ 7.0/10
6. [Fusionist Bridge Exploit Mints Trillions of ACE](#item-tech-news-6) ⭐️ 7.0/10
7. [OpenAI Scientist Proposes Shared Thresholds for Frontier AI Development](#item-tech-news-7) ⭐️ 7.0/10

**AI Creator Radar**
1. [Engineers’ New Focus in the Age of AI Agents](#item-ai-creator-1) ⭐️ 6.0/10
2. [Claude-Based Riemann Hypothesis Claim Enters Lean Review](#item-ai-creator-2) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lean and Mathlib endorse Alpöge’s Claude-assisted Riemann proof](https://www.panewslab.com/zh/articles/01a20261-882e-73d5-af92-7fb26f4a6cd2) ⭐️ 8.0/10

PANews reported that Lean and Mathlib jointly said they were “fully confident” Levent Alpöge’s Claude-assisted proof of the Riemann hypothesis was correct. The submitted artifact spans about 17 million lines and 175,187 Lean modules; according to the report, MIT mathematician Andrew Sutherland independently rebuilt it with Lean and Mathlib v4.33.1, dozens of researchers reproduced compilation, and several independent kernels accepted a roughly 61.6 GB export, while axiom checks reported no \`sorryAx\` and only three standard axioms. The evidence is not yet fully closed, however: some end-to-end comparator and kernel runs and sandbox-build comparisons remained unfinished, and the stated scope differs between the Riemann-hypothesis main theorem and four results concerning Dirichlet L-functions. Machine checking establishes the submitted derivation relative to Mathlib’s definitions and trusted kernels, but not that mathematicians understand the proof or that it has completed the formal publication, at least two years of public scrutiny, and broader recognition required by the Clay Millennium Prize rules.

rss · PANews · Nov 23, 01:00

**「Why formal verification matters」** Lean 4 is a proof assistant in which theorem statements and derivation steps are encoded for kernel checking, while Mathlib provides standard definitions against which the target proposition can be compared; MIT mathematician Andrew Sutherland has published verification files for the announced proof so others can inspect the reproducibility process. Machine checking is not equivalent to human mathematical understanding or prize acceptance: it still depends on faithful definitions, legitimate axioms, and the absence of placeholders such as &quot;sorry,&quot; while the report notes that publication and at least two years of public scrutiny are required for the Clay Millennium Prize. Anthropic’s earlier August Claude–Lean work had only raised a verified zero-density lower bound from 41.6% to 67.2%, making the current announcement a claimed advance from a partial result to a full formal proof.

**「Verification becomes the handoff」** For AI-research and developer teams, the immediate consequence is a concrete acceptance workflow: publish the roughly 17-million-line, 175,187-module Lean source, pin Lean/Mathlib and checker versions, rebuild independently, compare the theorem against Mathlib’s canonical \`RiemannHypothesis\`, and run multiple independent kernels on the approximately 61.6-GB export. This makes Claude’s contribution auditable as a reproducible artifact rather than a model claim, but “machine-checked,” “human-understood,” and “formally accepted” remain separate states: five modules required a higher computation-step limit, some Lean v4.36.0 runs and detailed logs remained unfinished, and the Clay process still requires formal publication and at least two years of public scrutiny before the Millennium Prize can be awarded.

<details><summary>References</summary>
<ul>
<li>RH Lean proof: verification files - MIT Mathematics</li>
<li><a href="https://www.claymath.org/events/millennium-prize-problems-lecture-series/">Millennium Prize Problems Lecture Series - Clay Mathematics Institute</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#ai-research`

---

<a id="item-tech-news-2"></a>
### [VMEG AI expands video dubbing into an enterprise localization workflow](https://www.woshipm.com/chuangye/6497922.html) ⭐️ 7.0/10

VMEG AI has expanded an overseas-facing marketing-video tool into a video-localization service for cross-border brands, enterprise training teams, and high-volume creators, translating 170+ languages with speaker separation, voice cloning, selectable AI voices, subtitles, and optional lip synchronization. Its June 2026 Glass Box Dubbing Workflow exposes transcripts, translations, speaker tracks, and timing so customers can correct terminology or pronunciation and regenerate only affected audio; in a VMEG-reported TELUS Health case, 360 minutes of English and French meeting audio was delivered in seven days with an estimated 60% cost saving versus conventional dubbing. The company said in August 2026 that it had more than two million cumulative registrations and 1,200 enterprise customers across 226 countries and regions, while a June announcement reported more than $2 million in ARR roughly 15 months after launch, with fewer than 20 employees in 2025. These business figures are company disclosures rather than independent verification, and cumulative registrations do not indicate paid customers; VMEG has not published paid-conversion, retention, revenue-mix, detailed-pricing, or third-party quality-benchmark data, leaving its competitive edge and unit economics uncertain.

rss · 人人都是产品经理 · Nov 23, 02:44

**「From Marketing Videos to Enterprise Dubbing」** VMEG AI started with AI marketing-video tools and added multilingual video translation in May 2024 after overseas customers requested localized content. By June 2026, its Glass Box Dubbing Workflow had expanded that capability into an enterprise process that exposes transcription, translation, speaker-specific dubbing, and timing for review and targeted regeneration rather than treating a one-click render as a black box.

**「Paid differentiation must move beyond language count」** HeyGen already advertises 175+ languages with voice cloning and lip synchronization, while ElevenLabs Dubbing v2 advertises 90+ languages and automatic voice cloning that preserves identity, pitch, and tone, so VMEG’s 170+ language count and core dubbing features are not unique by themselves. Buyers should therefore compare voice consistency, terminology controls, segment-level review, batch throughput, and total delivered cost; for VMEG, enterprise workflow and documented delivery performance—not the headline language total—must justify paying above free or competing automated dubbing options.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businesswire.com/news/home/20260626000999/en/VMEG-AI-Surpasses-$2M-ARR-Launches-Glass-Box-Dubbing-Workflow-for-Enterprise-Video-Localization">VMEG AI Surpasses $ 2 M ARR , Launches Glass Box Dubbing ...</a></li>
<li><a href="https://www.vmeg.ai/enterprise/">Enterprise AI Video Localization &amp; Dubbing Platform | VMEG . AI</a></li>
<li><a href="https://www.heygen.com/translate">AI Video Translator : Translate Videos into 175 + Languages</a></li>
<li><a href="https://elevenlabs.io/dubbing-studio">Dubbing v 2 : Dub content across 90 + languages and accents.</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#creator`, `#product`, `#ai-video`

---

<a id="item-tech-news-3"></a>
### [Zhipu Adds GLM-5.4 to Coding Plan](https://www.panewslab.com/zh/articles/01a20706-2ea1-74db-b899-b4f20f4cd322) ⭐️ 7.0/10

Zhipu AI announced that GLM-5.4 is now available through Coding Plan, where users can select it as \`glm-5.4\`. Zhipu says the model adds visual capabilities and stronger general coding performance, while V2, V3, and Team Plan users have received a 1.5-times increase in their GLM-5.4 usage allowance. The report provides no benchmarks, detailed plan rules, or official documentation, so the claimed improvements remain unverified.

rss · PANews · Nov 23, 06:09

**「Prior context」** OpenCode Console, formerly called Zen, already offered metered access to GLM-5.3 at 40% of its listed price, alongside a promotion for DeepSeek V4.1 Flash; this was separate from Zhipu’s Coding Plan. Zhipu says the preceding three months of parallel work on Scaling Loop and model size had already produced gains through Loop Transformer before GLM-5.4 added visual capabilities and broader general-purpose coding.

**「Coding Plan users gain expanded GLM-5.4 access」** Coding Plan users on the V2, V3, and team plans can set the model name to \`glm-5.4\` and, according to a Zhipu operator message quoted by PANews, receive 1.5 times the model quota; teams evaluating its new visual and general coding capabilities should first confirm the unspecified quota limits and compatibility rules because the report provides no benchmarks or detailed plan documentation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aipromonow.com/promos/opencode-glm-5-3-deepseek-v4-1-flash-60-off">OpenCode 按量调用 GLM - 5 .3 和 DeepSeek V4.1 Flash 打四折 | AI...</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#vibecoding`, `#coding-agents`, `#product`

---

<a id="item-tech-news-4"></a>
### [Visa expands agent verification and pilots a CLI wallet](https://www.panewslab.com/zh/articles/01a205ee-c563-7109-9307-765cdd7344b6) ⭐️ 7.0/10

Visa said it is expanding the Trusted Agent Protocol \(TAP\) and Visa Agent Directory so users can verify agents by connecting a wallet and securely adding a bank card, then register them in the directory. Agents validated through that process can, according to Visa, complete paid tasks—including video creation, music composition, gaming, paid surveys, and market research—and earn OUSD. Visa also introduced an experimental Visa CLI agent wallet for US users, built on Tempo and the Machine Payments Protocol \(MPP\), and described it as a connector for agent platforms and paid work.

rss · PANews · Nov 23, 01:04

**「Earlier foundation」** Visa unveiled the Trusted Agent Protocol \(TAP\) on October 14, 2025, as an ecosystem-led framework for agentic commerce. Its specifications use agent-specific cryptographic signatures so merchants can verify AI agents and secure agent-driven checkouts; the new expansion builds on that foundation by adding an agent directory and an experimental Visa CLI wallet.

**「A testable route to paid agent work」** The expansion provides a concrete verification, registration, task, and OUSD-payment flow for agent developers and US users. Visa CLI remains experimental and is limited to the United States, so the announcement does not establish broad availability or production readiness.

<details><summary>References</summary>
<ul>
<li><a href="https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx">Visa - Visa Introduces Trusted Agent Protocol: An Ecosystem ...</a></li>
<li><a href="https://usa.visa.com/about-visa/newsroom/press-releases.releaseId.21716.html">Visa Introduces Trusted Agent Protocol: An Ecosystem-Led ...</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#web3`, `#ai-tools`, `#payments`, `#product`

---

<a id="item-tech-news-5"></a>
### [Blur Disables Upgrade Paths, Locking 545.6 ETH](https://www.panewslab.com/zh/articles/01a205dd-70bf-7444-bdc7-80822b8f743a) ⭐️ 7.0/10

Blur disabled the Safe multisigs controlling Blur, Blend and BlurPool, leaving the related contracts without an upgrade path. Yuga Labs blockchain vice president Quit reported that approximately 545.6 ETH in Blur Pool is now permanently locked because 315 immutable contracts lack a withdraw\(\) function, including holdings associated with Moonbirds \(173.2 ETH\), Milady \(85 ETH\) and 0xSplits \(82.6 ETH\). His review of roughly 125,000 holder addresses also found 558 contracts holding about 550.9 ETH that remain withdrawable, although the withdrawals had not yet been completed. Blur’s trading interface closed on November 12 while the protocol remains on-chain, and Upbit’s previously announced BLUR delisting was scheduled for November 30.

rss · PANews · Nov 23, 00:45

**「Earlier Blur shutdown」** Blur had closed its trading interface on November 12 while leaving the protocol operational on-chain, and Upbit had announced a November 30 delisting of BLUR. The lockup occurred after that shutdown, when upgrade access was removed and some immutable pool contracts had no withdraw\(\) function through which their ETH could be recovered.

**「Permanent lock-in for certain pool holders」** The concrete consequence is that the roughly 545.6 ETH held by 315 immutable Blur Pool contracts without an implemented withdraw\(\) function has no usable withdrawal or upgrade-based recovery path, leaving those holders and dependent projects unable to retrieve the funds. The decisive compatibility check is the holding address: contracts that expose a working withdrawal function remain recoverable, while the 315 immutable contracts without one cannot rely on a future upgrade to add an exit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coingabbar.com/en/blur-eth-locked-545-6-eth-trapped-315-immutable-contracts">Blur ETH Locked: 545.6 ETH Trapped in 315 Contracts</a></li>
<li><a href="https://en.coin-turk.com/blur-pool-locks-545-6-eth-as-contract-upgrade-path-permanently-closed/">Blur Pool locks 545.6 ETH as contract upgrade path ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/approximately-545-6-eth-permanently-locked-in-blur-pool-affecting-multiple-projects">Approximately 545.6 ETH permanently locked in Blur Pool ...</a></li>

</ul>
</details>

**Tags**: `#web3`, `#ethereum`, `#nft`, `#protocol-governance`

---

<a id="item-tech-news-6"></a>
### [Fusionist Bridge Exploit Mints Trillions of ACE](https://www.panewslab.com/zh/articles/01a204d5-66bf-75a7-9719-0d8e39ab8fa4) ⭐️ 7.0/10

Fusionist, a blockchain gaming project, suffered an attack that exploited privileged minter permissions on its BNB Chain bridge, allowing an attacker to mint more than 6 trillion uncollateralized ACE tokens and exchange them for USDT before transferring funds through multiple wallets and across chains. PANews reports that 1,091.5 ETH, worth about $1.87 million, was moved through Tornado Cash, while an earlier report estimated that roughly $1.04 million in USDT was extracted after the minting of 10 quadrillion ACE. The report does not identify a confirmed root cause or remediation, and the differing token totals and loss estimates have not been reconciled.

rss · PANews · Nov 22, 19:56

**「Why bridge minter authority matters」** The relevant security mechanism is the cross-chain bridge’s privileged minter role, which can create unbacked ACE on BNB Chain if compromised rather than merely transfer existing tokens. Reports on this incident disagree on scale: the main account cites more than 6 trillion ACE minted and 1,091.5 ETH—about $1.87 million—sent through Tornado Cash, while another report estimated 10 quadrillion ACE and roughly $1.04 million in USDT extracted.

**「ACE dilution and bridge remediation risk」** The unauthorized minting exposes ACE holders to dilution and distorted pricing because more than 6 trillion uncollateralized ACE were reportedly created and exchanged for USDT. Until the root cause and remediation are confirmed, Fusionist should treat the BNB Chain minter privilege as potentially compromised by rotating or suspending it, auditing mint records and recipient wallets, and reconciling ACE and USDT flows; the report’s conflicting token and loss estimates should not be treated as verified totals.

**Tags**: `#web3`, `#security`, `#bridge`, `#tokenomics`, `#gaming`

---

<a id="item-tech-news-7"></a>
### [OpenAI Scientist Proposes Shared Thresholds for Frontier AI Development](http://www.geekpark.net/news/374304) ⭐️ 7.0/10

OpenAI chief scientist Jakub Pachocki proposed that frontier-model developers establish common evaluation, transparency, and pre-deployment red-team thresholds, using cross-company metrics such as perplexity to pause development until researchers can reliably understand and monitor model behavior. In an essay relayed by CnBeta, he reported log-perplexity readings of about 0.99 for GPT-3.5 and 0.91 for GPT-4, said models below 0.8 demonstrated new cybersecurity and mathematics capabilities, and warned that AI-driven pre-training progress could accelerate as early as 2027 faster than safety monitoring can keep pace. Sam Altman publicly supported the proposal, but it remains Pachocki’s personal recommendation rather than an adopted industry standard or a shipped OpenAI control. If competing laboratories agree, the proposed common gate would directly affect frontier-model training and release practices, including required evaluations before a model’s first use.

rss · 极客公园 · Nov 23, 01:22

**「Background」** The proposal builds on the idea that log-perplexity can serve as a cross-company measure of pretraining progress: OpenAI describes it as a model’s ability to predict the next token, with lower values indicating stronger predictions. It also draws on earlier calls for a coordinated pause in frontier-AI training, which sought to make temporary limits more technically enforceable than purely voluntary commitments.

**「Implication for model developers」** Frontier-model developers preparing for shared release standards would need to track cross-company log perplexity, document safety-monitoring capabilities, and complete evaluation, transparency, and red-team work before a model’s first use. Pachocki’s proposal specifically links capability emergence to a perplexity level around 0.76, but because it remains a proposal rather than an adopted industry rule, organizations should treat it as preparation for possible common thresholds—not as an immediate compliance requirement.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>
<li><a href="https://hardwired-pause.ai/paper">The Feasibility of a Hardwired Pause of Frontier AI Training</a></li>
<li><a href="https://aiweekly.co/alerts/openais-pachocki-urges-frontier-pause-at-068-07-perplexity">OpenAI&#x27;s Pachocki urges frontier pause at... | AI Weekly</a></li>
<li><a href="https://openai.com/index/perplexity-and-intelligence/">Perplexity and Intelligence | OpenAI</a></li>

</ul>
</details>

**Tags**: `#ai-safety`, `#model-evaluation`, `#ai-development`, `#standards`

---

## AI Creator Radar

<a id="item-ai-creator-1"></a>
### [Engineers’ New Focus in the Age of AI Agents](https://creatoreconomy.so/p/what-should-engineers-do-when-ai-writes-all-the-code-charles-lamanna) ⭐️ 6.0/10

In an interview published by Peter Yang, Microsoft EVP for Copilot and Agents Charles Lamanna argues that agents are becoming software’s main users and that engineers’ focus is moving from hand-writing code toward architecture, testing, scaling, and agent alignment. Yang relays Lamanna’s claim that some engineers are writing less code while thinking harder, and describes agent-era teams as managing agents with token budgets; he also cites that Copilot Cowork was built by 11 engineers, with one engineer maintaining the GitHub Copilot runtime. The conversation also covers Lamanna’s view of Microsoft rebuilding Office around Copilot, but it presents interviews and observations rather than a new product release, benchmark, or independently verified outcome.

rss · Creator Economy So · Nov 22, 15:03

**「Why It Matters Now」** The interview offers a timely view of how senior Microsoft leaders are framing engineering work around AI agents and Copilot, making it useful as a workflow discussion rather than a must-follow product update. The claims about reduced coding, agent management, and Office’s direction are attributed opinions; the supplied material includes no release dates or measured results.

**「A Practical Content Angle」** Content angle: Use the interview’s distinction between inexpensive code generation and costly alignment to examine what engineering work becomes more important when agents can build quickly: setting architecture, testing standards, scaling plans, and clear direction.

**Tags**: `#ai-agents`, `#ai-tools`, `#creator-workflows`, `#microsoft-copilot`

---

<a id="item-ai-creator-2"></a>
### [Claude-Based Riemann Hypothesis Claim Enters Lean Review](https://sspai.com/post/119418) ⭐️ 6.0/10

On November 20, 2026, Anthropic mathematical researcher Levent Alpöge said on his personal website that he had used Claude to find proofs of the Riemann hypothesis and generalized Riemann hypothesis, and had formalized them in Lean. Andrew Sutherland and other independent reviewers reported that all submitted Lean modules compiled and passed several checks, but Alpöge said the full paper was still forthcoming and acknowledged that he did not fully understand all of the mathematics involved. A November 21 joint statement from the Lean and Mathlib communities called the submitted formalization correct, while the source notes that core theoretical validation and scholarly interpretation remain incomplete; official recognition would require formal publication, at least two years of review, and broad academic acceptance.

rss · 少数派 · Nov 22, 23:34

**「Why It Matters Now」** The claim quickly progressed from a researcher’s personal declaration to initial independent Lean checks and a joint statement from the Lean and Mathlib communities. However, the full write-up and broader review are still pending, making this a timely case to discuss without treating the conjecture as formally solved.

**「Content Angle」** Angle: Map the verification chain from Claude-assisted discovery and Lean compilation to independent checks and formal publication, clearly separating machine-checkable correctness from the remaining human work needed to explain and review the mathematics.

**Tags**: `#ai-tools`, `#formal-verification`, `#ai-research`, `#creator-workflow`, `#mathematics`

---