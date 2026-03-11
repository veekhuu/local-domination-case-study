# Phase 3: Intelligence Gathering Prompts

← [Previous: Scrollytelling](./scrollytelling.md) | **Documentation:** [docs/03-intelligence.md](../docs/03-intelligence.md)

> **Note:** These prompts are reconstructed approximations of the prompts used during the project. They capture the intent and structure of the originals but may not be word-for-word matches.

---

## 1. Manus Pass 1: Competitive Analysis

**Target:** Manus AI

```
Here are [NUMBER] competitors in the [INDUSTRY] space in [TARGET MARKET]. They all rank on page 1 of Google for various key terms:

1. [COMPETITOR 1 URL]
2. [COMPETITOR 2 URL]
...
10. [COMPETITOR 10 URL]

Using SimilarWeb data, analyze all of them and give me:

1. **Traffic analysis**: Monthly visits, traffic sources, top pages
2. **Keyword rankings**: What keywords each competitor ranks for
3. **Strengths**: What they're doing right that we need to match
4. **Weaknesses**: What they're doing wrong that we can exploit
5. **Content gaps**: Topics or services they don't cover
6. **Technical assessment**: Site speed, mobile optimization, structured data

For each competitor, I need to understand:
- Their Google review count and rating
- Their website's perceived authority
- Their strongest performing pages

Organize this as a competitive matrix I can use for planning.
```

---

## 2. Manus Pass 2: Customer Sentiment

**Target:** Manus AI

```
Go to every review page you can find for these [NUMBER] competitors in [INDUSTRY] in [TARGET MARKET]:

1. [COMPETITOR 1]
2. [COMPETITOR 2]
...
5. [COMPETITOR 5]

Search Google Reviews, Yelp, BBB, Houzz, Angi, and any other review platforms.

Give me:
1. **Top 5 complaints** customers have about these companies (with specific examples)
2. **Top 5 things** customers praise about these companies
3. **Service gaps**: Things these companies don't offer that customers wish they did
4. **Pricing complaints**: What customers say about pricing, estimates, and value
5. **Wildcard**: Two additional findings that you think are interesting or actionable from the research — I'll let you decide what's worth highlighting

This is for competitive positioning. I want to know exactly what customers love and hate so we can position our company to address the pain points and match the praise points.
```

---

## 3. Manus Pass 3: SEO/AEO Research

**Target:** Manus AI

```
Research the latest best practices for SEO and AEO (Answer Engine Optimization) for [INDUSTRY] websites.

Find and analyze content from 5-7 top experts in SEO and AEO. Look at:
- Their blog posts and guides
- YouTube transcripts
- Conference presentations
- Documentation from Google about content quality

I also want you to review these specific resources:
[PASTE ANY YOUTUBE TRANSCRIPT URLs OR GOOGLE DOCUMENTATION LINKS]

Give me actionable recommendations for:
1. How to structure content so it ranks on Google AND gets cited by AI tools (ChatGPT, Perplexity, Claude)
2. Content formatting best practices (headers, schema, FAQ sections)
3. Internal linking strategy
4. How to write content that AI models want to reference
5. The difference between optimizing for traditional search vs. AI search
```

---

## 4. Claude + Tavily Gap Analysis

**Target:** Claude with Tavily Search + Perplexity MCP

```
I need you to search for and analyze the services that our competitors offer compared to what our company ([COMPANY NAME]) offers.

Our company provides these services:
- [SERVICE 1]
- [SERVICE 2]
...

Search for our top competitors in [TARGET MARKET] and find:
1. Services they offer that we also offer (confirm competitive parity)
2. Services they offer that we DON'T offer (potential gaps)
3. Services we offer that they DON'T (competitive advantages)
4. Unique value propositions each competitor uses
5. Pricing models or approaches mentioned publicly

Use Tavily and Perplexity to search for this information across their websites, reviews, and social media.
```

---

## 5. Keyword Research

**Target:** Claude Code / Gemini

```
Generate 100 target keywords for a [INDUSTRY] company in [TARGET MARKET] that offers these services:
- [SERVICE 1]
- [SERVICE 2]
...

Across these cities/areas:
- [CITY 1]
- [CITY 2]
...

Organize the keywords by:
1. **Difficulty to rank** (easy/medium/hard based on competition)
2. **Commercial value** (how much buying intent the searcher has: informational/commercial/transactional)
3. **Target page** (which page on our site should target this keyword)
4. **Category**:
   - Problem-based searches (e.g., "[PROBLEM] in [CITY]")
   - Service-specific searches (e.g., "[SERVICE] [CITY]")
   - Location combinations (e.g., "[SERVICE] near [NEIGHBORHOOD]")
   - Commercial intent (e.g., "[SERVICE] cost [CITY]", "best [SERVICE] [CITY]")

Note: These estimates are Claude's best guess. For more accurate data, use Gemini (which has access to Google's search data) or set up Keywords Everywhere MCP.
```

---

← [Previous: Scrollytelling](./scrollytelling.md) | [Next: Content Prompts →](./content.md)
