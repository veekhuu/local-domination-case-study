# Complete Tool List (By Phase)

Every tool used in this build, organized by when you'd use them.

---

## Planning & Brainstorming

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
Wispr Flow        Voice-to-text so you can talk to AI             Subscription
                  instead of typing

Claude            Brainstorming, planning, writing the PRD        Subscription

Gemini            Storyboarding, creative concepts, keyword       Free/Subscription
                  research. Has access to Google's search data
```

---

## Scrollytelling Hero Section

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
ChatGPT           Used a Custom GPT to write image                Subscription
                  generation prompts for Nano Banana

Nano Banana       AI image generator for each visual stage        Pay per generation

fal.ai            AI video generator. Upload start + end          ~$3-4 per clip
                  frame, describe the transition                  (~$30-40 total)

CapCut            Free video editor. Stitched clips together      Free
                  and adjusted speed

EZgif.com         Broke final video into individual frame         Free
                  images for the scroll effect
```

```
SCROLLYTELLING PIPELINE
═══════════════════════════════════════════════════════

  Storyboard        Generate         Generate         Stitch
  concepts          images           video clips      + extract
                                                      frames
     │                 │                │                │
     ▼                 ▼                ▼                ▼
  ┌────────┐     ┌──────────┐    ┌──────────┐    ┌──────────┐
  │ Gemini │ ──► │   Nano   │ ──►│  fal.ai  │ ──►│  CapCut  │
  │   +    │     │  Banana  │    │          │    │    +     │
  │ChatGPT │     │          │    │ $3-4/clip│    │  EZgif   │
  └────────┘     └──────────┘    └──────────┘    └──────────┘

  ~2 hours           ~1 hour         ~1 hour         ~30 min
```

---

## Competitive Intelligence

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
Manus AI          AI research tool with SimilarWeb access.        ~10K credits
                  Analyzed competitors, reviews, service          total
                  gaps, and SEO/AEO best practices

Claude +          Found gaps between competitor offerings         Subscription
Tavily Search +   and ours
Perplexity MCP
```

```
INTELLIGENCE GATHERING
═══════════════════════════════════════════════════════

              ┌───────────────────────┐
              │    10 COMPETITORS     │
              │   from Google pg. 1   │
              └───────────┬───────────┘
                          │
              ┌───────────┴───────────┐
              │                       │
              ▼                       ▼
     ┌────────────────┐     ┌────────────────┐
     │   Manus AI +   │     │   Claude +     │
     │   SimilarWeb   │     │   Tavily +     │
     │                │     │   Perplexity   │
     └───────┬────────┘     └───────┬────────┘
             │                      │
             ▼                      ▼
     ┌────────────────┐     ┌────────────────┐
     │  Pass 1:       │     │  Service gaps  │
     │  Traffic,      │     │  between       │
     │  keywords,     │     │  competitors   │
     │  strengths     │     │  and us        │
     └───────┬────────┘     └────────────────┘
             │
             ▼
     ┌────────────────┐
     │  Pass 2:       │
     │  Customer      │
     │  reviews,      │
     │  complaints,   │
     │  praise, gaps  │
     └────────────────┘
```

---

## Building & Coding

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
Claude Code       AI coding tool. Built the entire site,          Subscription
                  ran agent teams for content, handled
                  technical SEO. The workhorse.

Astro 5           Website framework. Makes sites load             Free
                  extremely fast.
```

---

## Speed Optimization

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
squoosh.app       Compress/convert images to WebP one by one.     Free
                  (Use Claude Code to batch-convert instead.
                  I learned that the hard way.)
```

---

## Deployment

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
GitHub            Where the code lives                            Free
Vercel            Hosting. Deploys directly from GitHub.          Free tier
```

---

## Indexing & Analytics

```
TOOL              WHAT IT DOES                                    COST
─────────────────────────────────────────────────────────────────────────
Rapid Indexer     Gets Google to index your pages faster          ~$30

Google Search     See how Google views your site and what         Free
Console           you're ranking for

Google Analytics  Traffic and visitor data                        Free

Microsoft         Heatmaps showing where visitors click           Free
Clarity           and scroll. Incredibly useful for
                  optimization.

Meta Pixel        Retargeting for potential future ad campaigns   Free
```
