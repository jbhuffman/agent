# Architecture Defaults

## Core Philosophy
Build systems that can be understood six months later by someone who did not attend the original meetings.
That someone is often you.

Favor designs that survive contact with reality.

## Primary Biases
- Clarity over cleverness
- Explicit over implicit
- Boring over novel
- Delivered over perfect

If a design needs a long explanation, it is already on probation.

## Platform Preferences
- C# / .NET for core services
- Azure-native where it makes sense
- Managed services over self-hosted infrastructure
- APIs as first-class contracts, not side effects

Choose tools that reduce operational thinking, not increase it.

## Integration Principles
- Idempotency is non-negotiable
- Retries without idempotency are just bugs with optimism
- Canonical models over pass-through payloads
- Explicit mapping layers, even when they feel redundant

Integrations should be predictable, inspectable, and boring.

## Data and Contracts
- Schemas are contracts
- Versioning is expected, not a failure
- Backward compatibility beats breaking changes
- Validation happens at the edges

“Flexible” payloads tend to be flexible until they are not.

## Error Handling and Observability
- Errors should be explicit and actionable
- Logs should answer “what happened” without a debugger
- Correlation IDs everywhere
- Silent failures are unacceptable

If you cannot explain a failure from logs alone, the system is unfinished.

## Security Defaults
- Least privilege by default
- Secrets never live in code or config files
- Identity over keys whenever possible
- Secure by design, not by checklist

Security should be boring and assumed, not bolted on later.

## Cloud Cost and Resource Discipline
- Cost is a feature, not an afterthought
- Start with consumption-based services when viable
- Understand free tiers, quotas, and scaling cliffs
- Prefer fewer resources with clearer responsibility

Every architectural choice has a monthly price tag.
If you cannot explain the bill, the design is incomplete.

## Testing Philosophy
- Tests exist to enable change, not to impress dashboards
- Unit tests cover business logic and edge cases
- Integration tests validate contracts and mappings
- End-to-end tests are selective and purposeful

Mock what you own.
Verify what you do not.

If tests make refactoring harder instead of easier, they are working against you.

## Performance and Scale
- Optimize for correctness first
- Measure before tuning
- Design for scale, do not pre-optimize for it
- Cost awareness is part of performance

Fast and fragile is not a win.

## Anti-Patterns to Avoid
- “We will clean it up later”
- Over-generalized frameworks
- Magic configuration with no documentation
- Tight coupling disguised as convenience
- Single points of failure with optimistic monitoring

If it feels clever, double-check it.

## Real-World Examples
- A single well-documented Function App is often better than ten microservices with unclear ownership
- A canonical data model saves time even when upstream systems claim to be “standard”
- Paying slightly more for a managed service often costs less than operating a cheaper one poorly
- Logging early prevents late-night archaeology

Reality rewards boring consistency.

## Decision Heuristics
When choosing between options, prefer the one that:
- Is easier to explain to a client
- Has fewer moving parts
- Fails in obvious ways
- Can be fixed without heroics

Heroics do not scale.

## Documentation Expectations
- Architecture decisions get written down
- Tradeoffs are recorded, not hidden
- Diagrams favor readability over completeness

If it matters, document it. If it does not, delete it.
