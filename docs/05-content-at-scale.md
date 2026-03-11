← [Previous: Site Skeleton](./04-site-skeleton.md) | [Next: Technical SEO →](./06-technical-seo.md)

# Phase 5: Content at Scale

**Time:** Day 2 Evening — Day 3
**Tools:** Claude Code (multiple instances, agent teams)
**Cost:** Subscription only
**Prompts for this phase:** [prompts/content.md](../prompts/content.md)

---

```
CONTENT AT SCALE — THREE PARALLEL TRACKS
═══════════════════════════════════════════════════════════

  ┌─────────────────────────────────────────────────────┐
  │  INPUT: All research documents from Phase 3          │
  │  "Read all of this. Now update the build plan."     │
  └────────────────────────┬────────────────────────────┘
                           │
              ┌────────────┼────────────────┐
              │            │                │
              ▼            ▼                ▼
     ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
     │  INSTANCE 1   │ │  INSTANCE 2   │ │  INSTANCE 3   │
     │               │ │               │ │               │
     │  SERVICE       │ │  LOCATION     │ │  BLOG         │
     │  PAGES         │ │  PAGES        │ │  ARTICLES     │
     │               │ │               │ │               │
     │  [NUMBER]     │ │  [NUMBER]     │ │  250+         │
     │  services     │ │  cities       │ │  articles     │
     └──────┬───────┘ └──────┬───────┘ └──────┬───────┘
            │                │                │
            └────────────────┼────────────────┘
                             │
                             ▼
              ┌──────────────────────────┐
              │  AGENT TEAM PHASES        │
              │                           │
              │  Phase 1: OUTLINES        │
              │  4-5 agents → outlines    │
              │  for 5-10 pages each      │
              │           │               │
              │           ▼               │
              │  Phase 2: RESEARCH        │
              │  Same agents → research   │
              │  from reputable sources   │
              │  Must cite everything     │
              │           │               │
              │           ▼               │
              │  Phase 3: WRITING         │
              │  10 agents writing        │
              │  simultaneously           │
              │  10 pages at once         │
              └──────────────┬───────────┘
                             │
                             ▼
              ┌──────────────────────────┐
              │  COPYWRITING POLISH       │
              │                           │
              │  Kennedy · Halbert        │
              │  Bencivenga · Ogilvy      │
              │  Cialdini · Hormozi       │
              │  Edwards                  │
              │                           │
              │  Direct-response          │
              │  frameworks applied       │
              │  across all pages         │
              └──────────────────────────┘
```

---

## Feeding the Research to Claude

After intelligence gathering was complete — competitor analysis, keyword research, market positioning — every research document was dumped into a single folder. Then Claude Code was pointed at all of it with a simple directive:

> "Read all of this. Now update the build plan."

Claude ingested the competitive analysis, keyword lists, audience research, and market data, then revised the build plan accordingly. The AI now understood the landscape: who the competitors were, what keywords to target, what content gaps existed, and how to position the site.

Some things still required manual input and human judgment:

- **Which cities to target** — Selecting the [NUMBER] specific cities for location pages based on business priorities and market opportunity
- **Programmatic SEO approach** — Deciding the templating strategy for generating location-specific content at scale
- **Strategic priorities** — Which services to emphasize, what angle to take in competitive positioning

The AI handles volume. The human handles strategy.

---

## Planning Before Writing

From the keyword research list, Claude was asked to plan **250+ blog articles** organized into topic clusters. The organizational structure was hub-and-spoke format:

- **Each cluster has ONE hub page** — A comprehensive page covering a broad topic (e.g., "[BROAD TOPIC] in [REGION]")
- **Multiple spoke pages branch from each hub** — Specific subtopics that go deep on one aspect (e.g., "[SPECIFIC SUBTOPIC]: What [LOCATION] Homeowners Need to Know")
- **Spokes link back to their hub** — Internal linking creates topical authority signals that search engines reward
- **No two articles target the same keyword** — This avoids keyword cannibalization, where your own pages compete against each other in search results

The critical discipline here: **plan topics, assign keywords, map connections. Do not write yet.**

This planning-first approach means that when writing finally begins, every article already knows its target keyword, its cluster position, which pages it links to, and which pages link back to it. Nothing is written in isolation. Everything is part of a connected content architecture.

---

## Three Parallel Claude Code Instances

With the plan in place, three separate Claude Code instances were fired up simultaneously, each responsible for a different content track.

### Instance 1: Service Pages

[NUMBER] services, each getting a detailed, conversion-optimized page. Every service page includes:

- **Detailed explanation of the service** — What it is, who needs it, when it is necessary
- **Step-by-step process for delivering it** — Transparency builds trust; showing your process removes uncertainty
- **Trust signals** — Credentials, years of experience, certifications, licenses, insurance details
- **"Why choose us" competitive differentiation** — What makes this company different from the dozens of other [INDUSTRY] companies in [REGION]
- **FAQ section (5-8 questions)** — Answers to the questions prospects actually ask, which also targets long-tail search queries
- **Service area details** — Which cities and neighborhoods are served
- **Local information for local SEO** — References to local landmarks, regulations, climate factors, and community details that signal geographic relevance to search engines

