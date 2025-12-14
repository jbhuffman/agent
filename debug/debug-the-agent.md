# Debug the Agent

## Purpose
A fast way to diagnose “why did it answer like that?” and steer outputs back to the intended defaults.

## Triage questions
1) What type of task is this?
   - writing
   - architecture
   - decision
   - mixed

2) Which file should be leading?
   - writing-style.md (writing)
   - architecture-defaults.md (architecture)
   - decision-framework.md (decisions)
   - templates.md (structure)

3) What went wrong?
   - too long
   - too vague
   - wrong tone
   - too salesy
   - too cautious
   - over-engineered
   - under-specified
   - missing tradeoffs
   - no next actions

## Fix commands (copy/paste)
### Tone drift
“Rewrite this with the writing-style.md voice. Keep the intent. Cut fluff. No em dashes.”

### Too long
“Compress by 30–50% while keeping the main point and the CTA style.”

### Too vague
“Replace abstractions with concrete nouns, steps, and examples. Add tradeoffs.”

### Over-engineered
“Re-solve this using architecture-defaults.md: fewer moving parts, managed services, clear contracts, idempotency.”

### Under-engineered
“Add the missing production concerns: error handling, observability, idempotency, security, and testing.”

### Missing decision clarity
“Use decision-framework.md. Recommend one option, justify it, list risks, and give a smallest responsible next step.”

### Template enforcement
“Use the exact template from templates/output-templates.md and fill it in. Do not invent a new structure.”

## Escalation rules
If output is still off after one rewrite:
- Ask for one missing constraint (time, audience, length, scope), then proceed.
- Offer two versions:
  - conservative and simple
  - bolder and more opinionated

## Quality bar checklist
Before finalizing:
- Is the point obvious on a skim?
- Are tradeoffs explicit when needed?
- Are next actions concrete?
- Does it sound like a senior practitioner, not a hype engine?
