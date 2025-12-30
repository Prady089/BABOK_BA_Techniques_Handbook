# Scenarios and Use Cases (BABOK® Technique)

## What This Technique Is
Scenarios and Use Cases describe **how users interact with a system** to achieve a goal.

- **Scenario**: narrative example of usage (often informal)
- **Use Case**: structured description including actors, steps, preconditions, and alternate flows

## Why This Technique Exists
Requirements are clearer when expressed as interactions and outcomes, especially when:
- workflows have exceptions
- multiple actors are involved
- system behavior matters

## When to Use
- Workflow-heavy systems
- Systems with many exceptions (banking ops)
- Integration-heavy processes
- Clarifying responsibilities between roles

## Use Case Structure (Typical)
- Name and goal
- Actors
- Preconditions
- Main success flow
- Alternate flows / exceptions
- Postconditions

## Example (Banking / IT)
Use Case: “Approve Transaction Above Limit”
- Actor: Approver
- Preconditions: user authenticated, transaction pending
- Main flow: review → validate limit → approve → audit log created
- Exceptions: insufficient permissions → reject with reason

## Common Mistakes
- Overly detailed use cases too early
- Missing alternate flows
- Writing use cases as UI instructions rather than behavior

## Related Techniques
- Acceptance Criteria
- Process Modelling
- Prototyping
- User Stories

## Key Takeaway
Scenarios and use cases turn vague needs into clear behavior and exception handling.
