# romanrabodzei.github.io

Personal GitHub Pages site for [Roman Rabodzei](https://romanrabodzei.github.io). A single-page site (home, about, projects, blog) built with plain HTML/CSS/JS, no build step or framework.

## Structure

```
├── index.html            # Single-page app: home, about, projects, and blog-index sections
├── blog/                  # Standalone blog post pages (one self-contained .html file per post)
├── images/                # Certification badges and resume PDF
├── content-plan-oct2026.md  # Editorial calendar / publishing schedule for upcoming posts
└── readme.md              # This file
```

### `index.html`

A client-side routed single-page site (`.page` sections toggled by a tiny JS router, hash-based navigation). Sections:

- **Home** — hero intro, tech-stack tags, latest-posts card (top 5, synced with `blog/`), career timeline, and social links
- **About** — bio and full certification list (Microsoft Azure, GitHub, HashiCorp, Kubernetes/CNCF), grouped by tier
- **Projects** — open-source project cards with grid/list view toggle
- **Blog** — full chronological list of all posts, linking into `blog/`

Supports light/dark theme (persisted in `localStorage`) and has no external JS dependencies beyond Google Fonts.

### `blog/`

Each post is a fully self-contained HTML file (own `<style>`/`<script>`, dark-themed by default, custom inline SVG hero illustration, share button, back-to-blog link). Posts are English-only and follow a consistent title convention (`Some Topic: Specific Subtitle`). Current coverage spans Azure platform engineering, AKS/Kubernetes internals, AI agents & Microsoft Foundry, GitHub/DevOps security, and certification write-ups.

New posts are added in two places in `index.html`: the full list under the **Blog** page, and the top-5 "Latest Posts" card on **Home** (oldest entry commented out, not deleted, to keep history easy to restore).

## Features

- About section with professional bio
- Licenses & Certifications (Microsoft Azure, HashiCorp, GitHub, Kubernetes / CNCF)
- Blog with 20+ posts on Azure, Kubernetes/AKS, AI agents, and DevOps security
- Links to LinkedIn and GitHub profiles
- Support links (Buy me a coffee, PayPal)