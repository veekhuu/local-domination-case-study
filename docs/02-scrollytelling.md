← [Previous: Planning](./01-planning.md) | [Next: Intelligence Gathering →](./03-intelligence.md)

# Phase 2: Creating the Scrollytelling Hero Section

**Time:** Day 1 Afternoon
**Tools:** Gemini, ChatGPT (Custom GPT), Nano Banana, fal.ai, CapCut, EZgif
**Cost:** ~$30-40
**Prompts for this phase:** [prompts/scrollytelling.md](../prompts/scrollytelling.md)

---

```
SCROLLYTELLING PIPELINE
═══════════════════════════════════════════════════════

  ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
  │  STORYBOARD   │     │  IMAGE GEN    │     │  WATERMARK   │
  │               │     │               │     │  REMOVAL     │
  │  Gemini +     │────►│  Nano Banana  │────►│              │
  │  ChatGPT      │     │  (via Custom  │     │  Clean for   │
  │               │     │   GPT prompts)│     │  professional│
  │  4 stages     │     │              │     │  use         │
  └──────────────┘     └──────────────┘     └──────┬───────┘
                                                    │
                        ┌───────────────────────────┘
                        │
                        ▼
  ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
  │  TRANSITION   │     │  VIDEO GEN    │     │  STITCH      │
  │  CONCEPTS     │     │               │     │              │
  │               │────►│  fal.ai       │────►│  CapCut      │
  │  Gemini       │     │  ~$3-4/clip   │     │  Speed up    │
  │  3 options    │     │               │     │  + merge     │
  │  per stage    │     │               │     │              │
  └──────────────┘     └──────────────┘     └──────┬───────┘
                                                    │
                                                    ▼
                                            ┌──────────────┐
                                            │  FRAMES       │
                                            │               │
                                            │  EZgif.com    │
                                            │  24 fps =     │
                                            │  hundreds of  │
                                            │  images       │
                                            └──────────────┘

  COST: ~$30-40          vs.         TRADITIONAL: $5,000-$10,000
```

---

## How Scrollytelling Works

Scrollytelling looks like magic, but the underlying mechanic is straightforward. Here is how it works:

- Each second of video contains approximately 24-30 individual frames (images).
- Traditional video ties those frames to **time** -- press play, and frames advance automatically.
- Scrollytelling ties frames to **scroll position** instead. As the user scrolls down the page, the next frame appears. Scroll up, and the animation reverses.
- The result: the user controls the playback by scrolling. It feels cinematic and interactive.

What you actually need to build this:

1. **Create a video** -- the visual story you want to tell
2. **Break it into hundreds of individual frame images** -- one image per frame
3. **Write a script** that displays the correct frame based on the user's scroll position

The creative challenge is making the video. The technical implementation is the easy part.

## Step 1: Storyboarding (Gemini + ChatGPT)

The storyboard was the creative foundation. This step involved bouncing between Gemini and ChatGPT to develop a coherent visual narrative.

The concept: a **4-stage visual journey** that takes the viewer from [STARTING POINT, e.g., "dreaming about a custom home"] to [ENDING POINT, e.g., "living in the finished home"]. Each stage represents a distinct emotional beat in the story.

The 4 stages might look like:

1. **[STAGE 1]** -- The dream or aspiration (e.g., imagining the perfect home)
2. **[STAGE 2]** -- The process begins (e.g., blueprints and planning)
3. **[STAGE 3]** -- Construction and transformation (e.g., building in progress)
4. **[STAGE 4]** -- The finished result (e.g., the completed home, lived in)

Getting the storyboard right took a few hours. This was the most creatively demanding and most fun part of the entire project. It was also the most time-consuming part of Day 1 -- but it set the creative direction for everything that followed.

## Step 2: Generating Images (Nano Banana via Custom GPT)

With the storyboard locked in, the next step was generating the actual images for each stage.

- **Tool:** Nano Banana AI image generator
- **Key trick:** Did not write prompts directly. Instead, found a **Custom GPT on ChatGPT** that was specifically built for writing Nano Banana prompts.

The workflow:

1. Describe each stage of the storyboard to the Custom GPT
2. The Custom GPT writes optimized prompts for Nano Banana
3. Feed those prompts into Nano Banana and generate images
4. Not every AI-generated image is usable -- run through variations until the quality is right
5. Run final images through a **watermark remover** for a professional, clean look

This last step matters more than you might think. A professional website cannot have watermarks on hero images. The watermark remover ensures every image looks like it was custom-created for the site.

## Step 3: Video Transitions (fal.ai + Gemini)

With the key frame images created, the next step was generating smooth video transitions between them. This is where the static images become a flowing visual story.

**fal.ai** is the core tool here. It works by uploading a beginning frame and an ending frame, then describing in words how you want the transition to look. The AI generates a video clip that morphs one image into the other.

But before generating anything, there was an important creative step:

1. **Feed both frames into Gemini** first
2. Ask: *"Here's frame one and frame two. Give me three concepts for how to transition between them. What's the best approach?"*
3. Gemini provides three creative options for the transition
4. **Pick the best concept** and use that description in fal.ai

This two-step approach (Gemini for creative direction, fal.ai for generation) produces far better results than going straight to generation with a vague prompt.

**Costs:**

- Each clip: ~$3-4 to generate
- Needed a few variations per transition (not every generation is perfect)
- Total for the entire hero section: **~$30-40**

## Step 4: Stitching (CapCut)

With all the individual transition clips generated, they needed to be combined into one seamless video.

- **CapCut** (free video editor) was used to stitch all clips together
- Certain parts were **sped up** to keep the overall length tight and engaging
- Each generated clip is about **8 seconds** long
- The goal: make everything feel like one continuous, seamless animation rather than a series of separate clips

CapCut is free, intuitive, and more than capable for this type of work. No need for Adobe Premiere or Final Cut Pro.

## Step 5: Frame Extraction (EZgif)

The final step converts the finished video back into individual frame images -- the raw material the scrollytelling script needs.

- **EZgif.com** broke the final video into individual frame images
- At **24 frames per second**, even a few seconds of animation produces a couple hundred images
- These frame images are what the scrollytelling JavaScript renders on the page based on the user's scroll position

The math: if your final video is 10 seconds long at 24fps, you get 240 individual images. The scrollytelling script maps scroll position to frame number, displaying the correct image as the user scrolls.

## Cost Comparison

```
┌────────────────────────┬───────────────┐
│  AI-Powered Pipeline   │  ~$30-40      │
│  Traditional Design    │  $5,000-$10K  │
└────────────────────────┴───────────────┘
```

The entire scrollytelling hero section cost approximately $30-40 in AI generation credits. A traditional approach -- hiring a videographer, animator, or motion graphics studio -- would run **$5,000 to $10,000 minimum** for comparable quality.

> "Don't believe me? Go on Fiverr or 99designs and ask for a quote."

The savings are not marginal. They are orders of magnitude different. This is what makes the AI-powered approach viable for [SMALL BUSINESSES / STARTUPS / SOLO FOUNDERS] who would never have the budget for traditional production.

---

**Prompts for this phase:** [prompts/scrollytelling.md](../prompts/scrollytelling.md)

← [Previous: Planning](./01-planning.md) | [Next: Intelligence Gathering →](./03-intelligence.md)
