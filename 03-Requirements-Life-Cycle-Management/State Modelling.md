# State Modelling (BABOK® Technique)

## What This Technique Is
State Modelling describes how an entity (e.g., account, case, transaction) moves through **different states** based on events and rules.

It answers:
- “What states can this item be in?”
- “What triggers a transition?”
- “What actions are allowed in each state?”

## Why This Technique Exists
Many defects come from unclear state behavior:
- actions allowed when they shouldn’t be
- missing transitions
- incorrect status reporting

State modelling improves clarity for:
- lifecycle management
- workflow automation
- exception handling

## When to Use
- Case management systems
- Approval workflows
- Transaction processing
- Any domain with statuses and transitions

## Example
Entity: Account
States: New → Active → Dormant → Closed
Triggers: Open account, no activity for 12 months, closure request

## How to Apply
1. Identify key states
2. Identify transitions and triggers
3. Define rules per state (allowed actions)
4. Add exception transitions
5. Validate with stakeholders

## Common Mistakes
- Missing exception states
- Too many states without value
- Not linking transitions to business rules

## Related Techniques
- Business Rules Analysis
- Use Cases
- Process Modelling

## Key Takeaway
State models make lifecycle rules visible and prevent “status confusion” defects.
