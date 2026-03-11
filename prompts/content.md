# Phase 4: Content at Scale Prompts

← [Previous: Intelligence](./intelligence.md) | **Documentation:** [docs/05-content-at-scale.md](../docs/05-content-at-scale.md)

> **Note:** These prompts are reconstructed approximations of the prompts used during the project. They capture the intent and structure of the originals but may not be word-for-word matches.

---

## 1. Research Feed Prompt

**Target:** Claude Code

```
Read all documents in the [RESEARCH FOLDER PATH]. These contain:
- Competitive analysis from Manus AI (SimilarWeb data on [NUMBER] competitors)
- Customer sentiment analysis (complaints, praise, service gaps)
- SEO/AEO best practices research
- Keyword research with 100+ target keywords
- Gap analysis between our services and competitors

After reading everything, update the build plan. We need to:
1. Match or exceed competitor coverage for all services
2. Address the top customer complaints in our content
3. Highlight our competitive advantages
4. Target keywords organized by difficulty and commercial value
5. Follow the SEO/AEO formatting best practices from the research
```

---

## 2. Blog Planning: Hub-and-Spoke

**Target:** Claude Code

```
From the keyword research list, plan out [NUMBER]+ blog articles organized into topic clusters using a hub-and-spoke format.

Rules:
- Each cluster has ONE hub page (broad topic) and multiple spoke pages (specific subtopics)
- Spoke pages link back to their hub page
- No two articles should target the same primary keyword (avoid keyword cannibalization)
- Each article needs a primary keyword, secondary keywords, and a target search intent
- Organize clusters by service area

DON'T write any articles yet. Just plan:
- Article titles
- Target keywords (primary + secondary)
- Which cluster each belongs to
- Internal linking map (hub → spokes, cross-cluster links)
- Publishing priority (which articles to write first based on keyword difficulty and commercial value)
```

---

## 3. Service Page Requirements

**Target:** Claude Code

```
Create detailed pages for each of our [NUMBER] services:
[LIST SERVICES]

Each service page must include:
1. **Service overview**: Detailed explanation of what the service is
2. **Our process**: Step-by-step breakdown of how we deliver this service
3. **Trust signals**: Credentials, experience, certifications, years in business
4. **Why choose us**: Competitive differentiation (reference the competitive analysis)
5. **FAQ section**: 5-8 frequently asked questions with detailed answers
6. **Service areas**: List of cities/neighborhoods we serve for this service
7. **Local information**: Area-specific details that help with local SEO
8. **CTA**: Clear call-to-action for consultation/quote

IMPORTANT: Research each service topic from reputable sources before writing. Content must be able to cite where information came from. No generic filler.
```

---

## 4. Location Page Requirements

**Target:** Claude Code

```
Create location pages for each of these [NUMBER] cities:
[LIST CITIES]

Each location page must include:
1. **Local service area details**: Neighborhoods, zip codes, service radius
2. **Local weather challenges**: How local climate affects [INDUSTRY] work (this is relevant for [INDUSTRY TYPE])
3. **Neighborhood-specific content**: Unique characteristics of the area
4. **Local regulations**: Permits, codes, or requirements specific to this city
5. **Service offerings**: Which of our services are available in this location
6. **Local trust signals**: Projects completed in this area, local reviews

IMPORTANT: Research each location from reputable sources. Include real local details, not generic content.

Implement ARIA attributes and follow WCAG 2.1 Level AA principles for accessibility.
```

---

## 5. Agent Team Orchestration

**Target:** Claude Code

```
I need you to organize agent teams to write all the content. Here's how to structure the work:

**Phase 1 — Outlines:**
Assign 4-5 agents. Each agent creates detailed outlines for their assigned pages (5-10 pages per agent). All agents return with completed outlines before moving to Phase 2.

**Phase 2 — Research:**
Same agents go out and research their topics from reputable sources using available search tools. Each piece of content must cite its sources. All agents return with research before Phase 3.

**Phase 3 — Writing:**
The main agent assigns 10 junior agents to write 10 pages simultaneously. Each agent follows the outline and incorporates the research. Quality requirements:
- Minimum [WORD COUNT] words per page
- Proper heading structure (H1 → H2 → H3)
- Internal links to related pages
- Schema-ready content structure
- Natural keyword integration (no stuffing)
- Unique, non-duplicative content across all pages

Run all three content tracks:
1. Service pages ([NUMBER] services)
2. Location pages ([NUMBER] cities)
3. Blog articles ([NUMBER]+ articles)
```

---

## 6. Copywriting Polish Prompt

**Target:** Claude Code

```
Review and polish the copywriting across the entire site using direct-response copywriting principles from these masters:

- **Dan Kennedy**: Magnetic headlines, urgency, direct response structure
- **Gary Halbert**: Conversational tone, story-driven copy, the "A-pile" test
- **Gary Bencivenga**: Proof-heavy copy, credibility building
- **David Ogilvy**: Research-backed claims, long-form that sells
- **Dr. Robert Cialdini**: Reciprocity, social proof, authority, scarcity, commitment, liking
- **Alex Hormozi**: Value stacking, irresistible offers, grand slam offers
- **Jim Edwards**: Copywriting frameworks, headline formulas, benefit-driven writing

For each page:
1. Strengthen the headline (make it specific, benefit-driven, and curiosity-inducing)
2. Add social proof elements where appropriate
3. Improve CTAs (make them action-oriented and specific)
4. Add urgency or scarcity where authentic
5. Ensure the copy speaks to customer pain points (reference the customer sentiment research)
6. Break up long blocks of text for scannability
7. Add trust-building elements throughout

Don't change the factual content or SEO structure. Just make the copy convert better.
```

---

← [Previous: Intelligence](./intelligence.md) | [Next: Technical SEO Prompts →](./technical-seo.md)
