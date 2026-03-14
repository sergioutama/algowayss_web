# Review Process Documentation

## Overview

This document defines the three-stage review process for all blog content before and after publication.

---

## Stage 1: Self-Review (Author)

### Timing
- **When**: Immediately after draft completion
- **Duration**: 15-30 minutes
- **Owner**: Content author

### Focus Areas

**Structure and Flow:**
- [ ] Read entire post aloud for natural flow
- [ ] Check that each section has single, clear purpose
- [ ] Verify transitions between sections are smooth
- [ ] Ensure conclusion reinforces key takeaway

**Content Quality:**
- [ ] Title is specific and compelling
- [ ] Opening hook creates immediate interest
- [ ] Main value proposition is clear within first 200 words
- [ ] All claims have supporting evidence or metrics
- [ ] Technical terms defined or explained on first use

**Tone and Voice:**
- [ ] Professional corporate tone maintained
- [ ] No slang, emojis, or informal language
- [ ] Appropriate for target audience (business or technical stakeholders)
- [ ] Consistent voice throughout entire post
- [ ] No over-promising or unrealistic claims

**Formatting:**
- [ ] Heading hierarchy is correct (H1 → H2 → H3)
- [ ] Lists and tables formatted properly
- [ ] No broken or invalid links
- [ ] Images have alt text
- [ ] No orphan paragraphs or awkward breaks

**Frontmatter:**
- [ ] All required fields present
- [ ] Date format is YYYY-MM-DD
- [ ] Categories and tags are valid
- [ ] Impact level is correct (high, medium, low)
- [ ] Description is 150-160 characters
- [ ] YAML syntax is valid

---

## Stage 2: Quality Gate (Before Publication)

### Timing
- **When**: Before scheduling publication
- **Duration**: 10-15 minutes
- **Owner**: Author with optional peer review

### Review Criteria Matrix

| Element | Weight | Pass Threshold | Notes |
|---------|--------|----------------|-------|
| Technical Accuracy | 30% | Zero errors | No incorrect technical claims |
| Clarity | 25% | Readable by target audience | No jargon without explanation |
| Value Density | 25% | ≥3 actionable insights | Clear business value |
| Formatting | 10% | Consistent throughout | Proper markdown, headings, lists |
| Grammar/Style | 10% | ≤3 minor issues | Professional writing quality |

### Scoring Process

1. **Review each element** against threshold
2. **Assign score** for each element (0-100%)
3. **Calculate weighted average** for overall score
4. **Require 80%+ overall score** to proceed to publication

### Pass/Fail Decision

**Pass criteria:**
- All critical issues (technical accuracy, major formatting errors) resolved
- Overall score ≥ 80%
- Frontmatter complete and valid
- File builds successfully in Jekyll

**Fail criteria:**
- Any critical technical error found
- Overall score < 80%
- Missing or invalid frontmatter
- Build errors in Jekyll

### Feedback Integration

**If corrections needed:**
1. Document issues in project template notes section
2. Make corrections to draft
3. Re-run self-review (Stage 1)
4. Proceed to quality gate (Stage 2) again

**If major rewrite needed:**
1. Identify root cause of issues (tone, structure, content)
2. Discuss with team for guidance
3. Plan revision approach
4. Complete revision before returning to review process

---

## Stage 3: Post-Publication Review

### Timing
- **When**: 48 hours after publication
- **Duration**: 10 minutes
- **Owner**: Content author or team lead

### Review Checklist

**Validation:**
- [ ] Post displays correctly in browser
- [ ] All images load properly
- [ ] Internal links work and point to correct destinations
- [ ] RSS feed includes the post
- [ ] Social media metadata renders correctly (OpenGraph, Twitter cards)

**Performance Monitoring:**
- [ ] Check Google Search Console for any indexing errors
- [ ] Monitor analytics for traffic and engagement
- [ ] Track social media shares and comments
- [ ] Note any user feedback or questions

