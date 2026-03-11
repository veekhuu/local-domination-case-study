← [Previous: Content at Scale](./05-content-at-scale.md) | [Next: Deploy & Index →](./07-deploy-index.md)

# Phase 6: Technical SEO & Speed Optimization

**Time:** Day 3
**Tools:** Claude Code
**Cost:** $0 (built into the dev process)
**Prompts for this phase:** [prompts/technical-seo.md](../prompts/technical-seo.md)

---

```
TECHNICAL SEO + SPEED OPTIMIZATION
═══════════════════════════════════════════════════════════

  ┌─────────────────────────────────────────────────────┐
  │                  SEO FOUNDATION                      │
  │                                                      │
  │  ┌───────────┐ ┌───────────┐ ┌───────────────────┐  │
  │  │  Schema    │ │  XML      │ │  robots.txt       │  │
  │  │  Markup    │ │  Sitemap  │ │  + crawl config   │  │
  │  │           │ │  w/ prior-│ │                    │  │
  │  │  Per-page  │ │  ities   │ │  Allow ALL         │  │
  │  │  structured│ │           │ │  crawlers          │  │
  │  │  data     │ │           │ │  (incl. training)  │  │
  │  └───────────┘ └───────────┘ └───────────────────┘  │
  │                                                      │
  │  ┌───────────┐ ┌───────────┐ ┌───────────────────┐  │
  │  │  Canonical │ │  Meta     │ │  llms.txt         │  │
  │  │  URLs     │ │  Titles & │ │                    │  │
  │  │           │ │  Descrip- │ │  AI crawler        │  │
  │  │  All pages │ │  tions   │ │  instructions      │  │
  │  │           │ │           │ │  (like robots.txt  │  │
  │  │           │ │  Every    │ │   for LLMs)        │  │
  │  │           │ │  page     │ │                    │  │
  │  └───────────┘ └───────────┘ └───────────────────┘  │
  └─────────────────────────────────────────────────────┘
                           │
                           ▼
  ┌─────────────────────────────────────────────────────┐
  │                SPEED OPTIMIZATION                    │
  │                                                      │
  │  Images ──► WebP    Videos ──► WebM                 │
  │  (squoosh.app OR Claude Code batch-convert)         │
  │                                                      │
  │  + Lazy loading (below-fold images/video)           │
  │  + Core Web Vitals optimization                     │
  │    ◦ LCP < 2.5s                                     │
  │    ◦ FID < 100ms                                    │
  │    ◦ CLS < 0.1                                      │
  └─────────────────────────────────────────────────────┘
                           │
                           ▼
  ┌─────────────────────────────────────────────────────┐
  │  RESULT: 97/100 PageSpeed (desktop)                  │
  │          86/100 PageSpeed (mobile)                   │
  │                                                      │
  │  One person beat a 20-person dev team.               │
  └─────────────────────────────────────────────────────┘
```

---

## SEO Foundation

With the content done, moved into the technical foundation — the behind-the-scenes work that makes search engines actually want to rank your site.

Claude added:

- **Schema markup** — Structured data that helps Google understand what each page is about. Applied to every page type: services, locations, blog articles, about page
- **XML sitemap** — With proper priority settings telling search engines which pages are most important
- **Robots.txt** — Optimized for crawling, telling search engine bots how to navigate the site
- **Canonical URLs** — For all pages, preventing duplicate content issues
- **Meta titles and descriptions** — Unique for every single page across [NUMBER_OF_PAGES]+
- **llms.txt** — A newer file that tells AI crawlers specifically what to pull from your site (similar to robots.txt but for large language models)

---

## The Common Crawl Decision

A deliberate — and somewhat controversial — choice:

> Allow Common Crawl and all LLM training bots to access our content. Not just search crawlers or AI search bots, but the training crawlers too.

**The theory** (from the CEO of SearchAtlas): If your company's information becomes part of the data that AI models are trained on, when someone later asks an AI about [INDUSTRY] in [TARGET MARKET], your company's information gets cited. You become part of the AI's knowledge base.

**The risk:** Basically zero. Your content is already public. You're just making it easier for AI models to learn from it.

Configure this in robots.txt by explicitly allowing:

- CCBot (Common Crawl)
- GPTBot (OpenAI)
- ClaudeBot (Anthropic)
- Google-Extended (Google AI training)
- Other major LLM training crawlers

---

## Speed Optimization

[INDUSTRY] websites need lots of images — portfolio shots, project photos, team pictures. These are all trust signals. But images from a phone camera are usually massive JPEG or PNG files that tank loading speed.

### Image Conversion

- Every image converted to WebP format
- Initially done one-by-one using squoosh.app (wasted about an hour)
- Then discovered Claude Code could batch-convert all of them
- Lesson learned: always ask your AI coding tool before doing repetitive manual work

### Video Conversion

- All videos converted from MP4 to WebM (smaller file size)

### Lazy Loading

- Images only load when you scroll to them
- Initial page load stays fast because only above-the-fold content loads immediately

### Core Web Vitals Optimization

- **LCP** (Largest Contentful Paint): < 2.5 seconds
- **FID** (First Input Delay): < 100 milliseconds
- **CLS** (Cumulative Layout Shift): < 0.1
- These are Google's speed metrics that directly affect search rankings

---

## The Results

```
┌────────────────────────────┬──────────┐
│  Desktop PageSpeed          │  97/100  │
│  Mobile PageSpeed           │  86/100  │
│  Previous 20-person team    │  85/100  │
└────────────────────────────┴──────────┘
```

One person with AI tools beat a 20-person dev team on the most important performance metric.

---

## Key Takeaway

> Don't waste an hour doing something one by one when Claude Code can batch-process it in seconds. And allow AI crawlers — the downside is zero, the upside could be significant for AEO.

---

**Prompts for this phase:** [prompts/technical-seo.md](../prompts/technical-seo.md)

← [Previous: Content at Scale](./05-content-at-scale.md) | [Next: Deploy & Index →](./07-deploy-index.md)
