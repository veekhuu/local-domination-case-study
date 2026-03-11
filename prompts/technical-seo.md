# Phase 5: Technical SEO Prompts

← [Previous: Content](./content.md) | **Documentation:** [docs/06-technical-seo.md](../docs/06-technical-seo.md)

> **Note:** These prompts are reconstructed approximations of the prompts used during the project. They capture the intent and structure of the originals but may not be word-for-word matches.

---

## 1. Schema Markup

**Target:** Claude Code

```
Add comprehensive schema markup (structured data) to every page on the site.

Page types and their schema:
- **Homepage**: Organization, LocalBusiness, WebSite
- **Service pages**: Service, FAQPage, BreadcrumbList
- **Location pages**: LocalBusiness (with geo coordinates), ServiceArea, BreadcrumbList
- **Blog articles**: Article, FAQPage (if applicable), BreadcrumbList
- **About page**: Organization, Person (team members)

Ensure all schema:
- Passes Google's Rich Results Test
- Includes proper @context and @type
- Has all recommended (not just required) properties filled
- Uses JSON-LD format in the <head>
```

---

## 2. XML Sitemap

**Target:** Claude Code

```
Generate an XML sitemap with proper priority settings:

- Homepage: priority 1.0, changefreq weekly
- Service pages: priority 0.9, changefreq monthly
- Location pages: priority 0.8, changefreq monthly
- Blog hub pages: priority 0.7, changefreq weekly
- Blog articles: priority 0.6, changefreq monthly
- About/Contact: priority 0.5, changefreq monthly

Include lastmod dates. Ensure the sitemap is referenced in robots.txt.
```

---

## 3. Robots.txt

**Target:** Claude Code

```
Create an optimized robots.txt file:

- Allow all major search engine crawlers (Googlebot, Bingbot, etc.)
- Allow AI search crawlers (ChatGPT-User, PerplexityBot, ClaudeBot, etc.)
- Allow LLM training crawlers (CCBot/Common Crawl, GPTBot, etc.)
- Block admin/private directories
- Reference the XML sitemap
- Reference llms.txt

Note on Common Crawl: We're deliberately allowing Common Crawl and all LLM training bots. The theory (from SearchAtlas CEO): if your company's information becomes part of AI training data, you get cited when someone asks about [INDUSTRY] in [TARGET MARKET]. The downside is basically zero.
```

---

## 4. llms.txt

**Target:** Claude Code

```
Create an llms.txt file for the site root. This is similar to robots.txt but specifically for large language models.

Include:
- Company name and description
- Primary services offered
- Service areas/locations
- Key differentiators
- Contact information
- Links to most important pages (homepage, services, about)
- Structured summary of what the company does

The goal: when an AI model crawls this file, it should have everything it needs to accurately describe and recommend our company.
```

---

## 5. Meta Tags

**Target:** Claude Code

```
Generate unique meta titles and descriptions for every page on the site.

Rules:
- Meta titles: 50-60 characters, include primary keyword, include brand name
- Meta descriptions: 150-160 characters, include primary keyword, include a call-to-action
- Each page must have a UNIQUE title and description (no duplicates)
- Include relevant location for location pages
- Include service name for service pages
- Blog articles should have compelling, click-worthy descriptions

Also implement:
- Canonical URLs for all pages (self-referencing canonicals)
- Open Graph tags for social sharing
- Twitter Card meta tags
```

---

## 6. Common Crawl Config

**Target:** Claude Code

```
Configure the site to explicitly allow Common Crawl and LLM training crawlers.

In robots.txt, ensure these are NOT blocked:
- CCBot (Common Crawl)
- GPTBot (OpenAI)
- ClaudeBot (Anthropic)
- Google-Extended (Google AI training)
- Bytespider (ByteDance)
- Any other major LLM training crawlers

Add a comment in robots.txt explaining why we're allowing these crawlers:
# We allow LLM training crawlers so our company information
# becomes part of AI training data. When users ask AI about
# [INDUSTRY] in [TARGET MARKET], our company gets cited.
```

---

## 7. Image Batch Conversion

**Target:** Claude Code

```
Convert all images in the site to WebP format for optimal loading speed.

For each image:
1. Convert from JPEG/PNG to WebP
2. Maintain quality at 80-85% (good balance of quality vs file size)
3. Generate responsive sizes (thumbnail, medium, large, full)
4. Update all image references in the HTML/Astro components
5. Add proper alt text if missing
6. Implement width and height attributes to prevent layout shift

Also convert any MP4 videos to WebM format for smaller file sizes.

Note: Don't use squoosh.app one by one — batch-convert everything programmatically.
```

---

## 8. Lazy Loading + Core Web Vitals

**Target:** Claude Code

```
Implement lazy loading and optimize for Core Web Vitals:

**Lazy Loading:**
- All images below the fold should use loading="lazy"
- Videos should use lazy loading
- The scrollytelling hero images should preload (they're above the fold)
- Use Intersection Observer for custom lazy loading if needed

**Core Web Vitals targets:**
- LCP (Largest Contentful Paint): < 2.5 seconds
- FID (First Input Delay): < 100 milliseconds
- CLS (Cumulative Layout Shift): < 0.1
- INP (Interaction to Next Paint): < 200 milliseconds

**Audit checklist:**
- Run PageSpeed Insights and fix anything below 90
- Minimize JavaScript bundle size
- Optimize CSS (inline critical CSS, defer non-critical)
- Enable text compression (gzip/brotli)
- Optimize font loading (font-display: swap)
- Remove render-blocking resources
```

---

← [Previous: Content](./content.md) | [Back to Prompts README →](./README.md)
