# Phase 1: Planning Prompts

← [Back to Prompts README](./README.md) | **Documentation:** [docs/01-planning.md](../docs/01-planning.md)

---

> **Note:** These are reconstructed approximations of the prompts used during the planning phase. The original workflow was voice-to-text via Wispr Flow, so these have been adapted into written form that captures the same intent.

---

## 1. Initial Concept Prompt

**Target: Claude**

```
I want to build a new website for [COMPANY TYPE] company. They do [LIST OF SERVICES] in [TARGET MARKET].

I'm going to use some programmatic capability to build out service pages and location pages. The main thing I want is for the hero section to have scrollytelling elements. I want to use Astro instead of WordPress.

Current situation: Their website is on [CURRENT PLATFORM] and it's nearly impossible to do proper SEO and AEO the way modern search engines want.

Goals:
1. Build a website that competes with established competitors who've been at this for years
2. Generate qualified leads consistently
3. Improve search visibility dramatically — both on Google and inside AI search tools like ChatGPT and Perplexity
```

---

## 2. Competitor Study Prompt

**Target: Claude / Gemini**

```
I've looked at 20-30 competitor websites in the [INDUSTRY] niche. They all have the same pattern:
- A few service pages
- A hero video at the top
- A "get a free consultation" button
- Maybe some blog articles

Nothing memorable. Nothing that makes you stop scrolling.

I want to do something completely different. Research scrollytelling websites in other industries and tell me:
1. Is scrollytelling common in [INDUSTRY]?
2. What makes scrollytelling effective for conversion?
3. What are the technical requirements?
4. Why would this differentiate us from every competitor?
```

---

## 3. PRD Development Prompt

**Target: Claude**

```
Based on our brainstorming, let's build a full PRD (Product Requirements Document) together.

Rules:
- For anything we don't have yet (final copy, images, specific content), just write [PLACEHOLDER] and move on
- Don't over-analyze. The point is to get the plan on paper so we don't stall
- Include sections for: site architecture, page types, SEO requirements, AEO requirements, design direction, content strategy, and technical stack

The framework is Astro 5. The site needs:
- Homepage with scrollytelling hero
- [NUMBER] service pages for: [LIST SERVICES]
- [NUMBER] location pages for: [LIST CITIES]
- Blog with [NUMBER]+ articles organized by topic clusters
- About page
- Contact/lead capture

Let's build this PRD now. Use placeholders liberally.
```

---

## 4. Framework Decision Prompt

**Target: Claude**

```
I'm deciding between WordPress and Astro 5 for a [INDUSTRY] website that needs:
- 550+ pages (service pages, location pages, blog articles)
- Scrollytelling hero section with hundreds of frame images
- Maximum PageSpeed score
- Schema markup on every page
- XML sitemap with priorities
- Fast build and deploy times

Compare these options. I'm leaning toward Astro because speed matters for both SEO and user experience. Am I right?
```

---

← [Back to Prompts README](./README.md) | [Next: Scrollytelling Prompts →](./scrollytelling.md)
