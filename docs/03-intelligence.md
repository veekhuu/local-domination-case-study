← [Previous: Scrollytelling](./02-scrollytelling.md) | [Next: Site Skeleton →](./04-site-skeleton.md)

# Phase 3: Intelligence Gathering

**Time:** Day 2
**Tools:** Manus AI (+ SimilarWeb), Claude + Tavily Search + Perplexity MCP, Claude Code
**Cost:** ~10,000 Manus credits
**Prompts for this phase:** [prompts/intelligence.md](../prompts/intelligence.md)

---

```
INTELLIGENCE GATHERING — FOUR PARALLEL RESEARCH FRONTS
═══════════════════════════════════════════════════════════════

  ┌─────────────────────────────────────────────────────────┐
  │                     RESEARCH INPUTS                      │
  └────┬──────────┬──────────────┬─────────────┬────────────┘
       │          │              │             │
       ▼          ▼              ▼             ▼
  ┌─────────┐ ┌──────────┐ ┌──────────┐ ┌──────────────┐
  │ MANUS   │ │ MANUS    │ │ MANUS    │ │ CLAUDE +     │
  │ PASS 1  │ │ PASS 2   │ │ PASS 3   │ │ TAVILY +     │
  │         │ │          │ │          │ │ PERPLEXITY   │
  │Competi- │ │Customer  │ │SEO/AEO   │ │              │
  │tive     │ │Sentiment │ │Research  │ │ Gap          │
  │Analysis │ │Mining    │ │          │ │ Analysis     │
  │         │ │          │ │          │ │              │
  │10 comp- │ │5 compet- │ │5-7 SEO   │ │ Service      │
  │etitors  │ │itors     │ │experts   │ │ comparison   │
  │via      │ │reviews   │ │+ YouTube │ │ vs. ours     │
  │Similar- │ │across    │ │+ Google  │ │              │
  │Web      │ │all plat- │ │docs      │ │              │
  │         │ │forms     │ │          │ │              │
  │~3K      │ │          │ │          │ │              │
  │credits  │ │          │ │          │ │              │
  └────┬────┘ └────┬─────┘ └────┬─────┘ └──────┬───────┘
       │          │              │             │
       ▼          ▼              ▼             ▼
  ┌─────────────────────────────────────────────────────────┐
  │                   RESEARCH OUTPUTS                       │
  │                                                          │
  │  ◦ Competitive matrix (traffic, keywords, strengths)    │
  │  ◦ Customer complaints + praise + service gaps          │
  │  ◦ SEO/AEO best practices                              │
  │  ◦ 100+ target keywords (organized by difficulty)       │
  │  ◦ Service gap analysis                                 │
  └────────────────────────┬────────────────────────────────┘
                           │
                           ▼
                  ┌──────────────────┐
                  │  KEYWORD          │
                  │  RESEARCH         │
                  │                   │
                  │  Claude Code      │
                  │  100 keywords     │
                  │  organized by:    │
                  │  ◦ Difficulty     │
                  │  ◦ Commercial val │
                  │  ◦ Target page    │
                  │  ◦ Search type    │
                  └──────────────────┘

  TOTAL COST: ~10,000 Manus AI credits
```

---

## The Shift: From Website to Weapon

> "This is where the project went from 'building a website' to 'building a weapon.'"

Up to this point, the project had a plan and a hero section. But Day 2 is where everything changed. Instead of guessing what content to write, what keywords to target, or what services to emphasize, the approach was to go on a full-scale research blitz. Multiple fronts, all at once.

The intelligence gathered in this phase informed every decision that followed -- from page copy to site architecture to content strategy. Without it, the website would have been built on assumptions. With it, every page was built on data.

## Manus Pass 1: Competitive Analysis with Real Data (~3,000 credits)

The first research pass focused on understanding the competitive landscape with hard numbers, not guesses.

**Why Manus AI specifically?** Because it has access to **SimilarWeb**, which provides actual traffic data, keyword rankings, and competitive metrics that are not available through standard browsing or free tools.

**The process:**

1. Compiled a list of approximately **10 competitors** from page 1 of Google for [PRIMARY KEYWORD / SERVICE + LOCATION]
2. Fed the list to Manus with clear instructions: analyze them all
3. For each competitor, Manus gathered:
   - **Traffic numbers** -- how many monthly visitors they get
   - **Top keywords** -- what search terms drive their traffic
   - **Strengths** -- what they do well (design, content depth, local SEO)
   - **Weaknesses** -- where they fall short (thin content, slow sites, missing services)
   - **Top-performing pages** -- which specific pages drive the most organic traffic

