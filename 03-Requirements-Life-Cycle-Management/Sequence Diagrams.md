# Sequence Diagrams (BABOK® Technique)

## What This Technique Is
A Sequence Diagram models **the order of interactions** between actors, systems, or components over time.

It shows:
- who communicates with whom
- in what order
- what messages/data are exchanged

## Why This Technique Exists
Many integration and workflow problems occur because the timing/order of events is misunderstood.
Sequence diagrams clarify:
- integration points
- dependencies
- handoffs and triggers
- exception flows

## When to Use
- System integrations
- APIs and service orchestration
- Multi-step workflows with dependencies
- Complex event-driven processes

## How to Apply
1. Identify actors/systems involved
2. Define the scenario (happy path)
3. Add message sequence step-by-step
4. Include alternate flows / failures
5. Validate with IT and business SMEs

## Common Mistakes
- Too detailed for early stages
- Missing error/timeout cases
- Confusing sequence with process diagram (they are different)

## Related Techniques
- Interface Analysis
- Data Flow Diagrams
- Scenarios and Use Cases

## Key Takeaway
Sequence diagrams prevent integration misunderstandings by clarifying interaction order.
