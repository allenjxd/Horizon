---
layout: default
title: "Horizon Summary: 2026-11-14 (EN)"
date: 2026-11-14
lang: en
---

> From 200 items, 8 important content pieces were selected

---

**Technology News**
1. [OpenAI Launches ChatGPT Wallet for U.S. Pro Users](#item-tech-news-1) ⭐️ 8.0/10
2. [MiniMax Opens H3-Image Weights in a Faster, Cheaper Image-Model Race](#item-tech-news-2) ⭐️ 7.0/10
3. [An AI-Assisted User Feedback Loop for Service Operations](#item-tech-news-3) ⭐️ 7.0/10
4. [UK, Singapore, Thailand Central Banks Trial Partior FX Synchronization](#item-tech-news-4) ⭐️ 7.0/10
5. [Thailand Proposes $148,000 Daily Stablecoin Transfer Cap](#item-tech-news-5) ⭐️ 7.0/10
6. [Web3Auth reports wallet access restored and plans asset returns](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [AI News: Models, Agents, and NVIDIA Leadership](#item-tech-blog-1) ⭐️ 6.0/10

**AI Creator Radar**
1. [A Human-in-the-Loop AI Workflow for Review Writing](#item-ai-creator-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Launches ChatGPT Wallet for U.S. Pro Users](https://www.panewslab.com/zh/articles/01a1d572-7ea0-754b-bb7e-5c48f1d3adbe) ⭐️ 8.0/10

OpenAI launched ChatGPT Wallet for U.S. ChatGPT Pro users, allowing them to ask dot to make purchases or hotel bookings through chat while retaining approval over every transaction. Each payment requires review and biometric authorization through Face ID, Touch ID, or a supported device, after which a payment token is generated so merchants and agents do not receive the underlying card number. At launch, the wallet supports U.S.-issued American Express, Chase, Mastercard, and Visa cards for users aged 18 or older with a U.S. billing address; virtual cards and use in Chat, Work, and standalone Codex threads are not supported.

rss · PANews · Nov 13, 15:06

**「How agent payments are authorized」** Agentic purchasing requires separating a user&\#x27;s payment credential from the merchant or agent executing the transaction. ChatGPT Wallet adds an authorization layer in which per-transaction review and Face ID or Touch ID approval lead to tokenized checkout, keeping the underlying card number hidden from both the merchant and the agent.

**「Scope of agent payments」** For eligible U.S. Pro users, dot can now make purchases or hotel bookings after each transaction is reviewed and approved with Face ID or Touch ID, while the merchant or agent receives a payment token rather than the real card number. The feature requires a U.S. billing address, an eligible card, and age 18 or older; virtual cards and Chat, Work, and standalone Codex threads are not supported at launch, so users should not assume agent-initiated payments are available across those surfaces.

**Tags**: `#ai-tools`, `#agents`, `#payments`, `#product`

---

<a id="item-tech-news-2"></a>
### [MiniMax Opens H3-Image Weights in a Faster, Cheaper Image-Model Race](https://www.woshipm.com/ai/6493871.html) ⭐️ 7.0/10

MiniMax released H3-Image and opened its model weights on November 10, saying it can generate a 16-megapixel image in 10 seconds at 50%–70% of comparable mainstream tools’ price. The article compares it with OpenAI’s November 5 GPT Image 2.6 update, advertised as 50% faster than its predecessor, and ByteDance’s November 9 Seedream 5.5 release, which emphasizes stable local and multi-turn editing. In product-level tests, H3-Image’s Hailuo AI high-speed mode generated images in 10–15 seconds, versus about one minute for ChatGPT and Doubao, but it struggled to combine human faces with elaborate food-based heads; Doubao’s edits were slow and inconsistent, while GPT Image 2.6 was judged strongest overall. Artificial Analysis rankings cited by the article placed GPT Image 2.6 Sunburst first, Seedream 5.5 tenth and H3-Image 23rd for text-to-image generation, showing that H3-Image’s headline speed advantage did not translate into comparable complex-prompt or editing performance in this limited test.

rss · 人人都是产品经理 · Nov 14, 03:39

**「Release context」** The comparison follows three closely spaced releases: OpenAI’s GPT Image 2.6 on November 5, ByteDance’s Seedream 5.5 on November 9, and MiniMax’s open-weight H3-Image on November 10. The shared context is a shift beyond one-shot image generation toward repeatable editing workflows; Seedream 5.5 emphasizes steadier multi-round editing, while H3-Image provides 1K, 2K, and 4K outputs of about 16 megapixels through an open model. MiniMax’s advertised 10-second generation time is also interface-dependent: Hailuo AI’s high-speed mode took 10–15 seconds in the report, while MiniMax Code took about a minute because its agent workflow added orchestration overhead.

**「Impact for developers and enterprises」** For developers selecting an image-generation backend, H3-Image’s open weights, claimed pricing at 50%–70% of comparable mainstream tools, and reported 10–15-second generation in Hailuo AI’s high-speed mode present concrete advantages for cost-sensitive or batch workflows. However, the approximately one-minute generation and five-minute edit observed through MiniMax Code show that agent and orchestration overhead can erase that speed advantage, so teams should benchmark their exact integration path. The tests also found H3-Image failing to merge food with human faces and worsening the scene during correction, meaning teams should validate complex-prompt and iterative-edit reliability before adopting it for local deployment or customization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seeddance.io/models/seedream-5-5">Seedream 5 . 5 Free Online: AI Image Generator &amp; Editor</a></li>
<li><a href="https://kie.ai/minimax-h3-image">MiniMax H 3 Image API: 16 MP Images and Editing | Kie.ai</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-models`, `#image-generation`, `#product`

---

<a id="item-tech-news-3"></a>
### [An AI-Assisted User Feedback Loop for Service Operations](https://www.woshipm.com/pd/6493736.html) ⭐️ 7.0/10

The article describes how a health consumer-services company rebuilt user-feedback handling into a traceable workflow covering 400 support, its mobile app and mini-program, experience officers, and internal trial feedback; the company reported reducing the demand-to-product or service-standard iteration cycle from three months to one month and increasing NPS by 8 points. AI interprets feedback, suggests responsible teams, and compares complaints with structured standards, while employees verify decisions and execute training or corrective action. Deployment begins with local testing and shadow mode, in which AI records recommendations without executing them; the reported results come from one company and are not independently validated here.

rss · 人人都是产品经理 · Nov 14, 02:09

**「Operational Context」** This service model relies on people to deliver one-to-one coaching, so user complaints can concern coach conduct, course design, or venue conditions and may require operational changes rather than software changes alone. The previous workflow lacked a shared intake channel, agreed responsibility rules, and visible ticket status, leaving departments unable to determine whether feedback had been addressed.

**「Implementation Guardrail」** Teams adopting this pattern must encode responsibility and fulfillment standards as machine-comparable rules, connect ticket outcomes to relevant personnel records, and define permissions for complaint data. AI should remain advisory until its accuracy has been checked against human decisions, particularly because coach-score changes can affect earnings; the described rollout records shadow-mode decisions first and requires human approval before a score takes effect.

**Tags**: `#ai-tools`, `#product`, `#product-ops`, `#user-feedback`

---

<a id="item-tech-news-4"></a>
### [UK, Singapore, Thailand Central Banks Trial Partior FX Synchronization](https://www.theblock.co/news/regulation/2026-11-13-uk-singapore-and-thailand-central-banks-complete-foreign-exchange-settlement-trial-linking-traditional-and-tokenized-systems-439692) ⭐️ 7.0/10

The Bank of England, Monetary Authority of Singapore, and Bank of Thailand completed a cross-border foreign-exchange settlement trial using Partior’s synchronization prototype. The trial connected conventional FX settlement systems with a tokenized system across the three jurisdictions. The published findings confirm the trial’s completion, but the supplied source does not describe the prototype’s technical design, results, or practical next steps.

rss · The Block · Nov 13, 12:27

**「Background」** Cross-border foreign-exchange settlement depends on conventional payment and market infrastructure across multiple jurisdictions, so a tokenized system must interoperate with those existing processes rather than function as a separate rail. The prerequisite tested by the three central banks was whether Partior’s synchronization prototype could connect conventional and tokenized cross-border FX settlement; the supplied summary does not describe its architecture, findings, or next steps.

**「Practical implication」** Partior’s synchronization prototype has been exercised in a cross-border trial involving three central banks, providing financial-infrastructure teams with a concrete reference for linking conventional and tokenized FX settlement. However, the supplied excerpt gives no findings, technical specifications, performance results, or rollout plan, so it does not support treating the prototype as production-ready or committing to deployment without reviewing the published trial findings.

**Tags**: `#web3`, `#tokenization`, `#fintech`, `#infrastructure`

---

<a id="item-tech-news-5"></a>
### [Thailand Proposes $148,000 Daily Stablecoin Transfer Cap](https://www.theblock.co/news/regulation/2026-11-13-thailand-seeks-daily-stablecoin-cap-439676) ⭐️ 7.0/10

Thailand is considering draft stablecoin rules that would cap certain transfers at US$148,000 per day to curb money laundering. The draft would also require stablecoins to move only between accounts or wallets belonging to the same person, potentially requiring changes to compliant wallet and payment infrastructure. The proposal is not final, and the source does not specify which stablecoins or transactions are covered or when the rules would take effect.

rss · The Block · Nov 13, 10:16

**「Draft transfer restrictions」** Thailand is still at the proposal stage: the reported rules have not been presented as an operative requirement, and the supplied excerpt does not specify their scope, start date, or implementation details. The same-person wallet condition is a separate design constraint from the proposed $148,000 daily cap on certain transactions, because it concerns which accounts or wallets may participate in a transfer rather than only the transaction amount.

**「Compliance impact」** If adopted, exchanges and stablecoin payment providers handling covered transactions would need systems that enforce the $148,000 daily limit and prevent transfers between wallets owned by different people. Because the rules are still a draft and their transaction scope and implementation date are unclear, providers may need to wait for the final requirements before changing production infrastructure.

**Tags**: `#web3`, `#regulation`, `#stablecoins`, `#product`

---

<a id="item-tech-news-6"></a>
### [Web3Auth reports wallet access restored and plans asset returns](https://www.panewslab.com/zh/articles/01a1d886-a1a5-7546-8e65-166c9393c1e5) ⭐️ 7.0/10

Web3Auth said existing users of its Plug &amp; Play and Single Factor Auth \(SFA\) SDKs have regained login and wallet access after unauthorized access affected embedded wallets created through Google or Apple sign-in, including wallets used by Torus Wallet and third-party applications such as Keplr. The company said affected funds are being safeguarded and it expects to announce the asset-return process within days, but has not disclosed the root cause, loss amount, or detailed procedure. Developers must abandon SDK v9 and earlier and migrate to v10 or v11; new SFA registration remains restricted, while Sapphire developers can reopen registration by migrating to the latest SDK and Legacy network registration is scheduled to return by November 23, 2026. Web3Auth also warned users not to disclose seed phrases, private keys, or login credentials to anyone offering asset-recovery assistance.

rss · PANews · Nov 14, 05:27

**「Affected wallet infrastructure」** Web3Auth’s Plug &amp; Play and Single Factor Auth \(SFA\) SDKs supplied login and wallet-access functions for the affected embedded wallets, including wallets used by Torus Wallet and third-party applications such as Keplr. Web3Auth attributed the unauthorized access to a vulnerability in its infrastructure that affected some wallets created through Google or Apple login.

**「Developer and user impact」** Web3Auth says existing users have regained access through Plug &amp; Play and SFA, but SFA new-user registration remains restricted, so affected applications are not yet operating normally. Developers must stop using SDK v9 or earlier, upgrade to v10 or v11, and migrate Sapphire integrations to the latest SDK; new registration on the Legacy network is planned to return by November 23, 2026. Affected users should wait for Web3Auth’s official asset-return process and never disclose seed phrases, private keys, or login credentials to unsolicited recovery services.

**Tags**: `#web3`, `#wallet-security`, `#developer-tools`, `#infrastructure`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [AI News: Models, Agents, and NVIDIA Leadership](https://latent.space/p/ainews-jensen-huang-resigns-after-33-years-leading-nvidia/) ⭐️ 6.0/10

rss · Latent Space · Nov 13, 09:04

**「Background」** After NVIDIA announced Jensen Huang’s departure following 33 years as CEO, president, and board member, with CFO Colette Kress as interim CEO, the issue’s surrounding account leaves the circumstances unsettled. It then broadens into a survey of models, open weights, local inference, agents, and compute geopolitics.

**「Solution」** Google’s Gemini 4 Hydrogen is the marquee launch, offering a 1M-token context, four reasoning levels, and $1.50/$7.50 per million input/output tokens; independent measurements put it near Claude Sonnet 5.5 and GPT-6.1 Sol on intelligence, but show weaker coding results, an 8% hallucination rate, and occasional runaway reasoning. Open-weight releases widen the field: Thinking Machines’ Inkling 2 Small is a 594B-total/17B-active Apache 2.0 MoE reported running at high throughput on GB200/GB300 and Vera Rubin, while Unsloth and KQuant target better Qwen quantization but face disputed baselines and unclear RAM-versus-quality trade-offs. The agent coverage tests usefulness in practice, from Anthropic’s managed sandboxes, meeting participation, and red teaming to a Claude Code game pipeline that automates Unity builds, tests, screenshots, and merges; voice-agent demos likewise expose low costs alongside trust and accountability concerns. On infrastructure, the issue relays claims that GPU initialization patterns suggest six Chinese models used Blackwell hardware, but notes that the estimated scale could instead support the view that export controls are working and that some models used Ascend chips.

**「Takeaway」** Across this digest, the durable signal is that AI progress now depends on inference economics, workflow integration, and operational safeguards as much as benchmark gains, making its deployment caveats more valuable than any single headline.

**Tags**: `#ai-tools`, `#ai-agents`, `#local-llms`, `#creator`

---

## AI Creator Radar

<a id="item-ai-creator-1"></a>
### [A Human-in-the-Loop AI Workflow for Review Writing](https://sspai.com/post/118153) ⭐️ 7.0/10

The author describes a first-person workflow for a food-engineering review that they say was accepted and published online by Food Science, with the author serving as first author and completing the work with guidance from a teacher and reviewers. The process uses Gemini for topic exploration and outlining, Zotero for reference management, Qwen for abstract screening and section synthesis, ChatGPT for drafting support and preliminary mechanism diagrams, WorkBuddy for formatting and reference checks, and Keynote or PowerPoint for the final figures. The article emphasizes that AI expands search terms, structures abstracts, and assists drafting, while the researcher must still search databases, verify claims and data against the papers, check terminology and mechanisms, and manually revise figures; its applicability beyond food-engineering reviews is not established.

rss · 少数派 · Nov 13, 07:00

**「Why Now」** The account offers a concrete, stage-by-stage example that combines named AI tools with research databases and manual verification checkpoints, rather than presenting a generic AI-writing workflow. However, it remains a single case study: the author reports the review&\#x27;s acceptance but provides no controlled comparison of writing time, output quality, or publication success rates.

**「Content Angle」** Content angle: Show where AI genuinely reduces repetitive work and where it cannot replace research judgment, using the review&\#x27;s five-stage workflow to identify each handoff from AI assistance to database searching, source verification, and manual figure reconstruction.

**Tags**: `#ai-writing`, `#research-workflow`, `#ai-tools`, `#zotero`, `#human-in-the-loop`

---