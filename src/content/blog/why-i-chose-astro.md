---
title: "Why I Chose Astro for This Blog"
description: "A quick look at why Astro is an excellent choice for a content-focused site in 2025."
pubDate: "2025-02-03"
tags: ["astro", "web", "performance"]
---

When I decided to rebuild this blog, I knew I wanted something fast and simple. I looked at a few options — Next.js, SvelteKit, plain HTML — and landed on Astro. Here's why.

## Zero JavaScript by default

Astro ships zero client-side JavaScript unless you explicitly add it. For a blog, that's the right default. There's nothing interactive here that requires JavaScript — pages are documents, and documents don't need a runtime.

The result: pages load instantly, Lighthouse scores stay near-perfect, and there's nothing to hydrate.

## Content collections

Astro's content collections give you type-safe frontmatter validation out of the box. Define a schema once:

```typescript
const blog = defineCollection({
  schema: z.object({
    title: z.string(),
    pubDate: z.coerce.date(),
    tags: z.array(z.string()).default([]),
  }),
});
```

And every post in that collection is validated at build time. Typos in dates, missing titles — caught before they ship.

## The island architecture

For any interactive component you do need, Astro's island architecture lets you hydrate only that component, not the whole page. A search widget, a code playground, a comment form — each is an isolated island. The rest of the page stays static HTML.

## Build output

The build output is static HTML + CSS. No server required, deploys to any CDN, and you get cache headers that actually make sense.

For a blog that doesn't need a database or real-time data, this is exactly the right architecture.
