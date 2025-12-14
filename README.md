# Agent Pack Usage
> Opinionated personal agent configuration. Shared as-is. Use what helps, ignore the rest.

## What this is
A small set of files that shape responses so they stay consistent across:
- writing
- system design
- decision-making
- delivery-style output

## Quick start
1) Upload these files into the GPT Knowledge section (or into a Project for a one-off session).
2) Start every serious session by saying what you want and what the output should look like.

## Session kickoff (recommended)
Start serious sessions with:

"Use my v1.0 agent defaults. Ask one clarifying question only if necessary, then proceed."

## Files and what they do
- agent/primer.md
  - Always-on identity, tone, defaults, and constraints.
- writing/writing-style.md
  - Voice and formatting rules for anything written.
- technical/architecture-defaults.md
  - Architecture bias, integration principles, cost discipline, and testing philosophy.
- decision/decision-framework.md
  - How to choose between options, plus career and consulting tradeoffs.
- templates/output-templates.md
  - Reusable skeletons for common deliverables.

## How to choose what to upload (if not using a Custom GPT)
- Writing task: primer + writing-style + templates
- Architecture task: primer + architecture-defaults (+ decision-framework if tradeoffs)
- Big decision: primer + decision-framework (+ architecture-defaults if technical)
- Mixed work (common): upload all five

## Versioning and Change Rules

Current version: v1.0  
Status: Stable daily driver

### What qualifies as a minor change (v1.x)
- Clarifying language
- Adding examples
- Tightening or refining constraints
- Adding templates or conversation starters
- Small tone adjustments

Rule:
If existing prompts still behave the same way, it is a minor change.

### What requires a major version bump (v2.0)
- Core tone or voice changes
- Reversing architectural or decision biases
- Changing the primary audience
- Adding constraints that alter default behavior

Rule:
If previously correct prompts now feel wrong, it is a major change.

### What does not belong in versioned files
- Client-specific rules
- Job-specific positioning
- Temporary experiments
- Emotional or situational adjustments

Those belong in:
- Project chats
- Session prompts
- Inline instructions

### How to update safely
1. Change one file at a time
2. Run at least one real task
3. Keep the change only if behavior improves
4. Revert without hesitation if it does not

## How to prompt for best results
Use one of these patterns:

### Writing
“Use the LinkedIn Post Template (Professional, Personal). Topic: ____. Point I want to land: ____. Keep it under ____ words.”

### Architecture
“Use Architecture Explanation Template (Technical Audience). Context: ____. Constraints: ____. Deliver: diagram-in-words + tradeoffs + next steps.”

### Decisions
“Use the Decision Framework. Options: A vs B. My priorities: ____. Recommend one, list tradeoffs, and give a smallest responsible next step.”

## Maintenance rules
- Keep files short and opinionated.
- Prefer updating templates over adding more files.
- When something feels off, use debug/debug-the-agent.md.
