# Content Extraction Process

## Overview
This document defines step-by-step process for extracting publishable stories from technical artifacts.

---

## Source 1: memory.md Patterns

### Step 1: Identify High-Value Entries
1. Scan memory.md for entries marked with business impact
2. Look for patterns: Problem, Solution, Result
3. Flag entries with quantifiable outcomes (percentages, metrics, cost savings)

### Step 2: Extract Story Elements

Extraction template:
- **technical_context**: What was the technical challenge?
- **business_impact**: How did this affect users/business?
- **timeline**: How long did this take to resolve?
- **stakeholders**: Who was affected?
- **outcome**: What was the measurable result?

### Step 3: Transform to Narrative
1. Convert technical jargon to business language
2. Focus on problem → solution → result arc
3. Remove code, keep concepts
4. Add context for non-technical readers

---

## Source 2: Git Commit Messages

### Step 1: Aggregate Related Commits

```bash
# Group commits by feature/fix
git log --oneline --grep="feat:" --since="2026-01-01"
git log --oneline --grep="fix:" --since="2026-01-01"
```

### Step 2: Identify Story Clusters
1. Group commits by feature branch or topic
2. Identify "why" behind the changes
3. Look for ADR references in commit messages

### Step 3: Extract Timeline
1. First commit = problem identification
2. Middle commits = solution iterations
3. Final commit = resolution

---

## Source 3: ADRs and Changelogs

### Step 1: Parse ADR Structure

ADR extraction:
- **title**: ADR-XXX: Decision Title
- **status**: accepted/superseded/deprecated
- **context**: Why was this decision needed?
- **decision**: What was decided?
- **consequences**: What are the impacts?

### Step 2: Transform ADR to Case Study
1. Context → Problem section
2. Decision → Solution section
3. Consequences → Results section

### Step 3: Cross-Reference
1. Link ADR to related memory.md entries
2. Find git commits that implemented the ADR
3. Gather metrics from deployment logs

---

## Quality Gates

Before publishing, verify:
- [ ] No sensitive information exposed
- [ ] Business value clearly stated
- [ ] Technical accuracy validated
- [ ] Stakeholder approval obtained
- [ ] SEO metadata complete
