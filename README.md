# Brief-to-Plan Agent

## What this project does
Brief-to-Plan Agent turns messy project briefs, meeting notes, or feature requests into a clean execution plan.

## Why this is useful
Teams often receive vague requests that are hard to turn into action. This agent helps by extracting the goal, identifying missing information, and producing a structured markdown plan with tasks, assumptions, risks, and next steps.

## How it works
1. The user pastes a brief.
2. The agent extracts key facts.
3. The agent generates a structured plan.
4. The agent reviews the result for completeness.
5. The final output is displayed and saved as markdown.

## Architecture
- Orchestrator: runs the full pipeline
- brief-analysis skill: extracts facts from the brief
- plan-generation skill: turns facts into a plan
- review-check skill: checks structure and completeness
- MCP-style tool layer: provides sample briefs and templates

## Course concepts used
- Agent / multi-agent style pipeline
- Agent skills
- Tool layer / MCP-style integration
- Security-minded human review
- Evaluation checks for output structure

## Files
- `specs/brief_to_plan_spec.md`
- `skills/brief_analysis/SKILL.md`
- `skills/plan_generation/SKILL.md`
- `skills/review_check/SKILL.md`
- `outputs/sample_plan_1.md`

## How to run
Run the notebook cells in order:
1. Spec and problem statement cells
2. Baseline plan generator
3. Review checker
4. Tool layer setup
5. Skill setup
6. End-to-end pipeline
7. Demo cell

## Evaluation
The project is checked by:
- verifying all required output sections exist
- testing multiple sample briefs
- checking that the plan stays structured and readable

## Limitations
This version uses simple logic for the first prototype. It can be improved later by adding stronger retrieval, richer agent reasoning, or a real UI.

## Next improvements
- add a richer front end
- add more sample briefs
- improve the review step
- connect the workflow to a stronger MCP server
