# Contribution #3: Back to top button is cropped on mobile

**Contribution Number:** 3  
**Student:** Yuan Yuan  
**Issue:** https://github.com/pydata/pydata-sphinx-theme/issues/2411  
**My Fork:** https://github.com/yyccPhil/pydata-sphinx-theme  
**Status:** Phase I Complete

---

## Why I Chose This Issue

I chose this issue — a cropped "back to top" button on mobile in pydata-sphinx-theme — because it's small, clearly defined, and has an obvious "done" state, which makes it a realistic first open-source contribution rather than something that could balloon in scope. My background is mostly in Python, so this front-end bug stretches me in a useful direction: I'll need to dig into the theme's CSS and mobile breakpoints, which complements my existing skills instead of repeating them. Just as importantly, I want to learn the full contribution workflow end-to-end — setting up the project locally, reproducing a bug, opening a focused PR with before/after screenshots, and responding to maintainer feedback — in a mature, newcomer-friendly project. My real goal this cycle isn't just closing one issue, but getting comfortable enough with the process that a bigger one feels routine next time.

---

## Understanding the Issue

### Problem Description
On Firefox for Android using the classic three-button navigation bar, pydata-sphinx-theme's "back to top" button is cropped — the system navigation bar overlaps and cuts off part of the button, so it doesn't render fully. The problem only appears with button navigation, not with the iOS-like gesture navigation that is now the default on several Android devices, and it was introduced in version 0.15.4. This matters because on long documentation pages the back-to-top control is a key mobile navigation aid, and a half-hidden, hard-to-tap button hurts usability for a real slice of Android users. I chose it because it's a well-scoped, reproducible CSS bug that lets me learn the full contribution workflow without risking scope creep.

### Expected Behavior
The "back to top" button should render fully and remain tappable on mobile, sitting clear of the on-screen navigation bar regardless of whether the device uses button navigation or gesture navigation.

### Current Behavior
On Firefox/Android with three-button navigation, the bottom portion of the "back to top" button is clipped by the system navigation bar, leaving part of the control cut off. (Reported against PST 0.20.0; regression introduced in 0.15.4.)

### Affected Components
The CSS/SCSS that controls the positioning and bottom offset of the "back to top" button, plus the mobile viewport handling for the on-screen navigation bar (likely involving the button's bottom spacing and safe-area / viewport-height behavior). Exact file(s) to be confirmed during reproduction.

---

## Reproduction Process

### Environment Setup
[Notes on setting up your local development environment - challenges you faced, how you solved them]

### Steps to Reproduce
1. [Step 1]
2. [Step 2]
3. [Observed result]

### Reproduction Evidence
- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach

### Analysis
[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution
[High-level description of your fix approach]

### Implementation Plan
Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]
1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests
- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests
- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing
[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress
[What you built this week, challenges faced, decisions made]

### Week [Y] Progress
[Continue documenting as you work]

### Code Changes
- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained
[What you learned technically]

### Challenges Overcome
[What was hard and how you solved it]

### What I'd Do Differently Next Time
[Reflection on your process]

---

## Resources Used
- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
