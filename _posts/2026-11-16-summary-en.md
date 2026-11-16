---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 154 items, 10 important content pieces were selected

---

**Technology News**
1. [Qwen4-Max Debuts with 2.4T-Parameter MoE and 1M-Token Context](#item-tech-news-1) ⭐️ 8.0/10
2. [DeepSeek’s Open-Source Chat Demo Nearly Mirrors the App, but PDF and Costs Differ](#item-tech-news-2) ⭐️ 8.0/10
3. [Meituan Open-Sources 1.6T-Parameter LongCat-2.5 Agent Model](#item-tech-news-3) ⭐️ 8.0/10
4. [Doubao App adds conversational map-based store search](#item-tech-news-4) ⭐️ 7.0/10
5. [Qwen4-Max-Preview Tests Favor Coding and Office Work](#item-tech-news-5) ⭐️ 7.0/10
6. [terminal-mac Isolates AI Agents in an Apple Silicon macOS VM](#item-tech-news-6) ⭐️ 7.0/10
7. [21 Institutions Commit $270 Million to Project Faro Stablecoin](#item-tech-news-7) ⭐️ 7.0/10

**AI Creator Radar**
1. [How Anthropic Designer Nate Parrott Uses Claude to Reduce Generic Design](#item-ai-creator-1) ⭐️ 7.0/10
2. [Building a Retro Local Music Player with AI Coding Tools](#item-ai-creator-2) ⭐️ 6.0/10
3. [Daily Brief: Over 100,000 Signatures Urge Jensen Huang’s Return](#item-ai-creator-3) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen4-Max Debuts with 2.4T-Parameter MoE and 1M-Token Context](https://qwen.ai/blog?id=qwen4-max) ⭐️ 8.0/10

Alibaba launched the Qwen4 generation, making Qwen4-Max available on the Qwen AI platform through API services and Token Plans for developers and enterprises. The model uses a new mixture-of-experts architecture based on Qwen Sparse Attention \(QSA\), has 2.4 trillion total parameters, and supports native vision and a 1-million-token context window; Alibaba also claims stable long-horizon task delivery. Qwen4-Max exposes four reasoning-effort settings: none, low, high, and xhigh.

hackernews · ilreb · Nov 16, 02:14 · [Discussion](https://news.ycombinator.com/item?id=50513215)

**「Architecture and configurable reasoning」** Qwen4-Max uses a sparse-attention mixture-of-experts architecture designed for native vision and million-token context. Its four reasoning-effort settings—none, low, high, and xhigh—let developers vary inference-time computation when balancing capability, price, and serving speed.

**「Practical impact for developers」** Qwen4-Max is now callable through Qwen AI’s API and Token Plan, giving developers and enterprises an option to test native-vision, long-context, and long-horizon tool workflows. Before production adoption, teams should verify the effective context limit on their integration—the vendor advertises one million tokens, while Artificial Analysis lists 984K—and benchmark end-to-end task cost and latency, since token consumption, caching, and pricing can reverse comparisons based on token price alone.

**「Cost and Serving-Speed Debate」** Practitioners focused on benchmark quality, price, and inference speed: one commenter cites Artificial Analysis figures of 43 and $3.27 average cost for Qwen4-Max, compared with 46 and $0.36 for GPT-6.1 Sol at medium reasoning, while another reports that a prior Qwen model ran at about 30 tokens per second versus roughly 80 for Opus in their OpenCode setup, though it performed better with voting excluded. Simon Willison highlighted the four reasoning-effort modes, and another commenter questioned whether open-weight models are improving as quickly as Anthropic&\#x27;s and OpenAI&\#x27;s.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen4-max">Qwen4 Max: Intelligence, Performance &amp; Price Analysis</a></li>
<li><a href="https://qwen.ai/blog?id=qwen4-max">Qwen4-Max: Your New Teammate Has Arrived</a></li>
<li><a href="https://kingy.ai/blog/qwen-4-release-date-status/">Qwen4-Max benchmarks, pricing and specs: How it compares</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-coding`, `#agents`, `#models`

---

<a id="item-tech-news-2"></a>
### [DeepSeek’s Open-Source Chat Demo Nearly Mirrors the App, but PDF and Costs Differ](https://www.woshipm.com/ai/6494311.html) ⭐️ 8.0/10

DeepSeek recently exposed APIs for web search, deep-thinking search, file and URL reading, speech recognition, and text-to-speech, and published an open-source chat-demo that runs with Node.js 22.12+ and pnpm or through an online version. The article says its deepseek-flash requests work through Anthropic-compatible Messages, OpenAI Responses, and Chat Completions endpoints, giving developers most of the official app’s interface and tool behavior without building the client from scratch. In the author’s testing, web search, deep-search answers, and URL reading largely matched the official app, including cited pricing, but an image-only PDF uploaded through the demo’s /anthropic/v1/files endpoint appeared empty while the same file succeeded through /files; the demo also rendered a dollar sign as a math delimiter. Costs varied with model behavior: the same deep-search task triggered three keywords and about RMB 0.028 in one API run versus nine keywords and about RMB 0.067 in the demo, while deepseek-flash’s off-peak price was RMB 1 per million uncached input tokens and RMB 4 per million output tokens.

rss · 人人都是产品经理 · Nov 16, 03:10

**「Background」** DeepSeek’s official web app already handled web search and file uploads through dedicated app-specific prompts rather than relying solely on a generic chatbot prompt, as documented in a community-maintained prompt collection. The new chatbot API and open-source demo expose that orchestration through tool declarations, \`latest\_reminder\` metadata, file references, and speech endpoints, so reproducing the App requires rebuilding its backend behavior as well as its interface.

**「Implementation Consequences」** Developers building a public client should route scanned or image-based PDFs through /files, keep the API key behind a backend because the demo stores it in browser local storage, and enable safety\_check at the high level when offering the service externally, as DeepSeek requires. API compatibility also has constraints: enabling tools, safety checks, or titles causes temperature and top\_p to be ignored; max\_tokens applies to each reasoning step rather than the whole answer; and latest\_reminder must immediately precede a user message and is unsupported by the Responses protocol. Teams should budget for keyword-level search charges rather than a fixed cost per query, while ordinary users can continue using the free official DeepSeek app.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/langgptai/awesome-deepseek-prompts/blob/main/README.md">awesome- deepseek -prompts/README.md at main...</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#vibecoding`, `#product`, `#api`, `#deepseek`

---

<a id="item-tech-news-3"></a>
### [Meituan Open-Sources 1.6T-Parameter LongCat-2.5 Agent Model](https://www.panewslab.com/zh/articles/01a1def9-753a-76a6-93ee-c7391db07d2b) ⭐️ 8.0/10

Meituan’s LongCat team released the LongCat-2.5 agent-model weights under the MIT license, according to PANews’ report citing The Decoder. The 1.6-trillion-total-parameter mixture-of-experts model activates about 48 billion parameters per token, supports a 1-million-token context window, and was trained entirely on Chinese hardware. Meituan also published a 4-bit quantized version and a self-hosting guide based on 194 Huawei Ascend chips, with no NVIDIA GPU instructions, while offering a limited-time API price of approximately €0.27 per million input tokens and €1.07 per million output tokens. Meituan reported a Terminal Bench v2.1 score of 88.4, compared with 89.1 for Claude Opus 5 and 88.8 for GPT-5.6 Sol; these are company-published comparisons rather than independently verified results.

rss · PANews · Nov 15, 11:30

**「Architecture and deployment context」** LongCat-2.5 uses a mixture-of-experts \(MoE\) architecture: its 1.6 trillion total parameters are distributed across experts, but only about 48 billion are activated per token, so the total parameter count does not represent the model capacity exercised at each inference step. For deployment, Meituan provides a 4-bit quantized build and a self-hosting guide based on 194 Huawei Ascend chips, but no Nvidia GPU recipe, making hardware support an explicit prerequisite for reproducing its published setup.

**「Deployment impact」** The only documented self-hosting path for LongCat-2.5 is tightly coupled to Ascend hardware: Meituan’s 4-bit guide targets 194 Huawei Ascend chips and provides no Nvidia GPU setup, so organizations seeking on-premises deployment must budget for compatible infrastructure or use the API instead. The promotional API is priced at about €0.27 per million input tokens and €1.07 per million output tokens, but teams should independently test the model on their workloads before relying on Meituan’s company-reported coding-agent scores.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/models/longcat-2.5">LongCat-2.5: Benchmarks, Pricing &amp; Context Window</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-agents`, `#vibecoding`, `#open-source`, `#ai-hardware`

---

<a id="item-tech-news-4"></a>
### [Doubao App adds conversational map-based store search](https://www.woshipm.com/ai/6494326.html) ⭐️ 7.0/10

Doubao has launched a “Find Store” feature that lets app users describe local needs in chat and see matching businesses plotted on a map. Results cover nearby restaurants, attractions, hotels, gas stations, and entertainment venues, with natural-language filters for party size, meal period, and budget, plus per-person prices, operating status, ratings, group-buy packages, and vouchers. Users can open a merchant page to purchase a deal or start navigation without leaving Doubao, extending its existing travel, ride-hailing, and hotel-booking features into local commerce. The report does not provide rollout scope, technical implementation details, user adoption figures, or measured conversion results.

rss · 人人都是产品经理 · Nov 16, 03:25

**「Background」** AI assistants traditionally returned text lists, leaving users to copy business names into map and group-buying apps. Doubao’s earlier “出行用豆包” entry had connected travel, ride-hailing, navigation, and hotel booking; “找店” applies that action-oriented approach to nearby merchants, with natural-language filters leading to map results, group-buy offers, ordering, and navigation.

**「Practical impact」** Users can now complete a nearby-shop search, compare locations and group-buy offers on a map, place an order, and start navigation without copying store names into separate map and shopping apps. Merchants may gain additional exposure through Doubao’s map listings, although the report provides no user-scale or conversion data to quantify the commercial effect.

**Tags**: `#ai-tools`, `#product`, `#local-commerce`, `#conversational-ai`

---

<a id="item-tech-news-5"></a>
### [Qwen4-Max-Preview Tests Favor Coding and Office Work](https://www.woshipm.com/evaluating/6494229.html) ⭐️ 7.0/10

Alibaba launched Qwen4-Max-Preview on November 11 as a 15-day preview for developers and office users, with text, image, and video input, a 1-million-token context window, and roughly 390,000 maximum output tokens, distributed through six channels including Token Plan, the Qwen app, Qoder, Qwen Office, QwenStudio, and Qwen Chat. Z Finance’s 12-test hands-on report found the model strongest on formula-based Excel, editable PowerPoint generation, iterative document revisions, long-record retrieval, and code repair, where it produced a package passing 57 tests; the tests also exposed an overstated convergence conclusion and omissions in generated outputs. The article interprets the absence of parameter details, technical documentation, and leaderboard results as a shift toward subscription-linked coding and Agent usage, but that strategic conclusion remains the author’s interpretation rather than an independently verified Alibaba statement.

rss · 人人都是产品经理 · Nov 16, 03:12

**「Qwen4 preview context」** Qwen4-Max-Preview went live on November 11, 2026, with developer documentation reporting a 1-million-token context window and room for roughly 390,000 tokens of output—limits suited to whole-document analysis and large generated artifacts. The source describes a fixed-weight, 15-day preview window, making it a controlled trial of long-context, office, coding, and agent workflows rather than an open-ended flagship release.

**「Practical impact」** Developers can evaluate Qwen4-Max-Preview as a workflow model, not just a benchmark leader: the reported tests produced formula-backed Excel files, editable presentations, offline web artifacts, and a repaired code package whose 57 tests passed, with text, image, and video input and a 1M-token context window also listed for the API model. Teams should validate these outputs in their own workflows, retain human review for qualitative conclusions because the model overstated convergence in the research reproduction, and plan around the reported 15-day preview period and inconsistent billing and file-output behavior across its six entry points.

<details><summary>References</summary>
<ul>
<li><a href="https://oneaiapikey.com/resources/blog/qwen4-max-preview-context-window">Qwen 4 Max Preview Context Window: the 1M- Token Window and...</a></li>
<li><a href="https://openrouter.ai/qwen/qwen4-max">Qwen 4 Max - API Pricing &amp; Providers | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#agentic-coding`, `#qwen`, `#product`, `#vibecoding`

---

<a id="item-tech-news-6"></a>
### [terminal-mac Isolates AI Agents in an Apple Silicon macOS VM](https://www.woshipm.com/ai/6494316.html) ⭐️ 7.0/10

The open-source terminal-mac project reportedly gives an AI agent a separate macOS desktop by running a guest through Apple’s Virtualization framework on Apple Silicon; Windows is not supported. According to the article, its built-in MCP server supports screenshots, clicking, dragging, scrolling, typing, and keyboard input, while Kitty or iTerm2 graphics protocols display the virtual Mac inside a terminal. The guest has separate files and settings and does not share the host’s main directory, project folders, clipboard, camera, or microphone, but the outer agent retains its existing host permissions, and terminals without a supported graphics protocol fall back to a separate VM window that may still affect focus.

rss · 人人都是产品经理 · Nov 16, 03:12

**「Background」** Desktop agents need an environment that can observe screens and receive GUI input, which a browser sandbox cannot provide when testing native macOS applications. The repository describes terminal-mac as an early-release candidate for Apple Silicon that uses Apple Virtualization for a real macOS guest, with a bundled helper capturing the screen and posting input events while a terminal viewer streams the display through the Kitty or iTerm2 graphics protocol.

**「Practical impact for developers」** Developers on Apple Silicon can connect Claude Code or other MCP-compatible clients to a separate macOS guest and give agents screenshot, click, drag, scroll, type, and key operations without taking over the host’s mouse, clipboard, or working documents. To avoid focus disruption, they must use a graphics-capable terminal such as Kitty, iTerm2, or Ghostty; otherwise terminal-mac falls back to a separate VM window, and the outer agent’s existing host permissions still need separate restriction.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/govijr/terminal-mac">GitHub - govijr/terminal-mac: Entire MacOS running in your ...</a></li>
<li><a href="https://github.com/govijr/terminal-mac/tree/main">GitHub - govijr/terminal-mac: Entire MacOS running in your ...</a></li>
<li><a href="https://github.com/govijr/terminal-mac">GitHub - govijr / terminal - mac : Entire MacOS running in your terminal.</a></li>
<li><a href="https://gitnova.dev/en/r/govijr/terminal-mac">govijr / terminal - mac — what it is and what it’s for | GitNova</a></li>

</ul>
</details>

**Tags**: `#ai-tools`, `#ai-agents`, `#vibecoding`, `#developer-tools`, `#macos`

---

<a id="item-tech-news-7"></a>
### [21 Institutions Commit $270 Million to Project Faro Stablecoin](https://www.panewslab.com/zh/articles/01a1dff9-1212-7390-b479-43499460d8eb) ⭐️ 7.0/10

Twenty-one financial institutions, including Goldman Sachs, Citigroup, Santander and Deutsche Bank, have committed approximately $270 million over five years to Project Faro, a dollar stablecoin project whose issuer plans to register in the United States and target a 2027 launch. The initiative aims to compete with Tether and Circle, which the report says together account for about 85% of a roughly $2.9 trillion stablecoin market. It remains a pre-launch undertaking: the project has no final name, CEO or token yet.

rss · PANews · Nov 15, 16:10

**「Background」** Project Faro would add a consortium-led dollar stablecoin to a market currently dominated by two issuers. The report also describes other institutional moves, including SoFi expanding SoFiUSD to Polygon, Anchorage Digital enabling its token to settle through Visa’s network, and Mastercard and BVNK launching the Global Money Platform.

**「Impact」** For banks and payment developers, the immediate result is a five-year funding commitment rather than usable payment infrastructure. Organizations should not treat Project Faro as an available stablecoin until a token, issuer leadership and further product details are disclosed, with launch only targeted for 2027.

**Tags**: `#web3`, `#stablecoins`, `#payments`, `#institutional-adoption`

---

## AI Creator Radar

<a id="item-ai-creator-1"></a>
### [How Anthropic Designer Nate Parrott Uses Claude to Reduce Generic Design](https://creatoreconomy.so/p/how-to-fix-ai-slop-with-claude-design-nate-parrott) ⭐️ 7.0/10

In an episode published on November 15, 2026, Anthropic designer Nate Parrott demonstrates workflows for designing with Claude, including turning a phone note into a Duet feature prototype, transforming a spreadsheet into a live dashboard, and converting that dashboard into a Claude Motion video. His five recommendations are to provide context and reference material upfront, research familiar UX patterns, identify and discourage Claude’s known design biases, begin with wireframes, and generate multiple options before remixing selected elements. The episode also covers prototype timelines, why Claude Design launched as a separate product, signs of AI-generated design, and how to evaluate design taste when AI cannot reliably judge it. These are demonstrations and recommendations rather than independently verified performance results.

rss · Creator Economy So · Nov 15, 14:05

**「Why It Matters」** The announcement provides a concrete, current workflow for creators who want to move from rough inputs such as notes or spreadsheets to interactive and motion-based outputs while avoiding familiar generic design patterns. The source does not establish a new Claude platform update or quantify how much the methods improve design quality.

**「Content Angle」** Possible angle: A practical breakdown of Claude’s “AI slop” workflow—supplying references, starting with wireframes, and using an options-and-remix loop—alongside the phone-note, spreadsheet, dashboard, and motion-video demonstrations.

**Tags**: `#creator`, `#ai-tools`, `#design`, `#workflow`, `#anthropic`

---

<a id="item-ai-creator-2"></a>
### [Building a Retro Local Music Player with AI Coding Tools](https://sspai.com/post/119012) ⭐️ 6.0/10

Author 西鸽 says they used AI coding tools to build 不卡带, a retro-styled local media player that is now basically usable and listed in the vivo app store. It plays local audio and video, can import NAS media through WebDAV, supports Webamp skins and EQ presets, and has been adapted for the outer screens of the vivo X Flip, moto Razr 50 Ultra, OPPO Find N2, and Nothing Phone 4a Pro. The author also reports that the prototype-to-polish phase was substantially more demanding: Antigravity’s usage ran out within days, prompting a switch to Codex. Skin compatibility remains only partially tested, while the device-sound filters are explicitly described as imagined effects that users should verify; the app targets listeners interested in local music, nostalgia, and foldable phones.

rss · 少数派 · Nov 16, 02:52

**「Why Now」** The app has moved from a prototype to a publicly downloadable test in the vivo app store, allowing readers to evaluate the author’s account directly. However, this remains a single creator’s experience without measured development time, model-cost data, adoption figures, or evidence of a broader change in AI-assisted software development.

**「Content Angle」** Content angle: Use 不卡带 as a case study in the gap between quickly producing functional code and the slower work of adapting multiple foldable devices, refining the interface, and testing skin compatibility, with the switch from Antigravity to Codex as the central tension.

**Tags**: `#ai-tools`, `#indie-apps`, `#product-design`, `#creator`

---

<a id="item-ai-creator-3"></a>
### [Daily Brief: Over 100,000 Signatures Urge Jensen Huang’s Return](https://sspai.com/post/119119) ⭐️ 6.0/10

The Nov. 15 daily brief reports that the public letter “Stand with Jensen” had collected more than 108,000 signatures by the afternoon of Nov. 14, including over 58,000 shareholders and 5,600 current employees, amid reporting that NVIDIA co-founder Jensen Huang had resigned, might return and faced calls not to replace him hastily. This is a secondary roundup without a primary announcement confirming his resignation or reinstatement, so the petition demonstrates support rather than a completed leadership change. It also says Microsoft 365 was fully restored early on Nov. 14 after an outage described as lasting about 19 hours, affecting more than 70 countries and around 20 services, including Outlook, Teams and Copilot. Microsoft attributed the incident to a technical problem introduced by a recent upgrade and ruled out a network attack or an AI agent; reported disruptions affected government and court offices, healthcare, banks, Euronext, Maersk and corporate communications, with some users falling back to phone and paper notices.

rss · 少数派 · Nov 15, 23:24

**「Why Now」** The petition has reached a measurable scale while cited reporting says Huang is exploring a return, but the supplied material does not confirm that he has been reinstated. The Microsoft 365 outage has already ended according to the brief, so the current focus is the scale of the disruption and its stated technical cause rather than an active outage.

**「Content Angle」** Content angle: A fact-checked governance explainer on what the 108,000-signature petition shows about shareholder and employee support for Jensen Huang—and what it cannot establish about his status or NVIDIA’s succession process.

**Tags**: `#ai-tools`, `#NVIDIA`, `#Microsoft-365`, `#Copilot`, `#service-outage`

---