# Quality Checklist for Blog Content

## Pre-Publication Checklist

Use this checklist before final approval and publication.

---

## Content Quality

### Title and Opening
- [ ] Title is specific and compelling (not generic)
- [ ] Opening hook creates immediate interest
- [ ] Main value proposition is clear within first 200 words
- [ ] Title includes primary keyword naturally
- [ ] Title is under 60 characters for SEO

### Body Structure
- [ ] Each section has a single, clear focus
- [ ] Conclusion reinforces key takeaway
- [ ] Flow is logical and easy to follow
- [ ] Transitions between sections are smooth
- [ ] No orphan paragraphs or awkward breaks

### Content Value
- [ ] Clear business value or impact stated
- [ ] Actionable insights or takeaways included
- [ ] Claims have supporting evidence or metrics
- [ ] Content is unique and original (not duplicate)
- [ ] Reader clearly benefits from reading

### Tone and Voice
- [ ] Professional corporate tone maintained
- [ ] No slang, emojis, or informal language
- [ ] Appropriate for target audience (business or technical)
- [ ] Consistent voice throughout entire post
- [ ] No over-promising or unrealistic claims

---

## Technical Accuracy

### Technical Claims
- [ ] All technical claims are accurate and verifiable
- [ ] No deprecated practices or technologies recommended
- [ ] Version numbers or dependencies noted if relevant
- [ ] Technical terms defined on first use or explained
- [ ] Security-sensitive information not exposed

### References and Sources
- [ ] All statistics have sources or data points
- [ ] Claims based on documented evidence
- [ ] Links to authoritative sources when appropriate
- [ ] No broken or invalid links
- [ ] References to internal documentation are accurate

---

## Readability

### Paragraph and Sentence Structure
- [ ] Paragraphs are 2-4 sentences max
- [ ] No walls of text (break up with headers/lists)
- [ ] Sentence length average is 15-20 words
- [ ] Active voice used in 90%+ of sentences
- [ ] No filler words (that, just, really, very)

### Formatting
- [ ] Headers are descriptive (not "Introduction", "Conclusion")
- [ ] Consistent header hierarchy (H1 → H2 → H3)
- [ ] Code blocks have language specified (if used, which is rare)
- [ ] Lists are properly formatted (bullets or numbers)
- [ ] Tables have headers and consistent alignment
- [ ] Emphasis (bold, italic) used sparingly and appropriately

### Definitions and Explanations
- [ ] Acronyms defined on first use
- [ ] Industry jargon explained or linked
- [ ] Complex concepts broken down for non-technical readers
- [ ] Examples provided when helpful
- [ ] No assumptions about reader knowledge

---

## Formatting

### Markdown Syntax
- [ ] Valid markdown throughout
- [ ] Proper heading hierarchy (no skipped levels)
- [ ] Lists formatted correctly (bullet points or numbered)
- [ ] Tables formatted with proper column alignment
- [ ] Links use descriptive anchor text (not "click here")
- [ ] No orphan or unpaired formatting characters

### Frontmatter
- [ ] All required fields present (title, date, categories, tags, impact, audience, description, image, author, layout)
- [ ] Date format is YYYY-MM-DD
- [ ] Categories are valid (case-study or dev-log)
- [ ] Impact is valid (high, medium, low)
- [ ] Audience is valid (business-stakeholders, technical-leaders, technical-stakeholders)
- [ ] Description is 150-160 characters
- [ ] YAML syntax is valid (can parse without errors)

### Visual Elements
- [ ] Images have descriptive alt text
- [ ] Image file names are descriptive (not "image1.png")
- [ ] Images optimized for web (under 200KB)
- [ ] No broken images or missing resources
- [ ] Images enhance content, not just decoration

---

## SEO and Meta Tags

### Page Meta
- [ ] Title tag is unique and descriptive (50-60 characters)
- [ ] Meta description is compelling (150-160 characters)
- [ ] Meta description includes call-to-action
- [ ] Canonical URL set correctly
- [ ] Viewport tag included for responsive design

### OpenGraph and Social Media
- [ ] og:title matches page title
- [ ] og:description matches meta description
- [ ] og:type is "article"
- [ ] og:url is correct canonical URL
- [ ] og:image is present (1200x630px recommended)
- [ ] twitter:card is "summary_large_image"
- [ ] twitter:title matches page title
- [ ] twitter:description matches meta description
- [ ] twitter:image matches og:image

### URL Structure
- [ ] URL contains primary keyword naturally
- [ ] URL uses hyphens (not underscores)
- [ ] URL is short and descriptive (under 60 characters)
- [ ] No unnecessary parameters or query strings
- [ ] Date-based URL structure (YYYY/MM/DD/)