**Output:** A competitive matrix showing Google review counts, website strength assessments, and a clear picture of what it would take to compete.

**Simultaneously**, Claude was used with the **Tavily search tool** and **Perplexity MCP** to run a parallel gap analysis -- comparing competitor service offerings against [YOUR COMPANY]'s services to identify gaps and opportunities that the competitive data alone might miss.

This first pass consumed approximately **3,000 Manus credits**.

## Manus Pass 2: Customer Sentiment Mining

The second Manus pass was completely separate from the first, with a fundamentally different objective: understanding what customers actually think.

Manus was sent to scrape and analyze review pages for **[NUMBER, e.g., 5] major competitors** across all review platforms (Google, Yelp, BBB, Houzz, etc.).

**Five specific deliverables were requested:**

1. **Top 5 customer complaints** -- with specific examples and quotes from actual reviews
2. **Top 5 things customers praise** -- what people love and mention repeatedly
3. **Service gaps** -- things customers want that competitors do not offer
4. **Pricing complaints** -- how customers feel about pricing, hidden fees, estimate accuracy
5. **Wildcard** -- two additional AI-chosen findings that did not fit the categories above

The wildcard category is intentionally open-ended. It lets the AI surface patterns you did not think to ask about.

> "I'm not going to tell you what the wildcard findings were, because what Manus discovers for your competitors and your market will be different than what it found for mine."

This intelligence directly shaped the website's messaging. When you know exactly what customers complain about with your competitors, you can address those pain points proactively on your own site.

## Keyword Research (~100 keywords)

While Manus handled the competitor and sentiment research, **Claude Code** was tasked with generating a comprehensive keyword list.

The output: approximately **100 target keywords**, organized across multiple dimensions:

| Dimension | Description | Example |
|---|---|---|
| **Difficulty** | How hard to rank (easy / medium / hard) | [EASY KEYWORD EXAMPLE] |
| **Commercial value** | Level of buying intent | [HIGH INTENT KEYWORD EXAMPLE] |
| **Target page** | Which page on the site should rank for it | Service page, location page, blog post |
| **Problem-based** | Searches framed as problems | "[PROBLEM] + [LOCATION]" |
| **Service-specific** | Searches for specific services | "[SERVICE] + near me" |
| **Location combinations** | Service + city/area pairings | "[SERVICE] + [CITY]" |

**Important caveat:** These were Claude's best guesses based on its training data. For more accurate search volume and difficulty data, supplement with:

- **Gemini** -- has access to Google's actual search data
- **Keywords Everywhere MCP** -- provides real-time search volume, CPC, and competition metrics

The keyword list served as a starting framework that was refined with real data later.

## Manus Pass 3: SEO/AEO Best Practices Research

The third and final Manus pass shifted focus from competitors to experts.

**Objective:** Understand the current best practices for both traditional SEO and the emerging field of AEO (Answer Engine Optimization -- optimizing content to be cited by AI tools like ChatGPT, Perplexity, and Claude).

**Research targets:**

- **5-7 top SEO and AEO experts** -- their published guides, frameworks, and recommendations
- **YouTube transcripts** -- long-form video content from these experts, transcribed and analyzed
- **Google documentation** -- official guidelines on what Google rewards and penalizes

**Goal:** Build a clear understanding of how to format content so it:

1. **Ranks on Google** -- traditional SEO (headings, internal links, page speed, content depth)
2. **Gets cited by AI tools** -- AEO (structured answers, clear definitions, authoritative formatting)

The output from this pass became the content formatting template used across every page on the site. Instead of guessing how to structure content, every page followed a research-backed format.

## Total Investment

All three Manus passes combined consumed approximately **~10,000 Manus AI credits**.

For context, this level of competitive intelligence, customer research, keyword analysis, and SEO strategy would typically require:

- A marketing agency engagement ($3,000-$10,000+)
- Multiple weeks of manual research
- Subscriptions to SimilarWeb, Ahrefs, SEMrush, and other tools ($200-$500/month each)

> **Key insight:** Don't guess what to write. Research first. The intelligence gathering phase is what separates a website that ranks from one that just exists.

---

**Prompts for this phase:** [prompts/intelligence.md](../prompts/intelligence.md)

← [Previous: Scrollytelling](./02-scrollytelling.md) | [Next: Site Skeleton →](./04-site-skeleton.md)
