# Acceptance and Evaluation Criteria (BABOK® Technique)

## What This Technique Is
Acceptance and Evaluation Criteria define **how a requirement, solution component, or entire solution will be judged as successful**.  
They make “done” measurable by specifying **conditions, measures, or tests** that must be satisfied for acceptance.

- **Acceptance Criteria**: Used to confirm the solution meets requirements (often at feature/story level).
- **Evaluation Criteria**: Used to compare options/solutions (often during selection or decision-making).

## Why This Technique Exists
Many failures happen because teams agree on *what to build* but not *how success will be measured*.  
This technique prevents:
- Misinterpretation of requirements
- Endless rework (“it’s not what I meant”)
- Disputes during UAT
- Weak solution evaluation

## When to Use
- During requirements definition (to clarify expectations)
- During backlog grooming (to make stories testable)
- During solution selection (vendor or build vs buy)
- During UAT planning and sign-off

## How to Apply (Step-by-Step)
1. **Identify the requirement/feature to be accepted or evaluated**
2. **Define measurable conditions**
   - functional conditions (what it does)
   - quality conditions (performance, security)
3. **Specify boundaries and exceptions**
4. **Confirm testability**
   - “Can QA/UAT verify this objectively?”
5. **Validate with stakeholders**
6. **Use criteria consistently in testing and sign-off**

## Output Examples
### Acceptance Criteria Example (Story-Level)
Requirement: “User can reset password”
- Password reset link expires within 15 minutes
- User receives email within 60 seconds
- Password must meet complexity policy
- Audit log records reset attempt and outcome

### Evaluation Criteria Example (Option-Level)
Comparing vendor tools:
- Total cost of ownership
- Compliance certification support
- Integration effort
- Scalability and performance
- Support model and SLA

## Common Mistakes
- Criteria are vague (“easy”, “fast”, “good UI”)
- Criteria are added too late (after build)
- Criteria ignore exceptions and negative cases
- Criteria not aligned with business goals

## Related Techniques
- Acceptance Testing
- Non-Functional Requirements Analysis
- Decision Analysis
- Metrics and KPIs

## Key Takeaway
Clear criteria convert opinions into measurable outcomes and make acceptance objective.
