# Phase 2: Scrollytelling Hero Prompts

← [Previous: Planning](./planning.md) | **Documentation:** [docs/02-scrollytelling.md](../docs/02-scrollytelling.md)

---

> **Note:** These are reconstructed approximations of the prompts used during the scrollytelling hero creation phase. The original workflow was voice-to-text via Wispr Flow, so these have been adapted into written form that captures the same intent.

---

## 1. Storyboard Brainstorming

**Target: Gemini / ChatGPT**

```
I'm building a scrollytelling hero section for a [COMPANY TYPE] website. Scrollytelling = the page tells a visual story as you scroll. Images and animations are tied to scroll position instead of time.

I need a storyboard concept. The visual narrative should show the journey from [STARTING POINT - e.g., "dreaming about a custom home"] to [ENDING POINT - e.g., "living in a finished custom home"].

Break it into 4 stages:
- Stage 1: [THE DREAM/PROBLEM]
- Stage 2: [THE PLANNING/DESIGN]
- Stage 3: [THE BUILDING/TRANSFORMATION]
- Stage 4: [THE FINISHED RESULT/NEW LIFE]

For each stage, describe:
1. The visual scene in detail
2. The mood and lighting
3. Key objects or elements that should be prominent
4. How it connects to the next stage

This needs to feel premium and immersive. Not generic stock photo territory — something that makes a visitor stop and think "these people are different."
```

---

## 2. Custom GPT Image Prompts

**Target: ChatGPT Custom GPT for Nano Banana**

```
I need image generation prompts written specifically for Nano Banana.

Here is Stage [NUMBER] of my scrollytelling storyboard:
[PASTE STAGE DESCRIPTION]

Write a detailed Nano Banana prompt that will generate this scene. Focus on:
- Photorealistic quality
- Consistent style across all stages
- [INDUSTRY]-appropriate imagery
- Warm, premium lighting
- High detail in architectural/construction elements
```

> **Tip:** The author found an existing Custom GPT that specializes in writing Nano Banana prompts rather than creating one from scratch. Search ChatGPT's GPT store for "Nano Banana prompt writer" or similar.

---

## 3. Video Transition Concept

**Target: Gemini**

```
Here are two images. Frame 1 is [DESCRIPTION OF STARTING IMAGE]. Frame 2 is [DESCRIPTION OF ENDING IMAGE].

I need to create a smooth video transition between them using an AI video generator (fal.ai).

Give me three creative concepts for how to transition from Frame 1 to Frame 2:
1. What visual elements should morph or transform?
2. What's the camera movement?
3. What's the mood shift?

Which concept would look most premium and professional for a [INDUSTRY] website? Recommend the best approach.
```

---

## 4. fal.ai Video Generation

**Target: fal.ai**

```
[PASTE THE WINNING CONCEPT FROM GEMINI]

Create a smooth transition from the start frame to the end frame. The transition should feel cinematic and premium. [SPECIFIC DETAILS ABOUT THE TRANSITION].
```

> **Cost note:** Each clip costs ~$3-4 to generate. Budget for a few variations per transition. Total hero section cost: ~$30-40.

---

## 5. Frame Extraction Workflow

This is not a prompt but the post-production workflow for turning your generated video clips into scrollytelling frames.

1. **Stitch clips together.** After generating all video clips, combine them in CapCut (free). Speed up certain parts to keep the overall length tight (~8 seconds per generated clip).
2. **Export.** Export the final stitched video as MP4.
3. **Extract frames.** Go to [EZgif.com](https://ezgif.com) and use the "Video to frames" tool. Set it to 24 frames per second. A few seconds of animation produces a couple hundred frame images.
4. **Download all frames.** These are the images the scrollytelling script displays based on scroll position. Each frame corresponds to a specific point in the user's scroll progress.

---

← [Previous: Planning](./planning.md) | [Next: Intelligence Prompts →](./intelligence.md)
