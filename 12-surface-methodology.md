# The 12-Surface AI Visibility Framework
### Dark Horse Strategies · Full Methodology

This document provides the complete scoring rubric, root cause diagnostics, and fix recommendations for each of the 12 AI visibility surfaces. It is the analytical backbone of the Dark Horse AI GTM Visibility Audit.

---

## How to use this document

1. Run the 25 LLM audit prompts in `/prompts/25-llm-audit-prompts.md`
2. Score each surface using the rubrics below (1–10)
3. Identify your Tier 3 surfaces — these are your highest-priority gaps
4. Use the "Fix" section for each surface to build your 90-day activation plan

---

## Surface 1: AI Interfaces (LLMs and Copilots)

**Platforms:** ChatGPT · Perplexity · Gemini · Claude · Microsoft Copilot · Google AI Mode

**What drives citation here:**
LLMs generate recommendations from their training corpus — a weighted blend of editorial content, Wikipedia, Reddit, structured web pages, and high-authority publications. Paid placement has no effect. What matters is citation density across trusted source types.

The single strongest predictor of LLM appearance is **brand search volume** (per Semrush's November 2025 study) — meaning brands that people actively search for are more likely to appear in LLM answers. The second strongest is cross-platform entity presence.

**Scoring rubric:**
- 8–10: Appears consistently in top 3 positions across multiple LLMs for primary category queries
- 5–7: Appears in some LLMs for branded queries but not category queries, or appears inconsistently
- 2–4: Appears only when brand name is included in the query
- 0–1: Does not appear in LLM responses even for branded queries

**Root causes of low scores:**
- Insufficient editorial coverage in high-authority publications
- No Wikipedia entity (removes a primary LLM citation source)
- Low Reddit mention volume (Reddit = 46.7% of Perplexity's top citations)
- Owned content not structured for LLM extraction

**Fix:** Earn coverage in high-DA publications. Build Wikipedia entity. Activate Reddit presence. Build answer-object pages on owned site.

---

## Surface 2: Search + AI-Augmented Search

**Platforms:** Google Organic · Bing · Google AI Overviews · Bing Copilot Search · Perplexity Search Mode

**What drives citation here:**
Google AI Overviews pull from the top 3 organic results for a query. The content format that performs best opens with a declarative summary paragraph directly answering the query, followed by FAQ-structured detail. This format — sometimes called an "answer object" — is the unit of content that AI Overviews extract and cite.

Bing Copilot Search weights Microsoft-ecosystem signals more heavily: Bing Places, Microsoft Advertising, and LinkedIn data all feed into Copilot recommendations.

**Scoring rubric:**
- 8–10: Appears in Google AI Overviews for primary non-branded category queries; ranks page 1 for multiple ICP-relevant queries
- 5–7: Ranks well for branded queries; appears in AI Overviews inconsistently or only for narrow queries
- 2–4: Ranks page 1 only for exact brand name queries; absent from AI Overviews
- 0–1: Does not rank page 1 even for branded queries; invisible in AI Overviews

**Root causes of low scores:**
- Practice/service pages don't open with declarative summary paragraphs
- No FAQ schema markup on key pages
- CMS blocks crawler access (JavaScript-heavy SPAs, crawl delays)
- Content targets solution-first language while buyers search problem-first

**Fix:** Restructure service pages with declarative openings and FAQ schema. Conduct problem-first keyword research. Audit robots.txt and crawler access.

---

## Surface 3: Review and Reputation Platforms

**Platforms:** G2 · Clutch · Capterra · UpCity · Glassdoor · Google Business Profile · PRovoke/O'Dwyer's (for agencies)

**What drives citation here:**
Review platforms are among the most-cited sources in ChatGPT for service firm recommendation queries. G2 and Clutch appear in 8–12% of B2B service category LLM citations. Critically, LLMs don't just cite that reviews exist — they extract the **language** of reviews. A review that says "their cybersecurity PR team helped us secure coverage in Dark Reading" trains the LLM to associate that brand with cybersecurity PR.

This means review generation strategy must be content strategy: the words reviewers use directly shape how LLMs describe your brand.

**Scoring rubric:**
- 8–10: 25+ reviews across 2+ platforms; vertical-specific tags; reviews contain outcome language and service-specific terminology
- 5–7: 10–25 reviews; present on primary platform; limited vertical tagging
- 2–4: Under 10 reviews; single platform; generic language in reviews
- 0–1: No reviews or profile claimed on major platforms

**Root causes of low scores:**
- No systematic review generation process
- Reviews exist but use generic relationship language ("great to work with") instead of outcome and service language
- Profile not tagged to specific verticals/categories
- Bliss-type acquisitions where review equity is locked to the acquired brand

**Fix:** Build a review generation workflow. Coach reviewers to include: (1) specific service category named, (2) industry/vertical context, (3) measurable business outcome. Prioritize Clutch for B2B services; G2 for any brand with a product component.

---

## Surface 4: Earned Media and Publisher Ecosystems

**Platforms:** Trade press · Business press (WSJ, Forbes, FT) · Vertical trades · Analyst reports (Gartner, Forrester, IDC)

**What drives citation here:**
Earned media is the single highest-weight input to LLM training data for brand visibility. Forbes holds 6.93% of ChatGPT citations (Semrush 2025). PR Newswire reaches 4.72% of ChatGPT citations but only for editorial-style content, not wire releases. Trade publications in a brand's specific vertical are heavily weighted for category queries.

The critical insight: **frequency of citation in high-authority publications compounds**. A brand mentioned in 50 articles across Forbes, TechCrunch, and relevant trade publications will appear in LLM answers even without any deliberate AEO strategy. Conversely, a brand with strong owned content but weak earned media will struggle to appear in category queries.

**Scoring rubric:**
- 8–10: Regular coverage in top-tier business press + vertical trades; named in analyst reports; O'Dwyer's/PRovoke listed at high tier
- 5–7: Regular trade press coverage; occasional business press; some vertical trades
- 2–4: Primarily press release coverage; occasional trade mentions
- 0–1: No meaningful editorial coverage; wire releases only

**Root causes of low scores:**
- PR strategy focused on announcements rather than thought leadership/bylines
- Coverage exists in wrong publications (low DA, not LLM training sources)
- Acquired brand's press coverage not migrated to acquirer's brand
- New vertical claims not backed by editorial presence in those vertical's trades

**Fix:** Map your buyer's publication list. Earn bylines and thought leadership placements there first. Treat analyst relations as an LLM citation strategy, not just a sales enablement play.

---

## Surface 5: Owned Content and Website Structure

**Platforms:** Brand website · Blog/insights hub · Landing pages · Schema markup layer

**What drives citation here:**
LLMs and AI search agents extract content from owned sites during retrieval. The content format that performs best:
1. Opens with a declarative statement directly answering a buyer query
2. Uses FAQ schema (JSON-LD) so search engines can extract individual Q&A pairs
3. Includes structured data markup (Organization, Article, FAQPage schemas)
4. Uses problem-first language that matches how buyers phrase queries to AI systems

The most common gap: brands write about themselves ("We are a leader in X") rather than writing answer-objects ("X is a [category] that helps [buyer type] achieve [outcome] by [mechanism]").

**Scoring rubric:**
- 8–10: Answer-object pages for all primary categories/practices; FAQ schema sitewide; Organization schema; regular publishing cadence with declarative openings
- 5–7: Good content depth; inconsistent structure; some schema; regular publishing
- 2–4: Content exists but not structured for AI extraction; minimal schema; publishing cadence irregular
- 0–1: Thin content; no schema; JavaScript-blocked crawling; no publishing cadence

**Root causes of low scores:**
- Service/practice pages written as brand marketing copy, not answer-objects
- No FAQ schema deployment
- CMS architecture blocks crawlers (Wix SPA issue is common)
- Solution-first language instead of problem-first language

**Fix:** Audit your 10 highest-traffic pages. Rewrite the opening paragraph of each as a direct, declarative answer to the buyer query that would logically land on that page. Add FAQ schema. This single change can move Google AI Overview appearance within 30–60 days.

---

## Surface 6: Technical and Developer Surfaces

**Platforms:** GitHub · dev.to · Stack Overflow · Hacker News · HuggingFace · API documentation platforms

**What drives citation here:**
Developer surfaces are crawled heavily by LLMs and are particularly high-weight for queries from technical buyers. A GitHub README is not just a documentation page — it is a structured, crawlable, citable document that LLMs treat as authoritative on technical topics. Dev.to posts are indexed by Google and crawled by Perplexity; a high-quality dev.to post on a B2B GTM topic will surface in AI answers within weeks of publication.

**This surface is uniformly underexploited by B2B services firms.** Most agencies and consultancies have zero GitHub or dev.to presence — meaning any brand that publishes substantive content there faces essentially no competition for LLM citations on those platforms.

**Scoring rubric:**
- 8–10: Active GitHub org with starred repositories; regular dev.to/HN posts; cited in developer community discussions
- 5–7: Some developer surface presence; GitHub exists but sparse; occasional community posts
- 2–4: Minimal presence; perhaps one old repository or a few community comments
- 0–1: No developer surface presence at all (the default for most B2B services firms)

**Root causes of low scores:**
- Not perceived as a technical brand
- No framework, tool, or methodology published in a developer-native format
- Underestimation of how heavily LLMs weight developer content sources

**Fix:** Publish a structured framework or methodology on GitHub. Write one dev.to post that explains your core approach for a technical-adjacent audience. Submit a "Show HN" post. This surface has the lowest competitive bar of all 12 — the time investment is small relative to the LLM citation gain.

---

## Surface 7: Social and Authority Signals

**Platforms:** LinkedIn (company + executive) · Twitter/X · Podcast appearances · Conference speaking · Award citations

**What drives citation here:**
LinkedIn reaches 15% of Google AI Mode citations and 5%+ of ChatGPT citations (Semrush November 2025). Executive-level LinkedIn publishing is one of the fastest controllable levers for LLM visibility — because LinkedIn content is crawled actively and the platform's authority signals are highly weighted.

Award citations are LLM training signals: a brand cited as "PRWeek Agency of the Year" or "Gartner Magic Quadrant Leader" will have those credentials appear in LLM descriptions of that brand for 12–24 months after the award.

**Scoring rubric:**
- 8–10: CEO publishes 3+ times/week with vertical positioning language; 50K+ LinkedIn followers; major award citations in past 24 months; conference speaking record
- 5–7: CEO publishes 1–2 times/week; 10–50K followers; some awards; occasional speaking
- 2–4: Company page active; executive publishing infrequent; no major award citations
- 0–1: Minimal social presence; inactive or absent executive voices

**Root causes of low scores:**
- CEO/founder doesn't publish or publishes without category-positioning language
- Award wins not referenced in company bio, website, or press releases
- LinkedIn follower count too low to drive meaningful citation signal
- Post-acquisition brand transition not reflected in executive social profiles

**Fix:** The executive LinkedIn publishing frequency gap is the fastest fix available. Three posts per week from the CEO, written with explicit vertical and category positioning language, will move LLM visibility within 60–90 days.

---

## Surface 8: Data Aggregators and Knowledge Graphs

**Platforms:** Wikipedia · Wikidata · Google Knowledge Graph · Crunchbase · ZoomInfo · Apollo · D&B

**What drives citation here:**
Wikipedia is among the top 3 sources cited by ChatGPT. A Wikipedia entity entry is the single most impactful individual action a brand can take for LLM visibility — it creates a structured, authoritative, multi-platform entity definition that LLMs draw from directly. Wikidata (Wikipedia's structured data layer) feeds Google's Knowledge Graph, which feeds Google AI Overviews.

B2B data platforms (ZoomInfo, Apollo, D&B) are crawled by LLMs for company research queries. The categories, descriptions, and service taxonomies listed on these platforms appear in AI-generated company research summaries.

**Scoring rubric:**
- 8–10: Wikipedia entry exists and is current; Wikidata entity linked; Google Knowledge Panel active; B2B data platforms accurate and fully categorized
- 5–7: No Wikipedia but Knowledge Panel partially active; B2B data platforms accurate; Crunchbase complete
- 2–4: No Wikipedia; partial Knowledge Panel; B2B data platforms have stale or incomplete data
- 0–1: No Wikipedia; no Knowledge Panel; B2B data platforms missing or inaccurate

**Root causes of low scores:**
- Company not perceived as Wikipedia-notable (often incorrect — many companies meet notability thresholds)
- No one has drafted the entry
- B2B data platform profiles not maintained post-acquisition or post-rebrand

**Fix:** Assess Wikipedia notability (criteria: coverage in multiple independent reliable sources). If criteria are met, draft an entry. This is a one-time investment with permanent LLM citation return. Then update all B2B data platform profiles with current descriptions, service taxonomies, and category tags.

---

## Surface 9: Marketplaces and Ecosystems

**Platforms:** Clutch category pages · Agency Spotter · The Manifest · UpCity · HubSpot Agency Directory · Salesforce AppExchange

**What drives citation here:**
Marketplace category pages are among the most-crawled content for "[category] company" queries. Clutch's "Top PR Agencies" category page, for example, is cited in AI answers to "best PR agency" queries more frequently than most individual agency websites. Being listed with full vertical tags and complete descriptions on these pages is a citation-building strategy, not just a lead gen play.

**Scoring rubric:**
- 8–10: Listed on all major relevant marketplaces; full vertical/service tags; complete descriptions; featured or top-listed status
- 5–7: Listed on primary marketplace (Clutch); partial vertical tags; incomplete descriptions on secondary platforms
- 2–4: Listed but thin; missing vertical tags; absent from 2+ relevant platforms
- 0–1: Not listed on major marketplaces or profiles unclaimed

**Root causes of low scores:**
- Profiles created but never optimized
- Missing vertical/category tags that LLMs use for category queries
- Secondary marketplaces (Agency Spotter, UpCity) not prioritized
- HubSpot / Salesforce ecosystem directories ignored despite high LLM citation weight for integrated marketing queries

**Fix:** Complete all marketplace profiles with full service and vertical taxonomy. Prioritize the tags — they are the literal words LLMs use when categorizing your brand for buyer queries.

---

## Surface 10: Case Studies and Proof Layers

**Platforms:** Owned case study pages · Award submission archives · Conference presentation recordings · Third-party success story features

**What drives citation here:**
LLMs cite case studies when answering "which company has experience with X" queries. The format that performs best is outcome-first: problem → approach → measurable result → client context. A case study that says "reduced cost per lead by 43% for a Series B cybersecurity company" trains the LLM to associate that brand with cybersecurity demand generation.

Award wins are a specific proof layer subtype: a brand cited as the winner of a named, prestigious award will have that credential appear in LLM descriptions for 12–24 months.

**Scoring rubric:**
- 8–10: 10+ published case studies with outcome metrics; multiple award citations; vertical-specific proof across all practice areas
- 5–7: 3–10 case studies; some award citations; proof concentrated in 1–2 verticals
- 2–4: Under 3 case studies; awards mentioned but not structured as extractable proof points
- 0–1: No published case studies; no award-based proof layer

**Root causes of low scores:**
- Case studies written as narrative stories rather than structured outcome documents
- Award wins not published on owned site in extractable format
- Acquired brand's proof layer not migrated to acquirer's brand
- Client confidentiality concerns preventing named case study publication

**Fix:** Adopt a structured case study format: headline (outcome) → client context → challenge → approach → result (with metric). Add FAQ schema. Even 3–5 case studies in this format will outperform 20 narrative case studies for LLM citation purposes.

---

## Surface 11: Community and Q&A Platforms

**Platforms:** Reddit · Quora · LinkedIn groups · Slack communities · Discord servers · PRSA/IABC/other professional forums

**What drives citation here:**
Reddit is the #2 LLM citation source after Wikipedia, comprising 46.7% of Perplexity's top citations and significant ChatGPT training data. A single high-voted comment in a relevant Reddit thread recommending your brand can drive more LLM citation value than a press release. This is because LLMs weight community-validated content (upvotes, replies, engagement) as a signal of trustworthiness.

Quora answers are similarly crawled and cited, particularly for definitional and recommendation queries.

**Scoring rubric:**
- 8–10: Regular authentic participation in relevant subreddits; multiple high-voted brand mentions; active Quora presence; cited in LinkedIn group discussions
- 5–7: Some Reddit presence; occasional Quora answers; community presence but not systematic
- 2–4: Rare mentions; no active participation; brand appears only when directly asked about
- 0–1: No community presence; brand not mentioned in relevant community discussions

**Root causes of low scores:**
- Not perceived as a platform where the brand belongs (incorrect)
- Fear of appearing promotional (solvable through authentic participation)
- No designated team members responsible for community engagement
- Underestimation of Reddit's LLM citation weight

**Fix:** Identify the 3–5 subreddits most active among your ICP. Designate 2 team members to participate authentically in discussions — answering questions helpfully, sharing insights, being genuinely useful. The goal is not to promote; it's to be cited. Helpful, high-voted comments generate more LLM citation value than any promotional post.

---

## Surface 12: Enterprise and Private AI Environments

**Platforms:** Microsoft 365 Copilot · Salesforce Einstein · Perplexity Teams · Custom enterprise GPTs · AI-augmented RFP tools

**What drives citation here:**
Enterprise AI tools draw from the same public citation sources as consumer LLMs — primarily surfaces 1–11. The brand that wins surfaces 1–11 will win surface 12 automatically. However, there are surface-12-specific signals worth noting: LinkedIn data is a primary source for Copilot company research; Salesforce Einstein draws from Salesforce's own CRM data ecosystem; Perplexity Teams allows enterprise users to set custom source preferences.

**Scoring rubric:**
- 8–10: Strong presence on surfaces 1–11; brand appears in enterprise AI research workflows; documented integration with enterprise AI tooling
- 5–7: Moderate surface 1–11 presence; enterprise AI appearance inconsistent
- 2–4: Weak 1–11 foundation; enterprise AI appearance rare
- 0–1: Near-absent across 1–11; effectively invisible in enterprise AI environments

**Root causes of low scores:**
- This surface is a lagging indicator of performance on surfaces 1–11
- LinkedIn company data incomplete or not current (direct Copilot input)
- No Perplexity-optimized content (structured, citation-dense, updated regularly)

**Fix:** This surface cannot be improved directly — it is improved by improving surfaces 1–11. The one exception: ensure LinkedIn company data is complete and current, as it is a direct input to Microsoft 365 Copilot recommendations.

---

## Aggregating your scores

Once you've scored all 12 surfaces:

1. Calculate your average score (sum / 12)
2. Identify your Tier 3 surfaces (scored 1–3) — these are your 90-day priorities
3. Identify your Tier 2 surfaces (scored 4–6) — these are your 6-month investment areas
4. Protect your Tier 1 surfaces (scored 7–10) — don't let these decay

**Grade scale:**
- A (8.5–10): Category-defining AI visibility — you appear consistently across all major surfaces
- B (7–8.4): Strong foundation — a few surfaces need attention but core presence is solid
- C (5–6.9): Moderate — visible in some contexts but missing critical surfaces
- D (3–4.9): Weak — appearing primarily for branded queries; invisible for category queries
- F (0–2.9): Near-absent — effectively invisible in AI-mediated buying environments

---

*Part of the [Dark Horse Strategies AI GTM Visibility Framework](https://github.com/darkhorsestrategies/ai-gtm-visibility-framework)*
*→ [darkhorsecapabilities.lovable.app](https://darkhorsecapabilities.lovable.app)*

*Last updated: June 2026*