### Instance 2: Location Pages

[NUMBER] target cities, each getting a unique, locally-relevant page. Every location page includes:

- **Local service area details** — Specific neighborhoods, districts, and surrounding areas covered
- **Local weather challenges** — Relevant for [INDUSTRY] because weather directly impacts materials, timelines, and maintenance needs (e.g., coastal moisture, inland heat, seasonal rain patterns)
- **Neighborhood-specific content** — References to local architecture styles, common building codes, HOA requirements, and area-specific challenges
- **Area information and local regulations** — Permit requirements, inspection processes, and compliance details specific to that municipality

Additionally, all location pages implemented **ARIA attributes** and followed **WCAG 2.1 Level AA accessibility principles**. California is heavily regulated for accessibility compliance. Without AI assistance, implementing these standards across [NUMBER] pages would have been an enormous manual undertaking. (Note: WCAG 2.2 was being drafted at the time of this build.)

### Instance 3: Blog Articles

**250+ articles** organized by topic clusters, following the hub-and-spoke plan created earlier. Each article targets specific keywords identified during the research phase, with internal linking mapped before a single word was written.

---

## The Research-First Requirement

> Every agent must research the topic from reputable sources before writing a single word. The content must be able to cite where the information came from. No making stuff up. No generic filler.

This single requirement made a huge difference in content quality.

Without it, AI-generated content tends toward vague, generic statements that sound plausible but say nothing specific. With the research-first mandate, every claim has a source. Every statistic has an origin. Every recommendation is grounded in verifiable information.

The difference between "weather can affect your [INDUSTRY] project" and "the average annual rainfall in [CITY] is [X] inches, with [MONTH] through [MONTH] bringing [PERCENTAGE]% of yearly precipitation — here is how that impacts [SPECIFIC SERVICE] timelines" is the difference between content that fills space and content that earns trust.

---

## Agent Team Orchestration

Claude Code organized itself into agent teams. Each agent was responsible for 5-10 pages. They ran in three coordinated phases:

### Phase 1 — Outlines

Four or five agents went out and created detailed outlines for their assigned pages, then came back. Each outline included the target keyword, heading structure, key points to cover, internal links to include, and the specific angle that differentiates this page from similar content.

### Phase 2 — Research

The same agents went out and did research from reputable sources, then came back. Each agent gathered statistics, local information, regulatory details, and industry-specific data relevant to their assigned pages. Everything was sourced and cited.

### Phase 3 — Writing

The main agent assigned 10 junior agents to write 10 pages simultaneously. Each junior agent received its outline, research notes, and the copywriting guidelines, then produced a complete, polished page.

> "I just sat there and watched it work. Ten agents running in parallel, all producing content that's been researched and cited. It was genuinely wild to see."

This three-phase approach — outline, research, write — is what makes quality at scale possible. Skipping any phase degrades the output. Outlines without research produce generic content. Research without outlines produces unfocused content. Writing without either produces content that belongs in the trash.

---

## Copywriting Polish

After raw content was in place, every page was polished for conversion using direct-response copywriting principles drawn from seven of the most influential copywriters and persuasion experts in history:

- **Dan Kennedy** — Magnetic headlines, urgency triggers, direct-response structure that demands action rather than passive reading
- **Gary Halbert** — Conversational tone, story-driven copy that reads like a letter from a trusted friend rather than corporate marketing
- **Gary Bencivenga** — Proof-heavy copy, credibility building through evidence and specificity rather than empty claims
- **David Ogilvy** — Research-backed claims, long-form copy that sells through depth and substance, not brevity
- **Dr. Robert Cialdini** — The six principles of influence: reciprocity, social proof, authority, scarcity, commitment and consistency, liking
- **Alex Hormozi** — Value stacking, irresistible offer construction, making the deal feel like a no-brainer
- **Jim Edwards** — Copywriting frameworks, headline formulas, systematic approaches to persuasive writing (from *Copywriting Secrets*)

These frameworks were synthesized into a **copywriting skill** that Claude could apply consistently across the entire site. Every headline, every CTA, every service description, every FAQ answer was run through these principles. The result is content that does not just inform — it persuades and converts.

---

## Content Volume

Between service pages, location pages, and blog articles: **550+ pages of content**, all researched, cited, and polished for conversion. Produced in days, not months.

For context on what that means manually:

| Content Type | Pages | Manual Estimate | With Agent Teams |
|---|---|---|---|
| Service Pages | [NUMBER] | [WEEKS] | Hours |
| Location Pages | [NUMBER] | [WEEKS] | Hours |
| Blog Articles | 250+ | [MONTHS] | Days |
| **Total** | **550+** | **[MONTHS]** | **~2-3 Days** |

---

## Key Takeaway

> Plan first. Research second. Write third. The 3-phase agent approach (outlines → research → writing) is what makes 550+ pages of quality content possible in days instead of months.

The temptation is always to skip straight to writing. Resist it. The planning and research phases are what separate content that ranks and converts from content that just exists.

---

**Prompts for this phase:** [prompts/content.md](../prompts/content.md)

← [Previous: Site Skeleton](./04-site-skeleton.md) | [Next: Technical SEO →](./06-technical-seo.md)
