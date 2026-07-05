---
name: plan-generation
description: |
  Generate a clear execution plan from extracted brief facts.
  Use when the agent needs a summary, task breakdown, risks, and next steps.
  Do NOT use for raw fact extraction.
---

# Plan Generation Skill

## When to use
- The brief has already been analyzed.
- The user wants a usable plan or project outline.

## When not to use
- The input has not yet been summarized.
- The task is only to identify facts.

## Workflow
1. Review extracted facts.
2. Convert them into a markdown execution plan.
3. Include tasks, risks, and next steps.