### Structured Data
- [ ] Article schema implemented (JSON-LD or microdata)
- [ ] Author schema included (Person or Organization)
- [ ] Organization schema present
- [ ] Schema validates through Google testing tool
- [ ] Breadcrumb schema if applicable

---

## Content-Specific Criteria

### For Case Studies
- [ ] Problem-Solution-Result structure followed
- [ ] Quantifiable results highlighted (before/after metrics)
- [ ] Business value clearly stated
- [ ] Timeline or scope mentioned
- [ ] Key takeaways or lessons learned included
- [ ] No code snippets (high-level overview only)

### For Dev Logs
- [ ] Quick Overview section present
- [ ] What changed is clearly explained
- [ ] Why it matters section included
- [ ] Next steps defined
- [ ] Before/after metrics included if applicable
- [ ] No code snippets (high-level overview only)

---

## Technical Validation

### Jekyll Build
- [ ] Jekyll builds without errors: `bundle exec jekyll build`
- [ ] No liquid template errors
- [ ] Post renders correctly in preview
- [ ] Navigation and links work
- [ ] Images and assets load properly

### Link Validation
- [ ] All internal links work and point to correct destinations
- [ ] All external links open successfully
- [ ] No 404 errors on linked pages
- [ ] Anchor text is descriptive
- [ ] No excessive external linking

### Cross-Browser Check
- [ ] Post displays correctly in Chrome
- [ ] Post displays correctly in Firefox
- [ ] Post displays correctly in Safari
- [ ] Mobile responsive layout works
- [ ] No rendering issues or broken layout

---

## Post-Publication Checklist

### Promotion
- [ ] Shared on company LinkedIn with relevant hashtags
- [ ] Shared on Twitter/X with image and tagline
- [ ] Internal team notified of publication
- [ ] Included in email newsletter (if applicable)
- [ ] Linked from related existing posts

### Monitoring Setup
- [ ] Google Search Console property verified
- [ ] Google Analytics tracking confirmed
- [ ] Search Console shows no indexing errors
- [ ] RSS feed includes the post
- [ ] Social media metadata renders in link previews

### Engagement Tracking
- [ ] Comment notifications enabled
- [ ] Social media share tracking active
- [ ] Analytics goals set up for engagement
- [ ] Time on page and scroll depth tracked
- [ ] Bounce rate monitored

### Issue Monitoring
- [ ] Check for broken links weekly for first month
- [ ] Monitor for user feedback or questions
- [ ] Track social media comments and mentions
- [ ] Document any technical corrections needed
- [ ] Prepare update process if issues found

---

## Final Approval Criteria

### Minimum Requirements for Publication

**Content:**
- All content quality items checked and passed
- Technical accuracy verified
- Professional corporate tone maintained
- No code snippets (high-level overview only)

**Formatting:**
- Valid YAML frontmatter
- Correct markdown syntax
- Jekyll builds successfully
- All links working

**SEO:**
- SEO checklist items complete
- Meta tags properly set
- URL structure follows convention
- Structured data implemented

### Excellence Indicators

Posts that exceed minimum standards:
- Novel insights or unique perspectives
- Exceptional clarity and flow (readability score 95%+)
- 3+ actionable takeaways for readers
- Strong potential for social engagement
- Valuable external reference potential
- Meets all content-specific criteria at high level

---

## Scoring Guide

### Calculating Overall Score

| Category | Weight | Pass Items | Pass % | Score |
|-----------|--------|------------|---------|-------|
| Content Quality | 30% | X/Y | (X/Y × 30) |
| Technical Accuracy | 25% | X/Y | (X/Y × 25) |
| Readability | 20% | X/Y | (X/Y × 20) |
| Formatting | 15% | X/Y | (X/Y × 15) |
| SEO/Meta | 10% | X/Y | (X/Y × 10) |
| **Total** | **100%** | | **Total Score** |

### Score Interpretation

- **90-100%**: Excellent - Ready for publication
- **80-89%**: Good - Minor corrections needed
- **70-79%**: Acceptable - Moderate corrections needed
- **60-69%**: Needs Work - Significant revisions required
- **< 60%**: Inadequate - Full rewrite needed

### Publication Decision

**Publish if:**
- Total score ≥ 80%
- All critical items passed (technical accuracy, major formatting)
- No blocker issues found

**Revise if:**
- Total score 70-79%
- Moderate corrections needed but fixable
- No major structural changes required

**Reject/Rewrite if:**
- Total score < 70%
- Major structural or content issues
- Significant revisions required
