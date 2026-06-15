# ai-gtm-visibility-framework
Audit brand visibility in across the 12 AI-mediated buying surfaces
### by Dark Horse Strategies

**The AI filter that now sits atop every B2B go-to-market strategy — and how to audit it.**

---

Most B2B GTM strategies were built for a world where buyers started with a Google search. That world is over.

In 2026, a growing share of B2B purchase research begins with a question typed into ChatGPT, Perplexity, Gemini, or Microsoft Copilot. The brands that appear in those answers get evaluated. The brands that don't are invisible — not because they lack a product, but because they lack presence on the surfaces that AI systems draw from when generating recommendations.

This repository contains Dark Horse Strategies' open-source **AI GTM Visibility Framework**: a structured methodology for auditing, scoring, and improving a B2B brand's presence across the 12 surfaces that feed AI-generated answers. It is the analytical foundation behind our client work and is published here in full — because the problem is too important to gatekeep.

---

## What's in this repo

```
/framework          12-surface scoring rubric and methodology
/prompts            25 LLM audit prompts — run these yourself today
/surfaces           Deep-dive guides for each of the 12 surfaces
/examples           Sanitized audit examples from real engagements
/templates          Scoring worksheets and report templates
```

---

## The core insight: AI mediation changes GTM math

Traditional GTM assumes a linear funnel: awareness → consideration → decision. AI mediation collapses this. When a buyer asks an LLM "what's the best [category] solution for [use case]," the model returns a shortlist — and that shortlist is the new awareness layer. If your brand isn't in it, you don't exist for that buyer at that moment.

The LLM shortlist is not random. It is a function of **citation density** — how frequently and authoritatively your brand appears across the sources that AI systems draw from during training and retrieval. Those sources are specific, observable, and actionable. That's what this framework maps.

---

## The 12 AI Visibility Surfaces

Each surface represents a distinct channel through which AI systems discover, learn about, and cite B2B brands. Performance varies dramatically by surface — a brand can be strong on one and invisible on eleven others.

| # | Surface | What AI draws from here |
|---|---|---|
| 1 | **AI Interfaces** | LLM training corpus — editorial coverage, Wikipedia, Reddit, structured web content |
| 2 | **Search + AI-Augmented Search** | Google AI Overviews, Bing Copilot, Perplexity Search — pulls from top organic results |
| 3 | **Review + Reputation Platforms** | G2, Clutch, Capterra, industry-specific review sites — heavily cited in "best X" queries |
| 4 | **Earned Media + Publisher Ecosystems** | Trade press, business press, analyst reports — the highest-weight training signal |
| 5 | **Owned Content + Website Structure** | Answer-object pages, FAQ schema, AEO-structured content on owned domains |
| 6 | **Technical + Developer Surfaces** | GitHub, dev.to, Stack Overflow, HN — high LLM citation weight for technical queries |
| 7 | **Social + Authority Signals** | LinkedIn (15% of Google AI Mode citations), executive publishing, award citations |
| 8 | **Data Aggregators + Knowledge Graphs** | Wikipedia, Wikidata, Google Knowledge Graph, Crunchbase, ZoomInfo |
| 9 | **Marketplaces + Ecosystems** | Clutch category pages, Agency Spotter, HubSpot Partner Directory, G2 categories |
| 10 | **Case Studies + Proof Layers** | Published case studies, award entries, client-named outcomes — cited in capability queries |
| 11 | **Community + Q&A Platforms** | Reddit (#2 LLM citation source), Quora, LinkedIn groups, Slack communities |
| 12 | **Enterprise + Private AI Environments** | Microsoft 365 Copilot, Salesforce Einstein, Perplexity Teams — fed by surfaces 1–11 |

---

## Scoring methodology

Each surface is scored on a **1–10 scale** across three dimensions:

| Dimension | What it measures |
|---|---|
| **Presence** | Does the brand appear on this surface at all? |
| **Depth** | Is the content substantive enough to be cited — or just a listing? |
| **Recency** | Is the content recent enough to be in active training/retrieval cycles? |

**Tier definitions:**
- **Tier 1 (7–10):** Strong — consistently cited; content is current and substantive
- **Tier 2 (4–6):** Moderate — present but shallow, stale, or narrowly scoped
- **Tier 3 (1–3):** Weak/Absent — not appearing in AI-generated answers for relevant queries

**Overall grade:**
Average across all 12 surfaces, weighted by relevance to the brand's primary buyer queries.

---

## How to run a quick audit on your own brand (15 minutes)

See [`/prompts/25-llm-audit-prompts.md`](./prompts/25-llm-audit-prompts.md) for the full prompt library.

**Quick start — run these 5 prompts right now:**

1. Open ChatGPT, Perplexity, and Gemini in separate tabs
2. In each, run: `"What are the best [your category] companies for [your ICP]?"`
3. Note whether your brand appears, at what position, and what language is used to describe it
4. Run: `"What should I look for when evaluating [your category] vendors?"`
5. Run: `"Compare [your brand] with [top competitor]"`

If your brand doesn't appear in responses 1–2, you have a Surface 1 gap. If it appears but the description is wrong or stale, you have a Surface 5 (owned content) or Surface 8 (knowledge graph) gap. The `/framework` directory maps every scenario to a root cause and a fix.

---

## The GTM reframe

Traditional GTM recommendation → **AI-mediated GTM recommendation**

| Traditional | AI-Mediated |
|---|---|
| SEO → rank for keywords | AEO/GEO → get cited in AI-generated answers |
| PR → earn media coverage | PR + Citation Engineering → structure coverage for LLM extraction |
| Review generation → star ratings | Review generation + taxonomy tagging → LLM-citable category signals |
| Thought leadership → LinkedIn posts | Thought leadership + Answer-object pages → LLM training signal |
| Analyst relations → Gartner mentions | Analyst relations + Wikipedia entity → Knowledge graph presence |
| Demand gen → paid + content | Demand gen → AI surface presence first, then paid amplification |

The AI filter doesn't replace traditional GTM. It sits on top of it. Every channel you already invest in has an AI-mediated version — and the brands that understand the difference are the ones appearing in shortlists.

---

## About Dark Horse Strategies

Dark Horse Strategies is an AI-native B2B GTM consultancy. We help B2B brands understand and improve their presence in AI-mediated buying environments — and rebuild their GTM motions around the AI filter that now sits atop every channel.

Our productized offerings include the AI Signal Sprint, AI Visibility Audit, AI Mediation Playbook, and Portfolio AI Mediation Playbook (for PE/VC firms auditing multiple portfolio companies simultaneously).

**→ [darkhorsecapabilities.lovable.app](https://darkhorsecapabilities.lovable.app)**
**→ [darkhorsestrategies.com](https://darkhorsestrategies.com)**

---

## Contributing

This framework is a living document. If you work in B2B GTM, AI/ML, or marketing technology and want to contribute surface definitions, prompt additions, or scored examples:

1. Fork this repo
2. Add your contribution to the relevant `/surfaces` or `/prompts` file
3. Open a pull request with a one-paragraph description of what you observed and why it matters

Contributions that include real observed data (which LLMs cited what, under what query conditions) are especially valuable.

---

## License

MIT. Use freely. Attribution appreciated but not required.

---

*Last updated: June 2026 | Dark Horse Strategies*
