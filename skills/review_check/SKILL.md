---
name: review-check
description: |
  Review the generated execution plan for missing sections, clarity, and structural completeness.
  Use when the agent needs a quality check before showing the final plan.
  Do NOT use to generate the plan itself.
---

# Review Check Skill

## When to use
- The plan is already written.
- The agent needs a quality gate.

## When not to use
- The plan has not been generated yet.
- The task is only extraction or planning.

## Workflow
1. Check required sections.
2. Look for missing or weak parts.
3. Return review notes or confirm the plan is structurally sound.
