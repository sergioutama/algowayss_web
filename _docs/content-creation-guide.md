# Content Creation Guide

## Overview

This guide establishes the process for creating high-quality blog content for Algowayss stakeholders.

---

## Pre-Writing Phase

### Topic Selection Criteria

Select topics that meet these criteria:
- Relevance score ≥ 7/10 from prioritized backlog
- Personal experience depth (can write 500+ words without external research)
- Audience pain point alignment verified
- Business impact clearly defined

### Research Protocol

**Before drafting:**
1. Check existing content library for overlap
2. Gather 2-3 reference sources maximum
3. Document key statistics/quotes with sources
4. Create outline before drafting

**Sources:**
- memory.md entries for technical context
- Git commit messages for timeline
- ADRs for decision rationale
- Project documentation for metrics

---

## Writing Phase

### Draft Structure Template

#### Case Studies (5 sections)
1. **Executive Summary** (2-3 sentences) - Problem statement and resolution
2. **The Problem** (2-3 paragraphs) - Business context and impact
3. **Our Approach** (2-3 paragraphs) - Strategy and key decisions
4. **Implementation** (2-3 paragraphs) - High-level solution overview
5. **Key Results** (1-2 paragraphs) - Metrics and business value

#### Dev Logs (4 sections)
1. **Overview** (2-3 sentences) - What was built/updated
2. **What We Built** (2 paragraphs) - Feature description and benefits
3. **Why It Matters** (2 paragraphs) - Business impact
4. **Next Steps** (1 paragraph) - What this enables

### Voice Guidelines

**Writing Style:**
- Use "we" for team perspective, "you" for reader direction (sparingly)
- Prefer active voice (90%+ of sentences)
- Technical terms: define on first use or link to documentation
- Sentence length: aim for 15-20 word average

**Tone:**
- Professional and corporate (no slang, no emojis, no informal language)
- Business stakeholder audience focus
- Clear and concise, avoid jargon where possible
- Measurable and specific (use numbers, percentages, metrics)

---

## Post-Writing Phase

### Self-Edit Checklist

After completing draft:
- [ ] Read aloud for flow and clarity
- [ ] Remove filler words (that, just, really, very)
- [ ] Verify all claims have evidence or metrics
- [ ] Check formatting consistency (headings, lists, tables)
- [ ] Validate all links work and point to correct destinations

### Content Quality Check

Before submission for review:
- [ ] Title is specific and compelling (not generic)
- [ ] Opening hook creates immediate interest
- [ ] Main argument/lesson is clear within first 200 words
- [ ] Each section has a single focus
- [ ] Conclusion reinforces key takeaway
- [ ] Call-to-action is present and appropriate

### Technical Validation

- [ ] No deprecated practices recommended
- [ ] All technical claims verified against documentation
- [ ] Version numbers/dependencies noted if relevant
- [ ] No security-sensitive information exposed

---

## Formatting Guidelines

### Markdown Structure

- Use H1 for title (automatically from frontmatter)
- Use H2 for major sections (Executive Summary, The Problem, etc.)
- Use H3 for subsections (rare, usually not needed)
- Use H4+ for sub-subsections (avoid, simplify structure instead)

### Lists and Tables

- Use bullet lists for itemized content
- Use numbered lists for sequential steps
- Use tables for before/after metrics comparisons
- Keep table width reasonable for mobile viewing

### Code and Technical Elements

**For blog posts:**
- NO code snippets (high-level overview only)
- NO bash commands
- Use architecture diagrams instead (if needed)
- Explain concepts, not implementation details

**Technical references:**
- Link to GitHub repos for interested readers
- Reference ADRs for architectural decisions
- Link to external documentation when needed

---

## Publication Workflow

### Draft Status

Track content through these stages:
1. **Draft** - Initial writing complete
2. **Review** - Self-edited and validated
3. **Quality Gate** - Checklist compliance verified
4. **Approved** - Final approval obtained
5. **Scheduled** - Publication date set
6. **Published** - Live on website
7. **Promoted** - Shared on social channels

### File Naming Convention

Blog post filenames must follow Jekyll convention:
```
_posts/YYYY-MM-DD-title-with-hyphens.md
```

Examples:
- `2026-02-25-audio-compression-optimization.md`
- `2026-02-26-multi-calendar-architecture.md`
- `2026-02-27-railway-deployment-patterns.md`

### Frontmatter Requirements

All blog posts must include complete frontmatter:
```yaml
---
layout: post
title: "Post Title"
date: YYYY-MM-DD
author: Algowayss Team
categories: [case-study] # or dev-log
tags: [tag1, tag2, tag3]
impact: high # or medium, low
audience: business-stakeholders # or technical-leaders, technical-stakeholders
description: "Brief description for SEO (150-160 characters)"
image: /img/placeholder.png
---
```

---

## Quality Standards

### Content Metrics

**Case Studies:**
- Word count: 800-1200 words
- Read time: 5-7 minutes
- Sections: 5 major sections
- Metrics: At least 3 quantifiable results

**Dev Logs:**
- Word count: 500-800 words
- Read time: 3-5 minutes
- Sections: 4 major sections
- Metrics: At least 1 quantifiable result

### SEO Requirements

- [ ] Primary keyword in title
- [ ] Meta description: 150-160 characters
- [ ] URL slug: topic-relevant, under 60 characters
- [ ] Internal links to related posts
- [ ] External links to authoritative sources
- [ ] Alt text on all images

---

## Common Pitfalls to Avoid

### Content Issues
- ❌ Generic or vague descriptions
- ❌ Missing business value or impact
- ❌ Technical jargon without explanation
- ❌ No measurable results or metrics
- ❌ Over-promising or unrealistic claims

### Formatting Issues
- ❌ Missing frontmatter or incomplete fields
- ❌ Incorrect date format (not YYYY-MM-DD)
- ❌ Broken or invalid links
- ❌ Inconsistent heading hierarchy
- ❌ Walls of text without breaks

### Tone Issues
- ❌ Too casual or informal
- ❌ Emojis or slang
- ❌ Second-person perspective (except sparingly)
- ❌ Industry buzzwords without substance
- ❌ Overly promotional or sales-focused

---

## Review Process

### Self-Review (15-30 minutes)
After completing draft:
1. Read entire post aloud for flow
2. Check for typos and grammar errors
3. Verify all claims have supporting evidence
4. Ensure tone is consistent throughout
5. Confirm all checklist items complete

### Quality Gate (10-15 minutes)
Before publication:
1. Verify all SEO checklist items complete
2. Check frontmatter is valid YAML
3. Test post renders correctly in Jekyll
4. Validate internal links work
5. Ensure images load correctly

### Post-Publication Review (48 hours after)
After publishing:
1. Check for comments or feedback
2. Monitor engagement metrics (views, time on page)
3. Verify no formatting issues in browser
4. Track social media engagement
5. Document any issues for future reference
