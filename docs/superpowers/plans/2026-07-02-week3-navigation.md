# Week 3 Navigation Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Update the landing page for Week 3 and add Back/Next navigation across lesson HTML pages.

**Architecture:** Keep the existing static HTML structure. Add Week 3 lesson cards to `index.html`, then add a small shared navigation block inside each lesson template render output using `lessonData.week` and `lessonData.day`.

**Tech Stack:** Static HTML, CSS, vanilla JavaScript.

## Global Constraints

- Do not change lesson content or exercise data.
- Preserve the existing warm visual style and CSS naming convention.
- Keep navigation local to static files; no external dependency.

---

### Task 1: Update index and lesson navigation

**Files:**
- Modify: `index.html`
- Modify: `english-w1d1.html` through `english-w3d7.html`

**Interfaces:**
- Consumes: each lesson file's `lessonData.week` and `lessonData.day` values.
- Produces: landing page links for Week 3 and per-lesson navigation links.

- [ ] Step 1: Add Week 3 section to `index.html` after Week 2.
- [ ] Step 2: Change landing page copy from 14 days to 21 days.
- [ ] Step 3: Add CSS for `.eng-nav`, `.eng-nav-link`, and `.eng-nav-link.disabled` to each lesson file.
- [ ] Step 4: Add `lessonPath()` and `navHtml()` helper functions after `normalize()` in each lesson file.
- [ ] Step 5: Replace the existing end tip with `${navHtml()}`.
- [ ] Step 6: Verify all expected navigation links are present.
