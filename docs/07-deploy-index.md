← [Previous: Technical SEO](./06-technical-seo.md) | [Back to README →](../README.md)

# Phase 7: Deployment, Indexing & Analytics

**Time:** Day 3 Evening — Week 2
**Tools:** GitHub, Vercel, Rapid Indexer, Google Analytics, Google Search Console, Microsoft Clarity, Meta Pixel
**Cost:** ~$30 (Rapid Indexer)
**Prompts for this phase:** No specific prompts — this phase is configuration and deployment

---

```
DEPLOY → WAIT → INDEX → MEASURE
═══════════════════════════════════════════════════════════

  DAY 3 EVENING
  ┌──────────┐     ┌──────────┐     ┌──────────┐
  │  Claude   │     │  GitHub   │     │  Vercel   │
  │  Code     │────►│           │────►│           │
  │           │     │  Code     │     │  Hosting  │
  │  Build    │     │  repo     │     │  (free)   │
  └──────────┘     └──────────┘     └──────┬─────┘
                                           │
                                    WEBSITE IS LIVE
                                           │
                                           ▼
  DAYS 4-7                         ┌──────────────┐
  ┌──────────────────────────┐     │              │
  │  THE WAITING GAME         │     │  NOTHING     │
  │                           │     │  HAPPENS     │
  │  "Three days. Nothing.    │     │              │
  │   Four days. Still        │     │  No rankings │
  │   nothing. Started        │     │  No traffic  │
  │   second-guessing."       │     │              │
  └──────────────────────────┘     └──────┬───────┘
                                          │
                                          ▼
  WEEK 2
  ┌──────────────────────────────────────────────────┐
  │  ANALYTICS SETUP                                  │
  │                                                   │
  │  ┌──────────┐ ┌──────────┐ ┌────────────────────┐│
  │  │  Google   │ │  Google   │ │  Microsoft Clarity ││
  │  │Analytics │ │  Search   │ │                    ││
  │  │          │ │  Console  │ │  Heat maps:        ││
  │  │ Traffic  │ │           │ │  where visitors    ││
  │  │ data     │ │ How Google│ │  click and scroll  ││
  │  │          │ │ sees site │ │                    ││
  │  └──────────┘ └──────────┘ └────────────────────┘│
  │                                                   │
  │  ┌──────────┐ ┌──────────────────────────────────┐│
  │  │  Meta     │ │  Rapid Indexer (~$30)            ││
  │  │  Pixel   │ │                                  ││
  │  │          │ │  Nudge Google to index all pages  ││
  │  │ Future ad│ │  (Google is slow for new sites)   ││
  │  │retarget- │ │                                  ││
  │  │ ing      │ │                                  ││
  │  └──────────┘ └──────────────────────────────────┘│
  └──────────────────────────┬───────────────────────┘
                             │
                             ▼
  ┌──────────────────────────────────────────────────┐
  │  RESULTS (After ~1 Week of Indexing)              │
  │                                                   │
  │  ✦ Ranking for competitive [TARGET MARKET] terms  │
  │  ✦ Showing up inside ChatGPT                     │
  │  ✦ 97/100 PageSpeed (desktop)                    │
  │  ✦ 86/100 PageSpeed (mobile)                     │
  │  ✦ 0 → 1,100+ visits in 7 days (~400 real)      │
  │  ✦ One person beat a 20-person dev team          │
  └──────────────────────────────────────────────────┘
```

---

## Deployment: GitHub to Vercel

- Site was about 80% done at deployment time
- Deployed through GitHub to Vercel
- Vercel: fast, free hosting platform that deploys directly from GitHub
- The website was live

> Don't wait for perfection. Deploy at 80% and iterate. A live site that's 80% done beats a perfect site that's still on your laptop.

---

## The Waiting Game

> Three days. Nothing. Four days. Still nothing. No movement in search rankings. I started second-guessing every decision.

This is normal. Google doesn't instantly index new sites. The waiting period is psychologically difficult but expected. Don't panic, don't make drastic changes.

---

## Analytics Setup

Installed tracking tools (should have done this BEFORE launch — lesson learned):

- **Google Analytics** — Traffic data: where visitors come from, which pages they visit, how long they stay
- **Google Search Console** — How Google views your site: which queries you appear for, click-through rates, indexing status, errors
- **Microsoft Clarity** — Heat maps showing exactly where visitors click and scroll on your pages. "This one is incredibly useful for optimizing your site later."
- **Meta Pixel** — For potential future ad retargeting campaigns

---

## Rapid Indexer

- Google's indexing can be extremely slow for new sites
- Used Rapid Indexer (~$30) to nudge Google to come look at all pages
- Significantly speeds up the indexing process
- About a week after indexing, results started appearing

---

## The Results

```
╔══════════════════════════════════════════════╗
║  FINAL SCORECARD                              ║
╠══════════════════════════════════════════════╣
║                                               ║
║  Pages live:           [NUMBER_OF_PAGES]+     ║
║  Desktop PageSpeed:    97/100                 ║
║  Mobile PageSpeed:     86/100                 ║
║  Total cost:           ~$[TOTAL_COST]         ║
║  Traditional cost:     $[TRADITIONAL_COST]+   ║
║  Build time:           [BUILD_DAYS] days      ║
║  Team size:            1 person               ║
║                                               ║
║  Traffic (7 days):     0 → 1,100+ visits      ║
║  (estimated real):     ~400 (excluding junk)  ║
║                                               ║
║  Competitive terms:    Ranking                ║
║  ChatGPT:              Showing up             ║
║                                               ║
║  Previous dev team     10-20 people           ║
║  Their PageSpeed:      85/100                 ║
║  Our PageSpeed:        97/100                 ║
╚══════════════════════════════════════════════╝
```

---

## What's Still Happening

The foundation was three days. But a good website is never truly done:

- Adding more trust signals (reviews, certifications, project photos)
- Researching more competitors as they change their sites
- Adding and optimizing lead capture forms
- Getting more social proof
- Writing more content to expand [INDUSTRY] coverage
- Monitoring Microsoft Clarity heat maps and adjusting design

---

## The Real Lesson

> The AI didn't make this easy. The AI made this possible. I still had to come up with the scrollytelling concept. I still had to decide which competitors to study. I still had to make judgment calls about content strategy, keyword targeting, and technical architecture. The AI removed the $[TRADITIONAL_COST] price tag. It didn't remove the thinking.

---

## What I'd Do Differently

1. **Set up Keywords Everywhere MCP from the start** — Initial keyword research was Claude's best guesses. Real search volume data from day one would have been better.
2. **Use Claude Code for image batch-conversion** — Wasted an hour on squoosh.app doing images one by one.
3. **Mobile-first from day one** — 97 desktop but only 86 mobile. Should have optimized for phones first.
4. **Install analytics before launch** — Missed the first week of data.

---

← [Previous: Technical SEO](./06-technical-seo.md) | [Back to README →](../README.md)
