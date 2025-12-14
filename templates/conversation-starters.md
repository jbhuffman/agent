# Conversation Starters

## Purpose
Quick prompts that reliably produce good outputs with minimal back-and-forth.
Use these as copy/paste starters, then fill in blanks.

---

## Parameters Block (Optional but Recommended)

Include this block at the top of any prompt when you want tighter control.

Parameters:
- Audience: [who this is for]
- Length: [short / medium / long / word count]
- Formality: [low / medium / high]
- Humor: [none / light / moderate]
- Assertiveness: [soft / balanced / strong]
- Output Format: [bullets / paragraphs / checklist / template]

---

## Writing: LinkedIn (Personal)

Parameters:
- Audience: [peers / recruiters / general]
- Length: under [X] words
- Humor: light to moderate
- Assertiveness: balanced

Prompt:
“Use the LinkedIn Post Template (Professional, Personal).
Topic: [topic]
Point I want to land: [point]
Close with a soft invitation.”

Variation: more humorous, same intent  
“Same as above, increase dry humor without undercutting the point.”

Variation: more serious  
“Same as above, minimize humor and keep it direct.”

---

## Writing: LinkedIn (Business Page)

Parameters:
- Audience: [industry / role]
- Formality: medium
- Humor: light
- Assertiveness: balanced

Prompt:
“Use the LinkedIn Post Template (Business Page).
Problem: [problem]
What usually goes wrong: [anti-pattern]
Preferred approach: [approach]
CTA: soft invitation, no sales language.”

---

## Writing: Email (Client or Recruiter)

Parameters:
- Audience: [client / recruiter / hiring manager]
- Length: short
- Formality: medium
- Humor: none

Prompt:
“Draft an email.
Goal: [follow-up / set next steps / clarify scope / negotiate]
Must include:
- [bullet]
- [bullet]
Constraints: direct, calm, no em dashes.”

---

## Writing: Short Boundary Statement

Parameters:
- Audience: [client / team / manager]
- Length: very short
- Assertiveness: firm but respectful

Prompt:
“Write a boundary statement using the Personal Boundary Statement Template.
Context: [hours / urgency / scope creep]
Keep it calm and unambiguous.”

---

## Resume: Role Summary

Parameters:
- Audience: hiring manager
- Length: 3–4 lines
- Formality: high
- Humor: none

Prompt:
“Write a resume summary for this job description:
[paste JD]
Emphasize integrations, platform delivery, and leadership.
Avoid buzzwords.”

---

## Resume: Bullet Refresh

Parameters:
- Length: one sentence per bullet
- Formality: high

Prompt:
“Rewrite these resume bullets using the Resume Bullet Template.
Focus on outcomes and system impact.
Bullets:
- [bullet]
- [bullet]
- [bullet]”

---

## Architecture: Technical Explanation

Parameters:
- Audience: senior engineers
- Length: medium
- Output Format: structured sections

Prompt:
“Use Architecture Explanation Template (Technical Audience).
System: [system]
Goal: [goal]
Constraints: [time/budget/security]
Deliver:
- approach
- alternatives
- tradeoffs
- risks
- revisit triggers
- next steps”

---

## Architecture: Non-Technical Explanation

Parameters:
- Audience: CFO / COO / client
- Length: short
- Humor: none

Prompt:
“Use Architecture Explanation Template (Non-Technical Audience).
Explain: [system]
Include 1–2 real-world examples.”

---

## Integrations: Design a Flow

Parameters:
- Audience: technical
- Output Format: steps + failure modes

Prompt:
“Design an integration flow.
Source: [system]
Destination: [system]
Data: [entities]
Volume: [rough estimate]
Requirements: idempotency, retries, audit trail, observability.”

---

## Integrations: Mapping Strategy

Parameters:
- Output Format: bullets + rules

Prompt:
“Propose a mapping strategy.
Canonical model: [yes/no]
Key fields: [list]
Edge cases: [list]
Include validation and versioning.”

---

## Testing: Practical Test Plan

Parameters:
- Audience: engineers
- Output Format: checklist

Prompt:
“Create a testing plan aligned with our testing philosophy.
Component: [service/integration]
Risks: [top risks]
Include:
- unit tests
- integration tests
- minimal e2e tests
- what not to test”

---

## Observability: What to Log and Measure

Parameters:
- Output Format: bullets

Prompt:
“Define an observability plan.
System: [system]
Include:
- logs
- metrics
- tracing
- alerting priorities”

---

## Decisions: Choose Between Options

Parameters:
- Assertiveness: strong
- Output Format: recommendation + rationale

Prompt:
“Use the Decision Framework.
Decision: [A vs B]
Priorities: [list]
Constraints: [budget/time/skills]
Recommend one and give the smallest responsible next step.”

---

## Career: Evaluate a Role

Parameters:
- Audience: personal
- Humor: none

Prompt:
“Evaluate this role using the career guidance in the Decision Framework:
[paste JD]
Output:
- green flags
- red flags
- interview questions
- success criteria
- recommended stance”

---

## Consulting vs Corporate: Monthly Focus

Parameters:
- Time Horizon: 4 weeks
- Output Format: weekly plan

Prompt:
“Use the Decision Framework.
Given my current situation, propose a 4-week focus split between:
- job search
- consulting pipeline
- product building
Include what to cut.”

---

## Planning: Turn Chaos into a Plan

Parameters:
- Output Format: phased plan

Prompt:
“Turn this into a clear plan:
[describe chaos]
Output:
- 3 phases
- weekly milestones
- definition of done
- risks and mitigations
- next 3 actions”

---

## Debug: Output Feels Off

Parameters:
- Rewrite Passes: 1

Prompt:
“Use debug/debug-the-agent.md.
Issue: [tone / length / clarity / over-engineering]
Rewrite accordingly without changing intent.”
