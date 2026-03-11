← [Previous: Intelligence Gathering](./03-intelligence.md) | [Next: Content at Scale →](./05-content-at-scale.md)

# Phase 4: Building the Site Skeleton

**Time:** Day 1 Evening
**Tools:** Claude Code, Astro 5
**Cost:** $0 (subscription tools only)
**Prompts for this phase:** Integrated into [prompts/planning.md](../prompts/planning.md)

---

```
SITE SKELETON BUILD
═══════════════════════════════════════

  ┌──────────────────┐
  │  CLAUDE CODE      │
  │  + Astro 5        │
  │                   │
  │  "Speed matters   │
  │   for SEO and UX" │
  └────────┬─────────┘
           │
           ▼
  ┌──────────────────────────────────┐
  │         HOMEPAGE                  │
  │  ┌────────────────────────────┐  │
  │  │  Scrollytelling Hero       │  │
  │  │  (hundreds of frame imgs)  │  │
  │  └────────────────────────────┘  │
  │  ┌────────────────────────────┐  │
  │  │  [PLACEHOLDER CONTENT]     │  │
  │  │  Services overview         │  │
  │  │  Trust signals             │  │
  │  │  CTA sections              │  │
  │  └────────────────────────────┘  │
  └──────────────────────────────────┘
           │
     ┌─────┼─────────────┐
     │     │             │
     ▼     ▼             ▼
  ┌──────┐ ┌──────────┐ ┌──────┐
  │Serv- │ │Location  │ │About │
  │ice   │ │Pages     │ │Page  │
  │Pages │ │          │ │      │
  │      │ │[NUMBER]  │ │      │
  │[NUM] │ │cities    │ │      │
  │types │ │          │ │      │
  └──────┘ └──────────┘ └──────┘

  All pages: [PLACEHOLDER] content
  Running: localhost only
```

---

## Why Astro 5?

Astro was chosen as the framework for one critical reason: **speed**. Astro generates extremely fast-loading websites through static site generation, which matters for two audiences that never compromise on performance.

- **Astro makes websites load extremely fast.** Static HTML ships to the browser with near-zero JavaScript overhead. Pages render almost instantly, even on slow connections and older devices.
- **Speed matters for both SEO and user experience.** Google uses page speed as a ranking factor. Visitors bounce from slow sites. A fast site wins on both fronts simultaneously.
- **Result: 97/100 PageSpeed on desktop.** The final site scored near-perfect on Google's PageSpeed Insights — a direct consequence of choosing the right framework from the start.
- **Perfect for a site with 550+ pages — static generation keeps everything fast.** Unlike dynamic frameworks that rebuild pages on every request, Astro pre-renders everything at build time. Whether you have 5 pages or 550, each one loads just as quickly.

If you are building a content-heavy site where organic search is the primary traffic channel, framework choice is not a minor decision. Pick something fast. Astro 5 delivers.

---

## What Got Built

At this stage, the following pages were created as the structural foundation of the site:

- **Homepage** with the scrollytelling hero section (from Phase 2) — the cinematic, frame-by-frame animation that hooks visitors immediately
- **Basic service pages** for [NUMBER] services — one page per core service offering, laid out with sections for descriptions, process steps, and calls to action
- **Location pages** for [NUMBER] target cities — one page per geographic area the business serves
- **About page** — company story, team credentials, and trust-building content

All of these pages contained **placeholder content** at this point. The real copy, images, and details come later in Phase 5. The goal here was purely structural: get the pages in place, get the layout right, and see how the site hangs together as a whole.

---

## The Visual-First Approach

> "I'm a visual person. I needed to see the website taking shape before I could move on to the content."

This is a deliberate strategy, not impatience. The build focused first on:

- **Layout** — How sections stack, how content flows from hero to services to social proof to CTA
- **Color scheme** — The palette that communicates [INDUSTRY] professionalism and premium positioning
- **Overall feel** — Does this look and feel like a real premium [INDUSTRY] website? Would a homeowner trust this company based on first impression alone?

The goal was singular: **make it look and feel like a real premium [INDUSTRY] website**. Not a template. Not a generic small-business site. Something that communicates quality, trustworthiness, and expertise at a glance.

Once the design was right — once it genuinely looked like a site belonging to a top-tier [INDUSTRY] company — the focus shifted entirely to content. Design validated. Time to fill it in.

---

## Why Placeholder Content Works

At this stage, everything is still [PLACEHOLDER]. Lorem ipsum. Temporary headings. Stock descriptions. That is by design.

The actual copy, images, and details come after the intelligence gathering phase has been completed and all the research is in hand. Writing final content before you have competitive intelligence and keyword research would be guessing.

This approach lets you:

1. **See the site structure early** — Understand how many pages exist, how they connect, and whether the information architecture makes sense
2. **Test the scrollytelling interaction** — Verify that the hero animation works smoothly, loads correctly, and creates the intended visual impact
3. **Validate the design direction** — Get feedback (from yourself or stakeholders) on look and feel before investing time in content
4. **Move fast without waiting for content** — Design and content can progress in parallel rather than sequentially bottlenecking each other

Placeholder content is not laziness. It is a deliberate workflow decision that keeps momentum high and prevents premature commitment to copy that will change once the research comes in.

---

## Local Development

Everything was running on the local computer at this point. Nothing was online yet. No domain pointed anywhere. No hosting configured. Just `localhost` in a browser.

This matters because:

- **Rapid iteration without deployment overhead** — Change a layout, refresh the browser, see the result. No build pipelines, no deploy steps, no waiting.
- **No public exposure of unfinished work** — Placeholder content stays private. Search engines never see half-built pages.
- **Freedom to experiment** — Try different color schemes, rearrange sections, swap layouts. Nothing is committed until you are ready.

The site goes live later. For now, the goal is to build and validate locally until it is ready.

---

## Key Takeaway

> Build the skeleton first. Get the design right. Fill in the content later. Trying to write final copy before you can see the layout is like furnishing a house before the walls are up.

---

**Prompts for this phase:** Integrated into [prompts/planning.md](../prompts/planning.md)

← [Previous: Intelligence Gathering](./03-intelligence.md) | [Next: Content at Scale →](./05-content-at-scale.md)
