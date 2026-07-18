---
title: Welcome to Sify Blog
description: Sify Blog is a modern blog theme built with Astro 6 + Tailwind CSS v4, ready to use out of the box.
date: 2026-06-10
tags: [Astro, Introduction]
category: Notes
pinned: true
cover: https://images.unsplash.com/photo-1499750310107-5fef28a66643?w=1200
---

Sify Blog is a fully-featured Astro blog theme built on Astro 6 and Tailwind CSS v4. If you are looking for a clean, modern, and easy-to-customize blog template, you've come to the right place.

- [Live Demo](https://astro-theme-sify-demo.vercel.app/)
- [GitHub Repository](https://github.com/santisify/astro-theme-sify)

## Quick Start

```bash
git clone https://github.com/santisify/astro-theme-sify.git my-blog
cd my-blog
bun install
bun dev
```

Open `http://localhost:4321` to preview. For detailed steps, please refer to [Building a Blog from Scratch](/post/getting-started).

## Features

| Feature | Description |
|------|------|
| Markdown / MDX | Support for standard Markdown and JSX components |
| Math Formulas | KaTeX rendering for inline and block equations |
| Mermaid Diagrams | Flowcharts, sequence diagrams, Gantt charts, etc. |
| Code Highlighting | Shiki dual theme, language labels, one-click copy, line numbers |
| Dark Mode | System preference sync + manual toggle, flicker-free |
| Full-Site Search | Triggered with `Ctrl+K`, title + body match with highlighting |
| Comment System | Waline comment area, dark mode support |
| RSS | Automatically generated RSS Feed |
| Friends | Friend links + friend circle dynamic updates + status health check |
| Article Series | Automatic grouping of articles in the same series |
| Share Buttons | Twitter / WeChat QR Code / Copy Link / Native Share |
| Reading Progress | Top progress bar + TOC highlighting |
| i18n | Multi-language switching support |
| PWA | Installable, supports offline access |
| SEO | Open Graph, Twitter Card, JSON-LD |
| Responsive | Perfectly adapted to mobile devices |

## Pages & Routes

| Path | Page |
|------|------|
| `/` | Homepage (Post List + Hero) |
| `/post/[...slug]` | Post Details Page |
| `/categories/[category]` | Category Page |
| `/tags/[tag]` | Tag Page |
| `/archives` | Archive Page |
| `/weekly` | Weekly Newsletter Page |
| `/friends` | Friend Links Page |
| `/about` | About Page |
| `/rss.xml` | RSS Subscription |

## Tech Stack

- **Framework**: Astro 6 + View Transitions
- **Styling**: Tailwind CSS v4 (`@theme` syntax)
- **Code Highlighter**: Shiki (Dual theme)
- **Math Formulas**: remark-math + rehype-katex
- **Diagrams**: Mermaid.js
- **Comments**: Waline
- **Deployment**: Vercel / Cloudflare Pages / Any static hosting

> Press `Ctrl + K` to call out the search panel at any time.
