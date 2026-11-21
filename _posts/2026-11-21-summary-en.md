---
layout: default
title: "Horizon Summary: 2026-11-21 (EN)"
date: 2026-11-21
lang: en
---

> From 207 items, 16 important content pieces were selected

---

**Technology News**
1. [AI-Assisted Lean Verification Reported for Tao’s Problems](#item-tech-news-1) ⭐️ 8.0/10
2. [Inkling 2 Mini targets local AI with open weights and looped architecture](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI Tests Business Management for ChatGPT Merchants](#item-tech-news-3) ⭐️ 8.0/10
4. [Lagarde backs a unified European tokenized-asset market](#item-tech-news-4) ⭐️ 8.0/10
5. [悦嫂坊 adds six service tools for independent maternity matrons](#item-tech-news-5) ⭐️ 7.0/10
6. [Author recreates Gemini Flow with DeepSeek Harness on Android](#item-tech-news-6) ⭐️ 7.0/10
7. [Meta Muse Reaches 10 Million Downloads After Seven Months](#item-tech-news-7) ⭐️ 7.0/10
8. [MoonPay Applies for National Trust Bank Charter](#item-tech-news-8) ⭐️ 7.0/10
9. [Fairmint plans Canton-first tokenized stock venue under SEC exemption](#item-tech-news-9) ⭐️ 7.0/10
10. [Bezos&\#x27;s Prometheus bets on AI-driven industrial engineering](#item-tech-news-10) ⭐️ 7.0/10

**Technology Blog**
1. [Onchain ANT Tokens and Perps Aren’t Equivalent](#item-tech-blog-1) ⭐️ 8.0/10
2. [Deceiving Hacking Agents with an Obfuscated Executable](#item-tech-blog-2) ⭐️ 8.0/10
3. [Two Riemann Hypothesis Claims and Verification Lessons](#item-tech-blog-3) ⭐️ 6.0/10
4. [Formal Verification for AI-Generated Software](#item-tech-blog-4) ⭐️ 6.0/10
5. [Anthropic&\#x27;s Record IPO and a Week of Local AI Releases](#item-tech-blog-5) ⭐️ 5.0/10

**AI Creator Radar**
1. [HarmonyOS student teams focus on cautious AI-agent design](#item-ai-creator-1) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AI-Assisted Lean Verification Reported for Tao’s Problems](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 8.0/10

The item points to Terry Tao’s post on unforced Navier–Stokes singularity and the generalized Riemann hypothesis and describes it as presenting AI-assisted work whose Lean proof was accepted by two independent kernels. Those details come from the item analysis and comments rather than the unavailable post text: the AI system, its role, the precise claims, and reproducibility are not identified. Accordingly, the supported conclusion is a reported machine-checked milestone, not independent confirmation that the named open problems have been solved.

hackernews · archon1410 · Nov 20, 17:21 · [Discussion](https://news.ycombinator.com/item?id=50578358)

**「Background」** The Euler and Navier–Stokes equations describe incompressible fluid motion, and their singularity questions ask whether sufficiently regular solutions can break down in finite time. Tao’s November 20, 2026 post connects results about unforced Euler and Navier–Stokes singularities to the Generalized Riemann Hypothesis, following OpenAI’s September 8 announcement of an AI-generated Navier–Stokes Millennium Prize solution with a formal Lean proof; the available excerpts do not establish whether the later claims extend that exact proof.

**「Verification caveat」** Anyone relying on the claimed proof should treat kernel acceptance as verification of the submitted Lean artifact, not yet as confirmation that the encoded theorem matches the intended mathematical claim or that the complete AI-assisted workflow is reproducible. A verification report says two independently built checkers accepted a Claude-developed Lean formalization but notes that further checks remain, so users should inspect the theorem statement, proof dependencies, and independent-checker reports before treating the result as a settled proof.

**「Community discussion」** Commenters focused on two concerns: softwaredoug asked how AI systems will create new abstractions beyond existing mathematical concepts, while sega\_sai and actusual expressed fear that AI-assisted proof work could displace human research or make scientists’ careers uncertain. swingboy raised a verification question: whether a passing Lean build proves the intended mathematical statement, not merely a formally encoded one, especially for a codebase described as roughly 15 million lines.

<details><summary>References</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/">Unforced Euler singularity, unforced Navier-Stokes ...</a></li>
<li><a href="https://openai.com/index/navier-stokes-solution/">On the Navier–Stokes Millennium Prize Problem | OpenAI</a></li>
<li><a href="https://xenospectrum.com/en/claude-riemann-proof-independent-verification/">Two Independent Verifiers Accept Lean Code for Claude ...</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#formal-verification`, `#ai-for-science`

---

<a id="item-tech-news-2"></a>
### [Inkling 2 Mini targets local AI with open weights and looped architecture](https://thinkingmachines.ai/news/inkling-2-mini/) ⭐️ 8.0/10

Thinking Machines has presented Inkling 2 Mini as an open-weight model built around a looped architecture and aimed at local AI inference and coding. A team note quoted in the discussion says training was performed end-to-end in NVFP4, but the supplied item contains no underlying release text or benchmark table, so the parameter count, license, download availability, and comparisons with models such as Qwen3.8-27B remain unverified. Early community reaction was positive but conditional on whether the results hold up in real-world use.

hackernews · jasondavies · Nov 20, 20:12 · [Discussion](https://news.ycombinator.com/item?id=50581260)

**「Background」** Open weights make model parameters available for local execution, and Ollama says Inkling 2 Mini can run on a Mac with 32GB or more memory. Its distinctive architecture loops the middle layers so the model performs more computation per token rather than generating additional tokens; Thinking Machines Lab also reports end-to-end NVFP4 training, pruning and healing, and low-bit quantization.

**「Local deployment with compatibility caveats」** Developers can now run Inkling 2 Mini locally rather than relying on a hosted API: Thinking Machines has released quantized GGUF versions through Unsloth and llama.cpp, with documented setups for Mac, NVIDIA, and AMD hardware. Users should verify backend compatibility before adopting it, since some optimized llama.cpp support was still in unmerged PRs; early testers reported about 27 tokens/s on a Ryzen 395 and roughly 10 tokens/s on a 32GB M1 Pro, while the vendor’s claimed benchmark parity with Qwen 3.8-27B still requires workload-specific validation.

**「Community reaction」** One tester reported 27 tokens per second decoding on a Ryzen 395 using llama.cpp&\#x27;s Vulkan backend and called the model promising in quick coding tests, while another measured about 10 tokens per second on a 32GB M1 Pro at q4\_xl and successfully wrote a CSV-sorting Python program. The latter tester said a coin-identification prompt failed and continued with unproductive output for 12,000 tokens; other commenters questioned whether benchmarks would hold up and what the broad release of looped models could mean for safety and interpretability.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://ollama.com/library/inkling-2-mini">inkling - 2 - mini</a></li>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>
<li><a href="https://unsloth.ai/docs/models/inkling-2-mini">Inkling 2 Mini - Run Locally Guide | Unsloth Documentation</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-models`, `#local-ai`, `#open-weights`

---

<a id="item-tech-news-3"></a>
### [OpenAI Tests Business Management for ChatGPT Merchants](https://www.woshipm.com/ai/6497514.html) ⭐️ 8.0/10

On November 10, OpenAI began testing Businesses in ChatGPT, adding a Business Hub where merchants can claim and edit company profiles, import price and inventory catalogs through CSV or a hosted feed, and manage products with agencies. Eligible U.S. e-commerce and online-service merchants can configure and publish a Business Agent for customer conversations, while Insights reports aggregated mentions, website clicks, and discovery topics over 28-day windows without exposing individual chats. The beta focuses on product discovery rather than checkout, and local merchants can only claim existing U.S. listings; its reported effects remain based on a secondary interpretation rather than independently measured results.

rss · 人人都是产品经理 · Nov 20, 09:06

**「From hosted checkout to merchant data」** OpenAI’s move follows the short-lived Instant Checkout experiment, launched with Stripe, Etsy, and Shopify on September 29, 2025 and shut down on March 24, 2026 after the company said the initial checkout lacked the flexibility it expected; OpenAI then shifted toward product discovery while leaving checkout with merchants. The November 10, 2026 Businesses in ChatGPT beta builds on that narrower role by adding merchant profile management and aggregated discovery insights rather than returning immediately to hosted transaction fulfillment.

**「Treat ChatGPT traffic as supplemental」** Merchants and local-service advertisers testing OpenAI-backed discovery should measure revenue per visit and purchase conversion, rather than optimize around clicks alone. A working paper found that ChatGPT ad visits converted at 0.37%, versus 1.17% for Google Search, and that 97% of advertisers earned less per visit; separate reporting put revenue at $0.89 per ChatGPT visit versus $2.45 for Google Search, supporting capped tests before shifting budget.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-businesses-chatgpt/">Introducing Businesses in ChatGPT - OpenAI</a></li>
<li><a href="https://openai.com/business/businesses-in-chatgpt/">Businesses in ChatGPT: Claim Your Business | OpenAI</a></li>
<li><a href="https://ppc.land/chatgpt-ad-visits-earn-shops-0-89-against-2-45-for-google-search-ads/">ChatGPT ad visits earn shops $0.89 against $2.45 for Google search ...</a></li>
<li><a href="https://fayfo.com/story/97-of-advertisers-earn-less-from-chatgpt-visits-115729/">97% of Advertisers Earn Less From ChatGPT Visits</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#agents`, `#product`, `#ecommerce`, `#local-search`

---

<a id="item-tech-news-4"></a>
### [Lagarde backs a unified European tokenized-asset market](https://www.panewslab.com/zh/articles/01a1f92c-a0bc-7586-8b57-599d76bfcbbb) ⭐️ 8.0/10

European Central Bank President Christine Lagarde said tokenization could create a genuinely integrated European digital-asset market, provided Europe establishes common rules and standards. She cited the ECB’s Pontes infrastructure, launched in September, which enables tokenized transactions to settle in central-bank money within the euro-area system, and an earlier-month settlement by the European Stability Mechanism of a €1 billion native digital bond through Pontes. Lagarde also reported that tokenized traditional assets recorded on public blockchains reached roughly €23 billion in March, five times their year-earlier level. She warned that divergent platform standards could fragment the market into incompatible settlement systems and said legislators, alongside the ECB’s Appia project, must support common rules because infrastructure alone is insufficient.

rss · PANews · Nov 20, 13:36

**「Background」** The immediate context is the rapid growth of tokenized traditional assets on public blockchains, whose value Lagarde said reached about €23 billion in March, five times the level a year earlier. The ECB launched Pontes in September to enable tokenized transactions to settle in central-bank money within euro-area infrastructure, establishing the technical basis for ESM’s €1 billion native digital-bond settlement earlier in November.

**「Practical Consequence」** Organizations seeking access to a unified European market for tokenized assets must treat cross-platform settlement and common rules as design constraints: Pontes can settle tokenized transactions in central-bank money, and the ESM has already used it for a €1 billion native digital bond, but divergent platform standards could leave tokens unable to settle with one another. Issuers, trading platforms, and infrastructure providers should verify Pontes compatibility and monitor the ECB and Appia standards work, while recognizing that Lagarde said legislation is still required and provided no final rule or implementation timetable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ecb.europa.eu/">European Central Bank</a></li>
<li><a href="https://themidpointnews.com/">The MidPoint News | Market structure news. Free. Always.</a></li>

</ul>
</details>

**Tags**: `#web3`, `#regulation`, `#digital-assets`, `#infrastructure`

---

<a id="item-tech-news-5"></a>
### [悦嫂坊 adds six service tools for independent maternity matrons](https://www.woshipm.com/ai/6495024.html) ⭐️ 7.0/10

The author says AI Coding helped them build 悦嫂坊, a WeChat mini-program for independent maternity matrons, with a second version containing six modules: local peer groups, shareable electronic business cards, hospital and home preparation checklists, confinement-meal ideas, fillable contracts, and service-date management. The interface targets users around ages 40–55 with larger text and buttons, plain-language labels, and simplified calendar actions, while the operator can manually create cards for users who cannot upload photos after recording their consent. Completing a contract automatically adds the engagement dates to the schedule, and presets cover 26-, 42-, and 52-day services. This is a creator-led product account without user counts, adoption evidence, implementation details, or independent validation; the author also says payments and membership were deliberately deferred until users became accustomed to the service.

rss · 人人都是产品经理 · Nov 21, 03:12

**「Product origins」** The project began as a multiyear product idea rooted in the author’s family and industry exposure: their mother has worked as a maternity nanny for more than a decade, and the author wanted a tool for independent maternity matrons. The author says they used AI Coding to implement it as the WeChat mini-program 《悦嫂坊》, and that the article followed the release of its second version.

**「Practical impact」** For independent maternity matrons using WeChat, version 2 of 悦嫂坊 consolidates peer-group access, electronic business cards, maternity-package and meal checklists, contract templates, and booking records into one mini-program; its larger text and buttons, plain-language labels, date shortcuts, and operator-assisted card entry are specifically designed for users aged roughly 40–55. The article provides no adoption or reliability data, so matrons should test the relevant workflows with clients before relying on them for contracts or scheduling, and should review any publicly shared card created through assisted entry.

**Tags**: `#ai-tools`, `#vibecoding`, `#product`, `#wechat-mini-program`

---

<a id="item-tech-news-6"></a>
### [Author recreates Gemini Flow with DeepSeek Harness on Android](https://www.woshipm.com/ai/6497702.html) ⭐️ 7.0/10

The author reports using DeepSeek Harness \(DSH\) with DeepSeek-V4.1-Flash Max to clean-room rebuild Google’s Gemini Flow as a native Android app, connecting a Xiaomi 9 Pro through ADB and using Kotlin with Jetpack Compose and a Python backend instead of decompiling the original. He says seven effective hours across 55 rounds consumed 421 million tokens and cost just over RMB 21, while the first native demo took under two hours and cost RMB 6.78. The published workflow combines uiautomator dumps, screenshots, an L0–L5 fidelity rubric, same-device side-by-side testing, and behavior checks that descend three to five levels into each workflow; documented problems included failed 8-to-16-second video extension, media re-encoding, task recovery, and API-key handling. The app and server are available in the binggandata/flowclone repository, with the reusable bggg-copy-app skill in binggandata/bggg-skills, although the reported costs, fidelity, and capabilities have not been independently verified.

rss · 人人都是产品经理 · Nov 21, 02:26

**「Clean-room mobile app replication」** The workflow uses clean-room reconstruction: the agent studies only an app’s publicly visible screens and interaction results, then rebuilds the functionality from scratch rather than decompiling code or capturing network traffic. In this case, DeepSeek Harness controlled an Android device through the Android Debug Bridge, using UI hierarchy dumps and screenshots to identify controls and visual properties before implementing a Kotlin client and Python server and validating them against the original app on the same device.

**「Practical impact」** For developers, this turns a vague AI-app cloning prompt into a reusable workflow: the released \`flowclone\` project provides a Kotlin Android client, a Python backend, UI and behavior specifications, and the \`bggg-copy-app\` skill, while the author reports completing a native Gemini Flow clone in about seven hours for roughly RMB 21. The result is a self-reported prototype rather than an independently verified 1:1 replacement for Google&\#x27;s Flow, so teams should test it on their target Android devices, rerun ADB and UI-state checks after layout changes, and keep AI-gateway credentials in the server rather than the APK. The official reference target is Google Flow, a creative studio for video, images, and related tools, so feature parity should be validated against that product.

<details><summary>References</summary>
<ul>
<li><a href="https://flow.google.com/">Google Flow - AI Creative Studio for Video , Images &amp; Custom Tools</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#vibecoding`, `#ai-agents`, `#product`

---

<a id="item-tech-news-7"></a>
### [Meta Muse Reaches 10 Million Downloads After Seven Months](https://www.woshipm.com/ai/6497691.html) ⭐️ 7.0/10

Meta says Muse, its personal AI agent, has passed 10 million downloads after seven months of development, with roughly one-quarter of users using it daily. Product lead Mona Sarantakos told Lenny’s Podcast that it grew from a weekend OpenClaw prototype connected to email, calendar, and home automation, then passed through three phases: defining the product, setting reliability and security standards with red-team testing, and running internal and external alpha tests. For sustained, multi-turn tasks, Muse uses clusters of agents to analyze real conversations, generate synthetic data, and aggregate results; Sarantakos said shopping unexpectedly became a leading use case, while smart-glasses and Charm integrations and more autonomous action remain future goals rather than shipped capabilities.

rss · 人人都是产品经理 · Nov 21, 02:14

**「From OpenClaw prototype to Muse」** Before Muse existed, product lead Mona Sarantakos spent a weekend configuring OpenClaw on a Raspberry Pi and connecting her email, calendar, and home-automation systems; by Monday, it had consolidated the family’s school notices into a brief and tracked expected schedules. That prototype prompted her to propose the product to Nat Friedman, after which the seven-month development effort focused on making an initially experimental agent reliable, secure, red-team tested, and suitable for broad consumer use.

**「Impact」** Muse’s scale makes shopping and personal productivity the most immediate proving ground for consumer-facing agents: Meta said the app had more than 10 million users and that shopping was among its leading activities. Teams building agents should prioritize concrete tasks in those areas and account for merchant-agent interoperability, while treating direct consumer-to-merchant agent conversations as exploratory rather than a generally available Muse integration.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/10/21/meta-says-muse-has-over-10m-users-with-shopping-a-top-activity/">Meta says Muse has over 10 M users, with shopping ... | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-agents`, `#product`, `#consumer-ai`

---

<a id="item-tech-news-8"></a>
### [MoonPay Applies for National Trust Bank Charter](https://www.theblock.co/news/business/2026-11-20-moonpay-applies-occ-national-bank-charter-444198) ⭐️ 7.0/10

MoonPay applied for a national trust bank charter that would bring its custody and stablecoin services under federal oversight. The crypto payments firm is joining other crypto companies pursuing similar charters, although the report says the applications face growing political scrutiny. The filing is not an approval, and the report provides no decision timeline, charter terms, or evidence of broader market impact.

rss · The Block · Nov 20, 10:39

**「National Trust Charter Context」** If granted, a national trust bank charter would place MoonPay’s custody and stablecoin-related services under a single federal OCC framework, but the application itself does not constitute approval. The OCC maintains a public list of pending digital-asset licensing applications, allowing MoonPay’s filing to be distinguished from a finalized charter.

**「Impact」** Nothing changes for MoonPay&\#x27;s customers or developers at filing: the application is not an approval, and the OCC national trust charter process described in the application guide requires a defined business plan, regulatory review, applicant-specific conditions, and final approval before the chartered activities begin. Integrators should therefore not assume new federally supervised custody or stablecoin APIs, settlement paths, or regulatory guarantees for MoonPay products, and should wait for the OCC&\#x27;s decision and the conditions attached to it before building on or communicating those capabilities. Because the charter rush is described as facing growing political scrutiny, teams relying on MoonPay-regulated rails should keep current arrangements in place and treat the outcome and its terms as unresolved.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theblock.co/news/business/2026-11-20-moonpay-applies-occ-national-bank-charter-444198">MoonPay applies for national trust bank charter to expand ...</a></li>
<li><a href="https://www.occ.gov/topics/charters-and-licensing/digital-assets-licensing-applications/index-digital-assets-licensing-applications.html">Digital Assets Licensing Applications | OCC</a></li>
<li><a href="https://www.itechguides.com/how-crypto-companies-get-a-national-trust-bank-charter/">How Crypto Companies Get an OCC National Trust Bank Charter</a></li>

</ul>
</details>

**Tags**: `#web3`, `#stablecoins`, `#regulation`, `#fintech`

---

<a id="item-tech-news-9"></a>
### [Fairmint plans Canton-first tokenized stock venue under SEC exemption](https://www.coindesk.com/business/2026/11/20/fairmint-plans-tokenized-stock-venue-on-canton-ethereum-under-sec-experiment) ⭐️ 7.0/10

Fairmint, through its wholly owned Fairmint TSV LLC, plans a tokenized-stock trading venue connecting automated market makers with issuer-authorized tokenized shares. The proposed venue would launch first on Canton Network and later connect to Ethereum, with Tradecraft named as the initial market maker and Fairmint TA serving as the SEC-registered transfer agent to verify holders, process transfers, and maintain official onchain ownership records. Fairmint TSV intends to operate under the SEC’s “innovation exemption” framework, but trading has not begun. Launch remains conditional on meeting the exemption requirements, issuing a public notice, completing relevant agreements, and becoming operationally ready.

rss · CoinDesk · Nov 20, 22:05

**「From Canton pilot to broader venue」** An earlier CoinDesk report described TSV LLC as preparing a Canton venue for issuer-sponsored tokenized Canton Strategic Holdings shares, with trading expected as early as the Monday after Oct. 29; the approach was intended to avoid the SEC’s 30-day company-objection window. Fairmint’s expanded proposal uses an AMM to connect issuer-authorized shares, initially on Canton and later on Ethereum, but remains prelaunch pending exemption requirements, public notice, completed agreements, and operational readiness.

**「Launch remains conditional」** Issuers and automated market makers do not yet have a live trading venue: launch requires meeting the SEC Innovation Exemption conditions, publishing notice, completing agreements, and reaching operational readiness. Until then, Canton support should be treated as pending and Ethereum support as a roadmap item, while Fairmint TA’s holder verification, transfer management, and on-chain ownership records describe the intended post-launch workflow.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/canton-strategic-holdings-moves-tokenize-234500958.html">Canton Strategic Holdings Moves to Tokenize Its Own Shares Under...</a></li>
<li><a href="https://www.coindesk.com/business/2026/10/29/tokenized-stock-venue-on-canton-could-beat-okx-ice-to-first-trade-under-sec-framework">Tokenized stock venue on Canton could beat OKX–ICE to first trade ...</a></li>
<li><a href="https://www.coindesk.com/business/2026/11/20/fairmint-plans-tokenized-stock-venue-on-canton-ethereum-under-sec-experiment">Fairmint plans tokenized stock venue on Canton, Ethereum ...</a></li>
<li><a href="https://phemex.com/news/article/fairmint-plans-tokenized-stock-trading-venue-on-canton-and-ethereum-under-sec-innovation-exemption-104387">Fairmint Tokenized Stock Trading Venue Canton Ethereum SEC E ...</a></li>

</ul>
</details>

**Tags**: `#web3`, `#tokenized-assets`, `#ethereum`, `#regulation`, `#product`

---

<a id="item-tech-news-10"></a>
### [Bezos&\#x27;s Prometheus bets on AI-driven industrial engineering](http://www.geekpark.net/news/374282) ⭐️ 7.0/10

At a November 17 Semafor summit in Menlo Park, Jeff Bezos said his AI startup Prometheus can complete simulated-chip, radio-device, or valve designs that previously required 10–20 engineers and six to nine months in about 12 hours. Billed as an “Artificial General Engineer,” the system combines neural surrogate models with unified multiphysics simulation to drive CAD and engineering agents; Blue Origin is privately testing it on two projects. Prometheus, co-founded by Bezos and Vik Bajaj, is valued at $41 billion and has raised about $14.5 billion. However, its tools are not publicly available, no release timetable has been announced, and the reported performance claim has not been independently verified.

rss · 极客公园 · Nov 20, 08:24

**「Background」** Prometheus emerged publicly in November 2025 with a $6.2 billion financing before raising another $12 billion in June 2026 at a $41 billion valuation. That financing sequence provides the immediate backdrop for the November 2026 demonstration: the AGE system was still being privately tested by Blue Origin and had no public release schedule.

**「Impact on engineering teams evaluating industrial AI」** Organizations in aerospace, chip, radio-device, and valve design have no access path to Prometheus yet: the only confirmed deployment is private internal testing by Blue Origin on two projects, and the company has published no product, tooling, or release date, so procurement and integration teams cannot schedule evaluation, validation, or compliance work. The design choice most relevant to those teams is that Prometheus trains on synthetic data generated by its own multiphysics simulation rather than requiring manufacturers to hand over proprietary process data — but any output still has to clear physical testing and FAA/FDA-grade review, so a hallucinated design means scrapped silicon or a failed pressure component rather than a bad paragraph of copy. Buyers should also not treat Prometheus as the only route into AI-assisted engineering: Siemens markets Industrial Copilots across design, planning, operations, and service, and LEAP 71 offers computational AI models that autonomously generate designs for physical parts, structures, and machines, both vendor-stated positions that give evaluators existing comparators.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/11/project-prometheus-bezos-bajaj-live-updates.html">Jeff Bezos and Vik Bajaj open up about Prometheus</a></li>
<li><a href="https://savedelete.com/read/prometheus-ai-2026.html">Jeff Bezos &#x27;s Prometheus Raises $ 12 B to Build an &#x27;Artificial General</a></li>
<li><a href="https://www.siemens.com/en-us/company/insights/generative-ai-industrial-copilot/">Siemens Industrial Copilot | Siemens</a></li>
<li><a href="https://leap71.com/">LEAP 71 | Engineering the Future</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#ai-tools`, `#engineering`, `#industrial-ai`, `#product`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Onchain ANT Tokens and Perps Aren’t Equivalent](https://www.bankless.com/read/what-you-own-when-you-buy-ant-onchain) ⭐️ 8.0/10

rss · Bankless · Nov 20, 20:56

**「Background」** Following Anthropic’s reported November 19 IPO debut, crypto traders can obtain nearly identical-looking ANT prices through issuer-backed tokens or cash-settled perpetual futures, but the author argues that this resemblance masks materially different economic and legal exposure.

**「Solution」** Backed tokens such as ANTx, ANTon, ANTc, Robinhood’s ANT, and rANT are generally created after an issuer acquires and custodies ANT shares, yet they typically confer no voting rights and may provide no legal claim against Anthropic. Perps such as xyz:ANT contain no shares at all, but when Nasdaq after-hours ANT was $92.60, every major instrument traded within roughly 0.5% of the others, making price a poor guide to what a buyer owns. Liquidity was substantially different: xyz:ANT recorded about $1.74 billion in 24-hour notional volume and $260 million in open interest, compared with $32 million for Robinhood’s token, $14 million for ANTx, $5 million for ANTc, and only $150,000 for ANTon; moreover, roughly 98% of ANTx tokens on Ethereum appeared to remain in its deployer’s wallet rather than buyers’ hands. The author also identifies divergent backing standards, 24/7 versus unclear redemption processes, and broad U.S. exclusions, while perp longs were paying approximately 5.5% annualized funding and could be liquidated at leverage of up to 10x. At publication, the simplest U.S. route remained the actual Nasdaq shares; a Kalshi perp was expected on November 23 pending approval, while a rights-bearing onchain version faced the SEC Innovation Exemption’s requirements for equivalent shareholder rights, no leverage, trading-volume caps, advance notice, and an Anthropic objection right, leading the author to place that possibility in 2027 or later.

**「Takeaway」** The article concludes that onchain markets did not solve the scarce IPO allocation, but did provide continuous price discovery and secondary access outside the United States; the real test is whether token structures deliver transparent backing, usable redemption, and meaningful rights rather than merely matching ANT’s price.

**Tags**: `#web3`, `#tokenized-assets`, `#crypto-trading`, `#regulation`, `#ai`

---

<a id="item-tech-blog-2"></a>
### [Deceiving Hacking Agents with an Obfuscated Executable](https://a16zfrontier.com/posts/article/deceiving-ai-hacking-agents/) ⭐️ 8.0/10

rss · a16z crypto · Nov 20, 20:55

**「Background」** After citing an FBI warning that ARTEX, an LLM-driven penetration-testing platform, had been weaponized for automated intrusions, the author asks whether defenders can manipulate what attacking agents encounter rather than only blocking them.

**「Solution」** The exploit combines ARTEX’s use of sub-agents with what the author calls two reinforcement-learned traits: relentless task completion and brittle refusal; the DeepSeek Flash models he tested reportedly showed little guardrail resistance when framed as penetration testing. Noticing that agents sometimes executed binaries presented as CAPTCHA-like obstacles, he obfuscated the executable so inspecting it became difficult and running it appeared to be the only way through. In an authorized offline CTF lab, where ARTEX was told only to find the service behind the CAPTCHA, roughly 100 runs across four models—mostly GLM 5.3 Flash and DeepSeek 4.1 1017 Flash—raised execution from probably under 10% to nearly 100%. Logs show agents checking strings and using timeouts, then rationalizing execution as the intended, low-risk lab step and citing the orchestrator; the author calls this “jagged intelligence.” Unlike prompt injection, the setup never explicitly orders the model; it supplies a familiar environmental path. The evidence remains exploratory—the lab was primitive, the malware-adjacent implementation was withheld, and generalization is uncertain—while the author stresses that testing was authorized and isolated and that “hacking back” is generally illegal.

**「Takeaway」** The author argues that apparently necessary environmental choices can steer autonomous penetration-test agents, making deception a possible active defense rather than relying on explicit prompt injection.

**Tags**: `#ai-agents`, `#ai-tools`, `#cybersecurity`, `#defensive-security`

---

<a id="item-tech-blog-3"></a>
### [Two Riemann Hypothesis Claims and Verification Lessons](https://latent.space/p/ainews-riemann-hypothesis-proved-twice-independently/) ⭐️ 6.0/10

rss · Latent Space · Nov 21, 05:02

**「Background」** The lead story concerns two unusually timed but still unverified claims to have proved the Riemann Hypothesis: Levent Alpöge’s Claude-assisted Lean artifact and Alessandro Masullo’s independent 940-page human draft. Their contrast raises a central verification question: whether a theorem can be machine-checkable without being human-readable, and whether its formal statement faithfully captures the claimed mathematical result.

**「Solution」** The author says Alpöge released 1.3GB of Lean code addressing GRH, while a prose version exceeded 250,000 pages; Elliot Glazer confirmed the formal target but reported that it was still compiling, estimating the chance of a Lean bug below 1%. Because Alpöge’s model and degree of steering were undisclosed, and Masullo’s proof remained a work in progress, the article treats both claims as provisional. It cites OpenAI’s Navier–Stokes claim as a cautionary precedent: critics questioned whether the Lean theorem matched the natural-language result. Elsewhere, the roundup argues that open models are improving faster than coding harnesses: CodeAF reportedly ranked first among ten DeepSWE harnesses using the same open model, while Inkling 2 Mini is presented as an Apache-2.0 looped MoE with 26.4B total parameters, 3.4B active parameters, and up to 1M context via YaRN. It also collects benchmark and practitioner claims for Gemini 4 Neon and Tencent’s Hy4 models, while noting that some comparisons rely on vendor data or undisclosed internal tests. The most actionable builder advice is to separate implementation from cleanup: make the code work first, then run dedicated refactoring and optimization passes.

**「Takeaway」** The author’s larger point is that AI-assisted work is becoming verifiable even when humans cannot fully comprehend it, but formal checking does not remove the need to validate statement fidelity, intended behavior, and maintainable implementation.

**Tags**: `#ai-tools`, `#vibecoding`, `#product`, `#open-models`

---

<a id="item-tech-blog-4"></a>
### [Formal Verification for AI-Generated Software](https://latent.space/p/formal-verification/) ⭐️ 6.0/10

rss · Latent Space · Nov 20, 21:18

**「Background」** As AI-generated code spreads, the author frames “slop” as a growing quality problem and asks how agent-built software can be trusted beyond an agent’s confidence. Tests, scans, patching, and model critiques expose many defects, Barrett argues, but cannot establish that no issue remains.

**「Solution」** The proposed answer is specification-first development backed by machine-checkable proofs: &amp;Truth’s Lean-based “verification machine” is meant to analyze code in any language and prove that it meets precisely stated requirements, with Lean checking each step rather than trusting the AI. Harmonic’s Aristotle similarly has AI write Lean proofs, while Axiom Math uses proof feedback to train mathematical reasoning models; Barrett also says Amazon calls cvc5 billions of times daily for specification analysis and test generation in Kiro. For security, &amp;Truth targets memory-safety proofs across C code, while Theorem and Anthropic describe LLM-scaled verification; on 36 small tasks, Anthropic reported that Opus 5.5 achieved a 50% solve rate using about 40% fewer tokens than Opus 5, though verification remains token-expensive. Barrett’s “veri-coding” vision keeps the agent in the loop but shifts human effort toward specifications and review, yet the article offers little hands-on evidence about practical costs or adoption barriers.

**「Takeaway」** The author’s central case is that formal verification could become a practical correctness gate for coding-agent outcomes, replacing confidence and sampling with explicit, checkable guarantees. If proof generation becomes precise, affordable, and easy to apply, Lean’s advances in AI-assisted mathematics could become a new software-assurance layer, though that promise remains largely vendor-led.

**Tags**: `#ai-tools`, `#vibecoding`, `#formal-verification`, `#developer-tools`

---

<a id="item-tech-blog-5"></a>
### [Anthropic&\#x27;s Record IPO and a Week of Local AI Releases](https://latent.space/p/ainews-anthropic-successfully-completes-largest-ipo-in-history-valued-at-1-5t/) ⭐️ 5.0/10

rss · Latent Space · Nov 20, 07:12

**「Background」** Latent Space&\#x27;s AINews for 11/18–11/19/2026 leads with Anthropic&\#x27;s completed IPO — an $81.3B offering priced at $83 that the digest says overtook SpaceX&\#x27;s June raise as the largest ever — framing it as a coding-focused &\#x27;Neolab IPO&\#x27; with no image or video models and no cofounder departures. The tension it sets up is whether a lab that publicly pledged to pace training &\#x27;as long as is necessary&\#x27; can now answer to shareholders, lockups, and trillion-dollar compute commitments.

**「Solution」** $ANT opened at $111.50 \(34.3% above the $83 price\), closed at $97.17 \(+17%\) before drifting to $92.60, and touched a roughly $2T fully diluted valuation at the open, with Class F shares holding 50.1% of voting power and about $1T of stock unlocking over the next year. The author&\#x27;s standout reading is that Anthropic raised ~$140B yet still holds ~$132B, implying under $10B of burn \(per Tanay Jaipuria\), while FT Unhedged&\#x27;s bear case — 20% on ~$1T of compute commitments at 40% operating margin and 17% tax — needs ~$602B/year, more than Alphabet&\#x27;s $471B or Apple&\#x27;s $478B, with proceeds largely funding data-center leasing that makes SpaceXSI an indirect beneficiary. Dario Amodei&\#x27;s IPO remarks commit to pacing training and deployment &\#x27;as long as is necessary&\#x27; so systems stay &\#x27;safe and will remain under human control,&\#x27; naming misuse by individuals or nation-states, economic disruption, and loss of control as the risks. Builder-side releases carry caveats the digest flags: Inworld&\#x27;s Apache-2.0 voice isolation \(64M offline 8-second-chunk and 58M real-time 20ms-chunk models\) separates rather than restores and its demo overlays synthetic noise; Kitten-TTS-2&\#x27;s 4MB Pico runs faster than real time on one phone CPU thread but largely ignores punctuation; AudioGhost v1.2 drops SAM-Audio&\#x27;s auxiliary models to avoid ~25GB of downloads and hold VRAM &\#x27;a bit over 4GB&\#x27; on NVIDIA, at lower quality and with no AMD path.

**「Takeaway」** Frontier AI has become a public-market story in which Anthropic&\#x27;s safety pledge must now survive lockups, compute-commitment math, and shareholder pressure, while open-science and RSI advocates circle the same listing. The deployable wins for builders this week sit in tiny permissive local models — a 4MB TTS, text-prompted sound removal — and even those arrive with caveats about prosody, CUDA-only paths, and evaluations built on synthetic noise.

**Tags**: `#ai-tools`, `#vibecoding`, `#local-ai`, `#ai-business`

---

## AI Creator Radar

<a id="item-ai-creator-1"></a>
### [HarmonyOS student teams focus on cautious AI-agent design](https://sspai.com/post/119291) ⭐️ 6.0/10

The 2026 HarmonyOS University Innovation Competition held its national finals and awards ceremony at Nanjing University, drawing from more than 800 universities, nearly 5,000 teams and nearly 10,000 students, with over 2,800 valid submissions. The article reports that Huawei announced a university innovation incubation plan offering technical support, AppGallery listing guidance and traffic support to winning student projects that are successfully published on Huawei’s app marketplace. Featured projects addressed real-world constraints by preserving missing-data states in elder-care monitoring, preventing blank sensor points from being interpreted as an absence of obstacles, and requiring confirmation before model-generated messages are treated as completed actions. The report describes competition-stage prototypes and design rules, but provides no complete workflows, deployed performance data or independently verifiable outcomes, so their readiness for scaled real-world use remains uncertain.

rss · 少数派 · Nov 21, 04:00

**「Why now」** This year’s competition was added to the national ranking for ordinary university discipline competitions, while the new incubation plan creates a concrete route from campus prototypes to app-market distribution support. The program change is documented, but adoption, user impact and commercial traction from the featured projects have not yet been demonstrated.

**「Content angle」** Potential angle: Use the student projects to examine what a reliable AI agent must refuse or double-check in safety-sensitive settings, then distinguish those documented design constraints from claims about actual performance.

**Tags**: `#ai-agents`, `#harmonyos`, `#product-development`, `#creator-tools`, `#case-study`

---