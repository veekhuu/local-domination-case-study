← [README](../README.md) | [Next: Scrollytelling Hero →](./02-scrollytelling.md)

# Phase 1: Planning & Concept Development

**Time:** Day 1 Morning
**Tools:** Wispr Flow, Claude, Gemini
**Cost:** $0 (subscription tools only)
**Prompts for this phase:** [prompts/planning.md](../prompts/planning.md)

---

```
PLANNING WORKFLOW
═══════════════════════════════════════

  ┌──────────────────┐
  │  COMPETITOR       │
  │  RESEARCH         │
  │  20-30 websites   │
  │  analyzed         │
  └────────┬─────────┘
           │  "They're all the same"
           ▼
  ┌──────────────────┐
  │  THE INSIGHT      │
  │  Scrollytelling = │
  │  unheard of in    │
  │  [INDUSTRY]       │
  └────────┬─────────┘
           │
           ▼
  ┌──────────────────┐     ┌──────────────────┐
  │  WISPR FLOW       │────►│  CLAUDE           │
  │  Voice-to-text    │     │  Brainstorming    │
  │  (talk, don't     │     │  + Plan Mode      │
  │   type)           │     │                   │
  └──────────────────┘     └────────┬─────────┘
                                    │
                                    ▼
                           ┌──────────────────┐
                           │  PRD              │
                           │  (placeholders    │
                           │   everywhere)     │
                           │                   │
                           │  ◦ Site arch      │
                           │  ◦ Page types     │
                           │  ◦ SEO/AEO reqs   │
                           │  ◦ Tech stack     │
                           │  ◦ Content plan   │
                           └──────────────────┘
```

---

## The Insight: Every Competitor Looks the Same

Before writing a single line of code, the first step was studying the competition. A deep dive into 20-30 competitor websites in the [INDUSTRY] space revealed a striking pattern: they all looked the same. A few service pages, a hero video, a "get a free consultation" button, maybe a handful of blog posts. Nothing memorable. Nothing that made any one of them stand out from the rest.

This uniformity is the opportunity. When every competitor follows the same playbook, differentiation becomes a powerful advantage. The insight was clear: if every website in [INDUSTRY] looks identical, doing something genuinely different would immediately command attention.

## Why Scrollytelling?

The idea that emerged was scrollytelling -- a website where the page tells a visual story as the user scrolls. Instead of a static hero section or an autoplay video, the visitor controls the narrative through their own scrolling. It feels cinematic and immersive.

Both Gemini and Claude confirmed the hypothesis: scrollytelling is a well-established technique in industries like journalism, fashion, and tech storytelling, but it is essentially unheard of in [INDUSTRY TYPE]. That gap between "proven technique" and "nobody in this space uses it" is exactly where the biggest opportunities live.

Being different is the fastest way to stand out when every competitor looks the same.

## The Planning Process: Talk First, Build Later

Planning started with talking, not building. Using Wispr Flow (a voice-to-text tool), the vision was described out loud and naturally, speaking directly to Claude in plan mode. No typing, no overthinking -- just explaining the idea as if talking to a collaborator.

The key input sounded something like this:

> "I want to build a new website for a [COMPANY TYPE] company. I want programmatic capability to build out service pages and location pages. The main thing I want is for the hero section to have scrollytelling elements. I want to use Astro instead of WordPress."

From there, the brainstorming unfolded collaboratively. Goals were identified together:

1. **Compete with established competitors** -- match and exceed what they offer online
2. **Generate qualified leads consistently** -- not just traffic, but people ready to buy
3. **Improve search visibility** -- rank on Google and get cited by AI search tools (ChatGPT, Perplexity, Claude)

The critical principle: start by talking, not building. Voice-to-text removes friction and lets ideas flow faster than typing ever could.

## Building the PRD

With the vision articulated, the next step was turning it into a structured plan. Over a few rounds of iteration with Claude, a full PRD (Product Requirements Document) took shape. The PRD covered:

- **Site architecture** -- how pages connect and link to each other
- **Page types** -- service pages, location pages, landing pages, blog posts
- **SEO/AEO requirements** -- what the site needs to rank on Google and get cited by AI tools
- **Design direction** -- scrollytelling hero, visual storytelling, differentiation
- **Content strategy** -- what content to create, for whom, and why
- **Technical stack** -- Astro 5 as the framework, deployment considerations

The critical rule throughout this entire process: **use [PLACEHOLDER] for anything not finalized.** If a detail was not decided yet -- the exact headline, the specific color palette, the final list of services -- it was marked as a placeholder and moved past. Nothing was allowed to stall progress.

> "If you don't have something, just write placeholder and move on. Over-analysis is the number one killer of projects like this."

## The Framework Decision: Astro 5

The technical stack decision was made early: Astro 5 over WordPress. The primary reason is speed. Astro generates static HTML by default, which makes websites load extremely fast compared to WordPress's PHP-rendered pages.

Speed matters for two reasons:

1. **SEO** -- Google uses page speed as a ranking factor. Faster sites rank higher.
2. **User experience** -- visitors bounce from slow sites. Every second of load time costs conversions.

This decision later proved right. The finished site achieved a **97/100 PageSpeed desktop score** -- a benchmark that most WordPress sites struggle to reach even with extensive optimization.

## Key Takeaway

> If you don't have something, just write "placeholder" and move on. The point is to get the plan on paper so you don't stall.

The planning phase is about momentum. A perfect plan that takes two weeks is worth less than a good-enough plan that takes two hours. Get the structure down, mark what you don't know, and keep moving.

---

**Prompts for this phase:** [prompts/planning.md](../prompts/planning.md)

← [README](../README.md) | [Next: Scrollytelling Hero →](./02-scrollytelling.md)
