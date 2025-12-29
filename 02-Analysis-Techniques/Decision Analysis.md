# Decision Analysis (BABOK® Technique)

## 1. What This Technique Is

Decision Analysis is a technique used by Business Analysts to **evaluate options and support informed decision-making** by comparing alternatives against defined criteria.  
It helps determine **which option provides the most value** under given constraints.

Decision Analysis brings **objectivity and transparency** to decisions that might otherwise be driven by intuition or hierarchy.

---

## 2. Why This Technique Exists

Business decisions often involve:
- Multiple solution options
- Conflicting stakeholder priorities
- Trade-offs between cost, risk, value, and time

Decision Analysis exists to help a BA:
- Structure complex decisions
- Make evaluation criteria explicit
- Reduce bias and subjectivity
- Enable defensible, auditable decisions

BABOK includes this technique because **clear decisions lead to clear direction and execution**.

---

## 3. When to Use Decision Analysis

Decision Analysis is most effective when:
- Choosing between solution options
- Prioritizing initiatives or features
- Evaluating vendor or product options
- Making trade-offs under constraints
- Supporting executive decision-making

Common BA scenarios:
- Buy vs build decisions
- Vendor selection
- Technology platform selection
- Process improvement options

---

## 4. When NOT to Use Decision Analysis

Decision Analysis may not be necessary when:
- There is only one viable option
- Decisions are trivial or low impact
- Criteria and outcomes are already agreed

In such cases, **simple consensus or judgment** may suffice.

---

## 5. Common Decision Analysis Techniques (Detailed)

Decision Analysis often uses **structured evaluation techniques** to compare options objectively and transparently.  
These techniques help Business Analysts support **defensible decisions**, especially when trade-offs exist.

---

## 5.1 Weighted Scoring

Weighted Scoring evaluates options by **scoring them against predefined criteria**, where each criterion has a **weight based on importance**.

This technique is useful when not all criteria are equally important.

### How it works
1. Identify decision criteria (e.g., cost, risk, compliance, scalability)
2. Assign a weight to each criterion (total usually = 100%)
3. Score each option against each criterion
4. Multiply score × weight
5. Sum weighted scores to rank options

### When to use
- Multiple competing options exist
- Stakeholders disagree on priorities
- Objective comparison is required
- Decisions must be auditable

### Example (Banking / IT)

**Decision:** Select a reporting platform

| Criteria | Weight | Option A | Option B |
|--------|--------|----------|----------|
| Cost | 30% | 3 | 4 |
| Compliance | 40% | 5 | 3 |
| Scalability | 30% | 4 | 4 |

Weighted totals determine the preferred option.

### Advantages
- Objective and transparent
- Balances multiple priorities
- Easy to explain to stakeholders

### Limitations
- Weights can be subjective
- Requires consensus on scoring

---

## 5.2 Cost-Benefit Analysis

Cost-Benefit Analysis compares **expected costs against expected benefits** to determine whether an option delivers net value.

It answers the question:  
**“Is this worth doing?”**

### How it works
1. Identify all costs (implementation, operational, change)
2. Identify all benefits (financial and non-financial)
3. Quantify where possible
4. Compare total costs vs total benefits

### When to use
- Investment or funding decisions
- Business case development
- Regulatory or automation initiatives

### Example (Banking / IT)

**Option:** Automate reconciliation

- Costs: Tool licensing, development, training
- Benefits: Reduced manual effort, fewer errors, compliance improvement

### Advantages
- Strong financial justification
- Easy for executives to understand

### Limitations
- Intangible benefits can be hard to quantify
- Long-term benefits may be underestimated

---

## 5.3 Risk Analysis (Option-Level)

In Decision Analysis, Risk Analysis evaluates **likelihood and impact of risks associated with each option**, not overall project risk.

### How it works
1. Identify risks per option
2. Assess likelihood (Low / Medium / High)
3. Assess impact (Low / Medium / High)
4. Compare overall risk exposure

### When to use
- High-impact decisions
- Regulated environments
- Vendor or technology selection

