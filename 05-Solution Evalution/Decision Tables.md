# Decision Tables (BABOK® Technique)

## What This Technique Is

A Decision Table is a structured technique used to **define complex business rules** by mapping conditions to corresponding actions.

It is especially useful when:
- Multiple conditions exist
- Rules overlap
- Outcomes depend on combinations of inputs

---

## Why This Technique Exists

Business rules are often described verbally and become ambiguous.

Decision tables:
- Eliminate ambiguity
- Ensure rule completeness
- Make logic testable
- Improve communication between business and IT

---

## When to Use Decision Tables

- Complex eligibility or approval logic
- Pricing or fee calculation rules
- Compliance decision logic
- Risk and authorization scenarios

---

## How Decision Tables Work

A decision table consists of:
- Conditions (inputs)
- Condition values
- Actions (outputs)
- Rules (rows defining outcomes)

---

## Real-World Example (Banking / IT)

**Loan Approval Decision Table**

| Credit Score | Income Verified | Existing Debt | Approve Loan |
|-------------|----------------|---------------|--------------|
| High | Yes | Low | Yes |
| Medium | Yes | Low | Yes |
| Medium | No | Low | No |
| Low | Any | Any | No |

This prevents inconsistent interpretation of approval rules.

---

## Common Mistakes

- Too many conditions without simplification
- Missing default or fallback rules
- Not validating with SMEs
- Treating decision tables as implementation logic instead of business logic

---

## Key Takeaway

Decision tables turn complex logic into **clear, testable business rules**.
