# How I Rebuilt a Construction Company Website in 3 Days With AI

### 550+ Pages · ~$500 Total · 97/100 PageSpeed · Showing Up in ChatGPT

---

This is a case study and full playbook for how I rebuilt a real construction company's website using AI tools, based on [@boringmarketer](https://github.com/boringmarketer)'s [Local Domination Blueprint](https://github.com/boringmarketer/guides/blob/main/LOCAL-DOMINATION-BLUEPRINT.md) as the foundation.

The blueprint gave me the structure. This repo documents what I added on top to take it from blueprint to live site in one of the most competitive markets in the U.S.

---

## The Situation

My friend runs a high-end custom home building company in the Bay Area. Kitchen remodels, ADU conversions, full custom builds. They're great at what they do. Online? Basically invisible.

Their website was on Wix. SEO was a nightmare. AEO (Answer Engine Optimization — showing up inside ChatGPT, Perplexity, and other AI search tools) was impossible.

So I nuked it and started from scratch.

---

## The Results

```
╔══════════════════════════════════════════════════╗
║                    RESULTS                        ║
╠══════════════════════════════════════════════════╣
║                                                    ║
║  ✦ 550+ pages live                                ║
║  ✦ 97/100 PageSpeed (desktop)                     ║
║  ✦ 86/100 PageSpeed (mobile)                      ║
║  ✦ Ranking for competitive Bay Area terms          ║
║  ✦ Showing up inside ChatGPT                      ║
║  ✦ ~$500 total cost                               ║
║                                                    ║
║  vs. traditional cost: $20,000–$30,000+           ║
║                                                    ║
║  One person beat a 20-person dev team              ║
║  on the most important performance metric.         ║
║                                                    ║
╚══════════════════════════════════════════════════╝
```

---

## The Complete Build Flow

```
~$500 total · 3 days · 550+ pages
═══════════════════════════════════════════════════

DAY 1 MORNING
┌─────────────────────────────────┐
│  PLANNING & CONCEPT             │
│  ◦ Wispr Flow + Claude          │
│  ◦ Research 30 competitor sites │
│  ◦ Brainstorm scrollytelling    │
│  ◦ Write PRD with placeholders  │
└───────────────┬─────────────────┘
                │
                ▼
DAY 1 AFTERNOON
┌─────────────────────────────────┐
│  SCROLLYTELLING HERO  (~$30-40) │
│                                 │
│  Storyboard ──► Images ──► Video ──► Frames
│  (Gemini)    (Nano      (fal.ai) (EZgif)
│              Banana)
│                    │
│              CapCut stitch
│              + speed up
└───────────────┬─────────────────┘
                │
                ▼
DAY 1 EVENING
┌─────────────────────────────────┐
│  SITE SKELETON                  │
│  ◦ Claude Code + Astro 5       │
│  ◦ Homepage with hero           │
│  ◦ Service/location/about pages │
│  ◦ All placeholder content      │
└───────────────┬─────────────────┘
                │
                ▼
DAY 2
┌─────────────────────────────────┐
│  INTELLIGENCE GATHERING         │
│                                 │
│  ┌──────────┐  ┌──────────────┐ │
│  │ Manus AI │  │ Claude +     │ │
│  │ + Similar│  │ Tavily +     │ │
│  │ Web      │  │ Perplexity   │ │
│  └────┬─────┘  └──────┬───────┘ │
│       │               │         │
│       ▼               ▼         │
│  ◦ 10 competitor analysis       │
│  ◦ Customer complaints/praise   │
│  ◦ Service gaps                 │
│  ◦ 100+ target keywords         │
│  ◦ SEO/AEO best practices       │
│                    (~10K credits)│
└───────────────┬─────────────────┘
                │
                ▼
DAY 2 EVENING → DAY 3
┌─────────────────────────────────┐
│  CONTENT AT SCALE               │
│                                 │
│  Claude Code Agent Teams:       │
│                                 │
│  Instance 1    Instance 2    Instance 3
│  8-9 service   45 location   250+ blog
│  pages         pages         articles
│                                 │
│  Phase 1: Outlines ──────────►  │
│  Phase 2: Research ──────────►  │
│  Phase 3: 10 agents writing ──► │
│                                 │
│  + Direct-response copywriting  │
│    polish across all pages      │
└───────────────┬─────────────────┘
                │
                ▼
DAY 3
┌─────────────────────────────────┐
│  TECHNICAL SEO + AEO            │
│  ◦ Schema markup                │
│  ◦ XML sitemap + robots.txt     │
│  ◦ Canonical URLs               │
│  ◦ Meta titles/descriptions     │
│  ◦ llms.txt (AI crawler access) │
│  ◦ Common Crawl allowed         │
│  ◦ Images → WebP, Video → WebM │
│  ◦ Lazy loading                 │
└───────────────┬─────────────────┘
                │
                ▼
DAY 3 EVENING
┌─────────────────────────────────┐
│  DEPLOY                         │
│  Claude Code → GitHub → Vercel  │
└───────────────┬─────────────────┘
                │
                ▼
WEEK 2
┌─────────────────────────────────┐
│  INDEX + MEASURE                │
│  ◦ Google Analytics             │
│  ◦ Google Search Console        │
│  ◦ Microsoft Clarity (heatmaps) │
│  ◦ Meta Pixel                   │
│  ◦ Rapid Indexer (~$30)         │
└─────────────────────────────────┘
```

---

## What I Added Beyond the Blueprint

The [Local Domination Blueprint](https://github.com/boringmarketer/guides/blob/main/LOCAL-DOMINATION-BLUEPRINT.md) covers the core structure: location pages, service pages, blog content, trust signals, lead capture, and GSC troubleshooting. It's the foundation.

Here's what I figured out building on top of it for a real client:

```
BLUEPRINT (James)              WHAT I ADDED
══════════════════             ══════════════════════════════════

Location pages        ──►     + Real SimilarWeb data on 10 competitors
Service pages         ──►     + Customer review sentiment mining
Blog content          ──►     + 10 Claude Code agents writing in parallel
Trust signals         ──►     + Scrollytelling hero section ($40 vs $10K)
Basic SEO             ──►     + AEO: llms.txt + LLM crawler access
WordPress assumed     ──►     + Astro 5 (97/100 PageSpeed)
                              + Direct-response copywriting polish
                              + AI image/video generation pipeline
```

Each addition is documented in detail in the [`/docs`](./docs) folder.

---

## Repo Structure

```
├── README.md .................. You are here
├── tools.md ................... Complete tool list by phase with costs
├── docs/
│   ├── 01-planning.md ......... PRD, brainstorming, concept development
│   ├── 02-scrollytelling.md ... Image → video → frame pipeline
│   ├── 03-intelligence.md ..... Competitive analysis + review mining
│   ├── 04-site-skeleton.md .... Astro 5, Claude Code, framework setup
│   ├── 05-content-at-scale.md . Agent teams, phases, research-first writing
│   ├── 06-technical-seo.md .... SEO + AEO + speed optimization
│   └── 07-deploy-index.md ..... Deployment, indexing, analytics
└── prompts/
    ├── README.md .............. How to use these prompts, what order
    ├── planning.md ............ PRD and brainstorming prompts
    ├── scrollytelling.md ...... Storyboard and image/video prompts
    ├── intelligence.md ........ Competitive analysis + review mining prompts
    ├── content.md ............. Agent team orchestration + writing prompts
    └── technical-seo.md ....... SEO, AEO, and optimization prompts
```

---

## Cost Breakdown

```
┌────────────────────────────┬───────────────┐
│  ITEM                      │  COST         │
├────────────────────────────┼───────────────┤
│  fal.ai video generation   │  ~$30-40      │
│  Manus AI research credits │  ~10K credits │
│  Rapid Indexer             │  ~$30         │
│  Other AI tool costs       │  scattered    │
├────────────────────────────┼───────────────┤
│  TOTAL                     │  ~$500        │
└────────────────────────────┴───────────────┘

vs. Traditional:
┌────────────────────────────┬───────────────┐
│  Scrollytelling hero       │  $5K-$10K     │
│  550+ pages of content     │  $15K-$20K+   │
│  Technical SEO setup       │  $2K-$5K      │
├────────────────────────────┼───────────────┤
│  TOTAL                     │  $20K-$30K+   │
└────────────────────────────┴───────────────┘
```

---

## Credits

This project wouldn't exist without James's ([@boringmarketer](https://github.com/boringmarketer)) [Local Domination Blueprint](https://github.com/boringmarketer/guides/blob/main/LOCAL-DOMINATION-BLUEPRINT.md). The blueprint provided the core strategy and structure. Everything in this repo builds on top of that foundation.

---

## What I'd Do Differently

1. **Set up Keywords Everywhere MCP from the start.** Initial keyword research was Claude's best guesses. Real search volume data from day one would have been better.
2. **Use Claude Code for image batch-conversion.** Wasted an hour on squoosh.app doing images one by one.
3. **Mobile-first from day one.** 97 desktop but only 86 mobile. Should have optimized for phones first.
4. **Install analytics before launch.** Missed the first week of data.

---

## What I'm Still Doing

The foundation was three days. But a good website is never done.

- Adding trust signals (reviews, certifications, project photos)
- Monitoring Microsoft Clarity heatmaps and adjusting design
- Writing more content to expand coverage
- Optimizing lead capture forms
- Researching competitors as they change their sites

---

## The Real Lesson

The AI didn't make this easy. The AI made this possible.

I still had to come up with the scrollytelling concept. I still had to decide which competitors to study. I still had to make judgment calls about content strategy, keyword targeting, and technical architecture.

The AI removed the $30,000 price tag. It didn't remove the thinking.

---

*Follow along on [LinkedIn](https://linkedin.com/in/veekhuu) · [X](https://x.com/veekhuu)*