### Example (Banking / IT)

| Option | Key Risk | Likelihood | Impact |
|------|----------|------------|--------|
| Build In-house | Skill gaps | Medium | High |
| Vendor Solution | Vendor dependency | High | Medium |

### Advantages
- Highlights hidden risks
- Prevents overly optimistic decisions

### Limitations
- Risk assessment can be subjective
- Requires good historical insight

---

## 5.4 Decision Matrix

A Decision Matrix is a **tabular technique** that compares options against criteria side-by-side.  
It may or may not include weights.

### How it works
- List options as rows
- List criteria as columns
- Score each option against criteria
- Compare totals or patterns

### When to use
- Early comparison of options
- Workshops and group decisions
- Visual stakeholder discussions

### Example (Simplified)

| Option | Cost | Risk | Compliance | Overall |
|------|------|------|------------|---------|
| Option A | Medium | Low | High | Strong |
| Option B | Low | Medium | Medium | Moderate |

### Advantages
- Simple and visual
- Good for workshops
- Easy to facilitate

### Limitations
- Less precise without weighting
- Can oversimplify complex decisions

---

## 5.5 Choosing the Right Decision Analysis Technique

| Decision Need | Recommended Technique |
|--------------|----------------------|
| Balance multiple priorities | Weighted Scoring |
| Financial justification | Cost-Benefit Analysis |
| Risk-sensitive decision | Risk Analysis |
| Group comparison | Decision Matrix |

---

## Key Takeaway

Decision Analysis techniques help Business Analysts:
- Replace opinion with structure
- Make trade-offs explicit
- Support confident, defensible decisions

The **choice of technique depends on decision complexity, risk, and stakeholder needs**.


---

## 6. How to Apply Decision Analysis – Step by Step

### Step 1: Define the Decision
Clearly state:
- What decision needs to be made
- The scope and constraints

### Step 2: Identify Options
List all viable alternatives.

### Step 3: Define Evaluation Criteria
Determine criteria such as:
- Cost
- Value
- Risk
- Feasibility
- Compliance

### Step 4: Weight Criteria (If Needed)
Assign relative importance to each criterion.

### Step 5: Score Each Option
Evaluate each option objectively against criteria.

### Step 6: Analyze Results
Compare scores and identify leading options.

### Step 7: Validate and Decide
Review results with stakeholders and confirm the decision.

---

## 7. Inputs

Typical inputs include:
- Business objectives
- Constraints and assumptions
- Stakeholder priorities
- Risk assessments
- Cost estimates

---

## 8. Outputs

Typical outputs include:
- Evaluated options
- Decision rationale
- Recommended solution
- Supporting analysis artifacts

---

## 9. Common Mistakes by Business Analysts

- Using unclear or subjective criteria
- Overcomplicating scoring models
- Ignoring stakeholder priorities
- Treating analysis as the decision itself
- Failing to document rationale

---

## 10. Real-World Example (Banking / IT)

**Scenario:** Selecting a reporting platform

Options include:
- Enhancing existing tools
- Purchasing a vendor solution
- Building a custom platform

Decision Analysis compares:
- Cost
- Time to implement
- Regulatory compliance
- Scalability

The outcome provides a clear, defensible recommendation.

---

## 11. Mapping to BABOK Knowledge Areas

Decision Analysis supports:
- Strategy Analysis
- Requirements Analysis and Design Definition
- Solution Evaluation

---

## 12. Interview Tips (For Job Interviews)

Example response:

> “I use decision analysis to objectively evaluate options against agreed criteria, ensuring decisions are transparent, defensible, and aligned with business objectives.”

---

## 13. Related Techniques

Often combined with:
- Prioritization
- Cost-Benefit Analysis
- Risk Analysis
- Workshops
- Brainstorming

---

## 14. Key Takeaways

- Decision analysis brings objectivity to complex choices
- Criteria and weighting must be agreed upfront
- Results support, not replace, stakeholder decisions
- Clear documentation improves buy-in and traceability
