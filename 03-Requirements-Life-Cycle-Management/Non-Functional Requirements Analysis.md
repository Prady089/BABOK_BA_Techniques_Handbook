# Non-Functional Requirements Analysis (BABOK® Technique)

## What This Technique Is
Non-Functional Requirements (NFRs) define **how well** a solution must perform rather than what it does.

Common NFR categories:
- Performance (speed, throughput)
- Security (auth, encryption, access control)
- Availability (uptime, failover)
- Reliability (error rates)
- Usability (ease of use)
- Scalability (growth support)
- Maintainability (supportability)
- Compliance (audit, retention)

## Why This Technique Exists
Many solution failures come from missing NFRs:
- system is too slow
- security gaps appear
- audit requirements are missed
- solution cannot scale

BABOK includes this to ensure solutions meet quality and compliance expectations.

## When to Use
- Any system change or new build
- Regulated environments (banking, healthcare)
- Integrations and data platforms
- Customer-facing applications

## How to Apply (Step-by-Step)
1. Identify NFR categories relevant to the initiative
2. Elicit NFRs from stakeholders and standards (security, ops, compliance)
3. Convert NFRs into measurable statements
4. Define acceptance criteria and test methods
5. Validate trade-offs (performance vs cost, security vs usability)
6. Maintain NFRs through design and testing

## Example NFR Statements
- “System must respond within 2 seconds for 95% of transactions.”
- “Audit logs must be retained for 7 years.”
- “Role-based access must restrict approvals above limit thresholds.”

## Common Mistakes
- NFRs written vaguely (“fast”, “secure”)
- NFRs discovered late (post-production issues)
- No measurable test method
- Ignoring operational stakeholders (support teams)

## Related Techniques
- Acceptance and Evaluation Criteria
- Risk Analysis
- Interface Analysis
- Metrics and KPIs

## Key Takeaway
NFRs protect the solution’s quality, compliance, and operational success.
