# Pagsun AI Insights

A content repository for articles that help Founders and CEOs learn AI strategy — delivering actionable insights, explaining why they matter, and teaching how to build and manage an AI workforce.

---

## Mission

Most founders approach AI reactively — chasing tools instead of building strategy. **Pagsun AI Insights** exists to change that. Every article is written to give founders and executives a clear, practical understanding of how to use AI as a competitive advantage: what decisions to make, how to sequence them, and how to build the team and systems that sustain it.

The guiding editorial principle is: **insight over information**. Readers should finish every article knowing not just what to do, but why it matters and exactly how to start.

---

## Repository Structure

```
pagsun-ai-insights/
├── README.md         # This file — project documentation and content standards
└── insights/         # All published and draft articles
    ├── ai-strategy-basics.md
    ├── building-ai-team.md
    └── shopify-ai-success.md
```

All article files live in the `/insights` directory as individual Markdown files.

---

## Article Format

Every article is a `.md` file consisting of two parts: a **frontmatter block** and the **article body**.

### Frontmatter

Each file must begin with a YAML frontmatter block enclosed in `---` delimiters. All fields are required unless marked optional.

```yaml
---
title: "Article Title Here"
description: "One or two sentence summary shown in previews and SEO."
date: "YYYY-MM-DD"
readTime: "X min read"
category: "strategy"
author: "Sundar Rajan"
featured: false
image: "https://..."
imageAlt: "Descriptive alt text for the image"
---
```

#### Field Reference

| Field | Type | Description |
|---|---|---|
| `title` | string | Full article title. Keep under 70 characters for SEO. |
| `description` | string | Short summary for previews and meta description. 120–155 characters ideal. |
| `date` | string | Publication date in `YYYY-MM-DD` format. |
| `readTime` | string | Estimated reading time, e.g. `"6 min read"`. |
| `category` | string | One of the defined categories (see below). Use the slug value. |
| `author` | string | Author full name. Default: `"Sundar Rajan"`. |
| `featured` | boolean | Set `true` to surface the article as featured content. Limit to 1–2 at a time. |
| `image` | string | Full URL to the hero image. Recommended size: 1200×600px. |
| `imageAlt` | string | Descriptive alt text for accessibility and SEO. |

---

## Categories

Articles are organized into four categories. Use the slug value in the `category` frontmatter field.

| Category | Slug | Description |
|---|---|---|
| Strategy | `strategy` | AI strategy frameworks, prioritization models, and planning approaches for leaders making foundational AI decisions. |
| Implementation | `implementation` | Step-by-step guidance on deploying AI systems, running pilots, and integrating AI into existing workflows. |
| Case Studies | `case-study` | Real-world examples of companies implementing AI — what they did, what worked, and what didn't. |
| AI Workforce | `ai-workforce` | Guidance on hiring, structuring, managing, and scaling AI teams inside a company. |

---

## Writing Standards

### Content Structure

Each article should follow this general structure:

1. **Opening hook** — A sharp observation or problem statement that captures why this topic matters to a founder right now.
2. **The problem** — Concrete framing of what goes wrong without the right approach.
3. **The insight or framework** — The core actionable content, broken into clear phases or steps.
4. **Evidence or example** — A real-world case, data point, or illustration that validates the approach.
5. **Key takeaways** — 3–5 bullet points summarizing what the reader should walk away with.
6. **Next steps** — A concrete call to action or first step the reader can take immediately.

### Voice and Tone

- Write for a smart, time-constrained founder — not a technical audience.
- Be direct. Avoid hedging language ("it might be helpful to consider...").
- Use concrete numbers and timelines wherever possible.
- Prefer short paragraphs and scannable headers.
- Every section should earn its place — cut anything that doesn't add insight.

### File Naming Convention

Use lowercase, hyphen-separated slugs that match or relate to the article title.

```
# Good
ai-strategy-basics.md
building-ai-team.md
shopify-ai-success.md

# Avoid
AIStrategyBasics.md
article1.md
new_article_draft.md
```

### Images

Hero images are sourced from [Unsplash](https://unsplash.com). Use the following URL format to request a correctly sized image:

```
https://images.unsplash.com/photo-{PHOTO_ID}?w=1200&h=600&fit=crop
```

Always write a descriptive `imageAlt` value — describe what is visually in the image, not just the article topic.

---

## Adding a New Article

1. Create a new `.md` file inside `/insights/` using the naming convention above.
2. Add the complete frontmatter block at the top of the file.
3. Write the article body in Markdown, following the content structure guidelines.
4. Set `featured: false` unless this article is intended to lead the publication.
5. Verify the `date` field reflects the intended publication date.

---

## About the Author

**Sundar Rajan** writes about AI strategy and implementation for founders and executive leaders. Pagsun AI Insights is built on the belief that AI is not a technology problem — it's a strategy and leadership problem — and that the founders who understand this distinction will build the companies that define the next decade.