**Issue Detection:**
- [ ] Scan for any formatting issues that appeared post-publish
- [ ] Check for broken links discovered by users
- [ ] Monitor for technical corrections or updates needed
- [ ] Track engagement metrics (views, time on page, bounce rate)

### Issue Resolution Protocol

**For minor issues (typos, formatting):**
1. Correct immediately without post-publication announcement
2. No correction note needed

**For moderate issues (inaccurate claims, broken links):**
1. Document issue in project file
2. Update published content within 24 hours
3. Add brief correction note if significant: *[Correction: Updated on DATE - What changed]*
4. Share correction on social media if post had significant engagement

**For major issues (incorrect technical information, misleading claims):**
1. Immediately unpublish post
2. Complete full review and rewrite
3. Re-publish with correction note
4. Announce correction prominently on all channels
5. Document lessons learned for future prevention

---

## Feedback Integration Process

### Handling Technical Corrections

**When errors are identified post-publication:**
1. **Document issue** in project template notes section with:
   - What was incorrect
   - Source of feedback (internal review, user comment, etc.)
   - Date discovered
   - Impact level (minor, moderate, major)

2. **Determine correction approach**:
   - Simple fix: Edit in place
   - Moderate fix: Add correction note
   - Major fix: Full rewrite required

3. **Implement correction** with appropriate timeline:
   - Minor: < 24 hours
   - Moderate: < 48 hours
   - Major: Emergency process

### Engagement Response Protocol

**For reader questions and comments:**
- Respond to all comments within 48 hours
- Document recurring questions for future content
- Update post FAQ section if common questions emerge
- Consider follow-up posts for popular topics

**For negative feedback:**
- Evaluate objectively against quality standards
- Identify valid feedback vs personal preference
- Incorporate valid feedback into future content guidelines
- Update content creation guide if recurring issues identified

---

## Review Documentation

### Review Log

Maintain a log of all reviews for continuous improvement:

| Date | Post Title | Reviewer | Stage | Score | Issues Found | Resolution |
|-------|-------------|------------|-------|-------|---------------|-------------|
| 2026-02-25 | Audio Compression | Author | Self | 95% | Minor typos fixed |
| 2026-02-25 | Audio Compression | Peer | Quality | 92% | Formatting adjusted |
| 2026-02-26 | Audio Compression | Author | Post-Pub | N/A | No issues found |

### Lessons Learned

Document recurring patterns and improvements:
- **Common issues**: Types of issues found frequently
- **Root causes**: Why issues occur (training, process gaps, etc.)
- **Process improvements**: Changes made to prevent recurrence
- **Training needs**: Knowledge gaps identified for team development

---

## Continuous Improvement

### Monthly Review

Each month, review the review process:
1. Calculate average scores across all posts
2. Identify most common issues
3. Evaluate if current process is effective
4. Adjust review criteria or weights as needed
5. Update documentation with process improvements

### Annual Review

Each year, conduct comprehensive process review:
1. Analyze year-long performance data
2. Compare against content quality goals
3. Gather team feedback on review process
4. Benchmark against industry best practices
5. Implement major process improvements if needed

---

## Quality Standards Summary

### Minimum Requirements for Publication

**Content Quality:**
- All technical claims accurate and verifiable
- Clear business value and impact articulated
- Measurable results or metrics included (case studies)
- Professional corporate tone throughout
- No code snippets or bash commands (high-level overview only)

**Formatting Quality:**
- Valid YAML frontmatter
- Correct markdown syntax
- Proper heading hierarchy
- Working internal links
- Alt text on all images

**SEO Quality:**
- Compelling, specific title
- Description 150-160 characters
- Primary keyword in title and first 100 words
- Internal linking to related content
- Validated with SEO checklist

### Excellence Indicators

Posts that demonstrate excellence typically have:
- Novel insights or unique perspectives
- Exceptional clarity and flow
- Actionable takeaways for readers
- Strong engagement metrics
- Positive external references or citations
