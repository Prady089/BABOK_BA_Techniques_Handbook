# Acceptance and Evaluation Criteria

## Overview

**Definition:** Acceptance and Evaluation Criteria define the specific, measurable conditions that a requirement, solution component, or entire solution must satisfy to be considered complete and acceptable by stakeholders.

**Purpose:** This technique transforms subjective expectations into objective, testable conditions that enable clear communication, reduce ambiguity, and provide a concrete basis for determining when work is "done" or which solution option is best.

**Scope:** Applied at multiple levels—from individual user stories to entire solution evaluations—this technique bridges the gap between what stakeholders want and how teams verify they've delivered it.

---

## Key Concepts

### Acceptance Criteria
Conditions that must be met for a requirement, feature, or deliverable to be accepted by stakeholders. They answer: "How will we know this requirement has been successfully implemented?"

**Characteristics:**
- Specific and unambiguous
- Testable and verifiable
- Written from the user/business perspective
- Include both positive and negative scenarios
- Define boundaries and constraints

### Evaluation Criteria
Standards used to assess and compare alternative solutions, options, or approaches. They answer: "How will we decide which option is best?"

**Characteristics:**
- Aligned with business objectives
- Weighted by importance
- Quantifiable where possible
- Cover multiple dimensions (cost, quality, risk, etc.)
- Enable objective comparison

### The Distinction
- **Acceptance Criteria** = "Did we build it right?" (verification/validation)
- **Evaluation Criteria** = "Did we choose the right thing?" (decision-making)

---

## Why This Technique Matters

### Problems This Technique Solves

1. **Ambiguous Requirements**
   - Stakeholders and delivery teams interpret requirements differently
   - "User-friendly" means different things to different people
   - Technical teams build what they think is needed, not what stakeholders expect

2. **Failed Acceptance**
   - Solutions rejected during UAT because expectations weren't clear
   - Endless revision cycles: "That's not what I meant"
   - Disputes about whether requirements have been met

3. **Poor Decision-Making**
   - Solution options compared on gut feeling rather than objective measures
   - Post-implementation regret: "We should have chosen the other vendor"
   - Inability to justify decisions to leadership

4. **Testing Gaps**
   - Test cases don't align with actual business needs
   - QA doesn't know what "pass" looks like
   - Defects escape to production because success wasn't defined

### Benefits of Using This Technique

- **Shared Understanding:** Everyone agrees on what "done" looks like before work begins
- **Reduced Rework:** Clear targets minimize interpretation errors and false starts
- **Objective Testing:** QA can create comprehensive test cases directly from criteria
- **Faster Acceptance:** UAT proceeds smoothly when expectations are pre-defined
- **Better Decisions:** Evaluation criteria enable transparent, defensible solution selection
- **Traceability:** Links requirements → criteria → tests → acceptance in a clear chain

---

## When to Use This Technique

### BABOK Knowledge Areas
- **Requirements Analysis and Design Definition** (primary)
- **Requirements Life Cycle Management**
- **Solution Evaluation**
- **Strategy Analysis** (for strategic options)

### Project Lifecycle Timing

| Phase | Application |
|-------|-------------|
| **Initiation/Planning** | Define evaluation criteria for solution approach selection |
| **Requirements Elicitation** | Clarify acceptance criteria as requirements are discovered |
| **Requirements Analysis** | Formalize criteria to make requirements testable |
| **Design** | Refine criteria based on design constraints and feasibility |
| **Development** | Guide development and create test cases |
| **Testing** | Execute tests against defined criteria |
| **UAT/Acceptance** | Formal sign-off based on satisfied criteria |
| **Post-Implementation** | Evaluate actual performance against acceptance criteria |

### Specific Scenarios

**Use Acceptance Criteria when:**
- Writing user stories for agile backlogs
- Defining requirements in a business requirements document
- Planning UAT sessions
- Creating test cases and test plans
- Resolving disputes about whether functionality is complete
- Preparing for sprint reviews or demos

**Use Evaluation Criteria when:**
- Comparing vendor solutions (build vs. buy decisions)
- Selecting between design alternatives
- Prioritizing requirements or features
- Assessing proposals or bids
- Making go/no-go decisions on projects or phases
- Conducting feasibility studies

---

## How to Apply This Technique

### Step-by-Step Process

#### For Acceptance Criteria

**Step 1: Identify the Requirement or Feature**
- Start with a clear requirement statement (user story, use case, business requirement)
- Ensure the requirement itself is properly defined before creating criteria
- Example: "As a customer, I want to reset my password so I can regain access to my account"

**Step 2: Define Functional Conditions**
- What specific behaviors or outcomes must occur?
- Consider the happy path first, then alternatives
- Use concrete, observable actions

Example:
- User can request password reset from login page
- User receives reset email with unique link
- User can set new password meeting complexity requirements
- User can log in immediately with new password

**Step 3: Define Quality and Non-Functional Conditions**
- Performance: How fast? How many concurrent users?
- Security: What data protection measures?
- Usability: What accessibility standards?
- Compliance: What regulations or policies apply?

Example:
- Reset email delivered within 60 seconds
- Reset link expires after 15 minutes
- Password must contain 8+ characters, including uppercase, lowercase, number, symbol
- Process complies with GDPR data handling requirements

**Step 4: Specify Boundaries and Exceptions**
- What should NOT happen?
- What are edge cases or error conditions?
- What are limits or constraints?

Example:
- User cannot reset password more than 3 times per hour
- Expired links display clear error message
- Invalid passwords show specific validation errors
- System locks account after 5 failed reset attempts

**Step 5: Confirm Testability**
- Can each criterion be verified objectively?
- Does QA have the tools/access to test it?
- Are measurements specific enough?

Red flags:
- ❌ "System should be fast" → ⚠️ Not testable
- ✅ "Login page loads within 2 seconds for 95% of requests" → ✓ Testable

**Step 6: Review and Validate with Stakeholders**
- Walk through criteria with product owner, users, QA, developers
- Confirm criteria match their definition of "done"
- Adjust based on feedback
- Get formal agreement before development begins

**Step 7: Document and Link to Requirements**
- Record criteria in requirements management tool or story
- Ensure traceability between requirement → criteria → tests
- Keep criteria visible and accessible to entire team

#### For Evaluation Criteria

**Step 1: Define the Decision Context**
- What decision needs to be made?
- What options are being evaluated?
- Who will use these criteria to decide?

Example: "Select a CRM system from 3 vendor options"

**Step 2: Identify Evaluation Dimensions**
- What factors matter to stakeholders?
- Consider: cost, functionality, risk, strategic fit, technical fit
- Group related factors into categories

Example Categories:
- Financial (TCO, licensing, implementation cost)
- Functional (features, integration, customization)
- Technical (scalability, performance, security)
- Organizational (vendor stability, support, training)
- Risk (implementation complexity, change management)

**Step 3: Define Specific Measurable Criteria**
- For each dimension, create concrete measures
- Specify how each criterion will be assessed
- Define the scale or scoring method

Example:
| Criterion | Measurement Method | Scale |
|-----------|-------------------|-------|
| Total Cost of Ownership (5 years) | Financial analysis | Actual $ amount |
| Integration with existing ERP | Technical assessment | 1-5 (1=custom dev required, 5=native integration) |
| User adoption time | Vendor data + references | Days to 80% proficiency |
| Vendor financial stability | Credit rating + revenue analysis | Low/Medium/High risk |

**Step 4: Assign Weights to Criteria**
- Not all criteria are equally important
- Assign percentage weights based on stakeholder priorities
- Ensure weights sum to 100%

Example:
- Total Cost of Ownership: 30%
- Feature completeness: 25%
- Integration capability: 20%
- Implementation risk: 15%
- Vendor support quality: 10%

**Step 5: Define Scoring Method**
- How will each option be scored against each criterion?
- Common approaches: numerical scale (1-5), pass/fail, actual values
- Document scoring guidelines to ensure consistency

**Step 6: Evaluate Options and Calculate Results**
- Score each option against each criterion
- Apply weights to scores
- Calculate total weighted scores
- Document rationale for each score

**Step 7: Validate and Decide**
- Review results with decision-makers
- Perform sensitivity analysis (what if weights change?)
- Consider qualitative factors not captured in scores
- Document final decision and rationale

---

## Inputs and Outputs

### Inputs

**For Acceptance Criteria:**
- Requirements (user stories, use cases, business requirements)
- Business rules and policies
- Regulatory/compliance requirements
- Quality attributes and NFRs
- Stakeholder expectations
- Similar historical requirements and their criteria

**For Evaluation Criteria:**
- Business objectives and strategy
- Decision context and options
- Stakeholder priorities
- Organizational constraints
- Risk tolerance
- Budget and resource constraints

### Outputs

**Acceptance Criteria Deliverables:**
- Documented criteria within requirements (user stories, BRD, FRD)
- Acceptance test plans derived from criteria
- Definition of Done (DoD) for sprints or releases
- UAT scripts and checklists
- Sign-off documentation templates

**Evaluation Criteria Deliverables:**
- Evaluation criteria matrix (criteria × options)
- Weighted scoring models
- Comparison scorecards
- Decision analysis reports
- Recommendation documents with justification
- Vendor selection documentation

---

## Practical Examples

### Example 1: User Story Acceptance Criteria (E-commerce)

**User Story:**
"As a registered customer, I want to save items to a wishlist so I can purchase them later."

**Acceptance Criteria:**

*Functional:*
- User can add any in-stock item to wishlist from product detail page
- User can add any in-stock item to wishlist from search results
- User can view wishlist from account menu
- User can remove items from wishlist
- User can move items from wishlist directly to cart
- Wishlist displays: item name, image, current price, availability status
- Wishlist persists across sessions (saved to user account)

*Quality/Non-Functional:*
- Wishlist page loads within 3 seconds
- Wishlist supports up to 100 items per user
- Price updates reflect current pricing in real-time
- Wishlist available on mobile responsive design

*Boundary/Exception:*
- Out-of-stock items remain in wishlist but show "unavailable" status
- Deleted products are automatically removed from wishlist with notification
- Guest users cannot create wishlists (redirected to login/register)
- Wishlist is private (not shareable in this release)

**How These Criteria Are Used:**
- Developers know exactly what to build
- QA creates 15+ test cases covering all scenarios
- Product owner can verify each criterion during sprint review
- UAT testers have clear checklist for acceptance

---

### Example 2: Solution Evaluation Criteria (HR System Selection)

**Decision:** Select new HRIS (Human Resources Information System) from 3 vendors

**Evaluation Criteria Matrix:**

| Criterion | Weight | Measurement Method | Vendor A | Vendor B | Vendor C |
|-----------|--------|-------------------|----------|----------|----------|
| **Financial** | | | | | |
| Total Cost of Ownership (5yr) | 20% | Actual cost | $450K (4) | $380K (5) | $520K (3) |
| **Functional** | | | | | |
| Core HR features completeness | 25% | Feature checklist (1-5) | 5 | 4 | 5 |
| Payroll integration | 15% | Integration assessment | 3 | 5 | 4 |
| Reporting/analytics capability | 10% | Demo evaluation | 4 | 3 | 5 |
| **Technical** | | | | | |
| Scalability (support growth to 5000 employees) | 5% | Technical specs | 5 | 5 | 4 |
| Security certifications | 10% | Compliance documentation | 5 | 4 | 5 |
| **Organizational** | | | | | |
| Implementation timeline | 5% | Vendor proposal | 4 | 3 | 4 |
| Training and change management support | 5% | Service offering review | 3 | 4 | 5 |
| Vendor stability/references | 5% | Reference checks, financial analysis | 5 | 3 | 4 |
| **Weighted Total Score** | **100%** | | **4.30** | **4.15** | **4.45** |

**Scoring Scale:** 1 = Does not meet needs, 2 = Partially meets, 3 = Meets minimum, 4 = Exceeds, 5 = Significantly exceeds

**Decision Outcome:**
Vendor C selected based on highest weighted score, with particular strength in analytics (strategic priority) and strong security posture. Higher cost justified by superior functionality and better alignment with 5-year growth plans.

**Sensitivity Analysis:**
If cost weight increased to 30% (reducing functional weights), Vendor B would score highest. Decision validated with executive team that functionality > cost for this strategic system.

---

### Example 3: NFR Acceptance Criteria (System Performance)

**Requirement:**
"The customer portal must provide acceptable performance during peak usage periods."

**Acceptance Criteria (Making it Measurable):**

*Response Time:*
- Homepage loads within 2 seconds for 95th percentile of requests
- Search results display within 3 seconds for 90th percentile
- Account dashboard loads within 2.5 seconds for 95th percentile
- Transaction processing completes within 5 seconds for 98th percentile

*Throughput:*
- System supports 500 concurrent users without degradation
- System handles 50 transactions per second sustained load
- System handles 100 transactions per second peak load for up to 15 minutes

*Availability:*
- System uptime: 99.5% monthly (excluding planned maintenance)
- Planned maintenance windows: Sunday 2am-6am only, max 1x per month
- Recovery Time Objective (RTO): 4 hours for critical failures
- Recovery Point Objective (RPO): 15 minutes data loss maximum

*Scalability:*
- Performance criteria remain valid with 2x current user base (1000 concurrent users)
- System can scale horizontally by adding application servers
- Database can handle 5 million customer records without redesign

**Test Approach:**
- Load testing with JMeter simulating 500-1000 concurrent users
- Monitoring with APM tools during UAT and initial production period
- Performance regression testing in CI/CD pipeline
- Quarterly performance reviews against baseline

---

### Example 4: API Acceptance Criteria (Technical Requirement)

**Requirement:**
"Provide REST API for third-party partners to check order status"

**Acceptance Criteria:**

*Functional:*
- Endpoint: GET /api/v1/orders/{orderId}/status
- Authentication: OAuth 2.0 bearer token required
- Response includes: order ID, status, timestamp, items summary, tracking number (if shipped)
- Returns 200 for valid requests, 404 for non-existent orders, 401 for unauthorized, 403 for access to other company's orders
- Supports query parameter: ?includeHistory=true (returns status history)

*Data Quality:*
- Status updates reflect in API within 5 minutes of warehouse system update
- Data format: JSON conforming to published schema (v1.2)
- Date/time fields in ISO 8601 format with timezone
- Monetary values include currency code

*Security:*
- Rate limiting: 100 requests per minute per API key
- TLS 1.2 or higher encryption required
- API keys expire after 90 days
- No PII exposed beyond necessary order details (email masked)

*Performance:*
- Average response time: <500ms
- 99th percentile response time: <2 seconds
- API uptime: 99.9% monthly

*Documentation:*
- OpenAPI 3.0 specification published
- Developer guide with examples published
- Sandbox environment available for partner testing

**Integration Testing:**
- 3 pilot partners successfully integrate and test in sandbox
- All test scenarios in test suite pass (120+ test cases)
- Security penetration testing completed with no high-severity findings

---

## Templates and Formats

### Template 1: User Story Acceptance Criteria (Agile)

```markdown
## User Story
As a [role], I want [feature] so that [benefit].

## Acceptance Criteria

### Functional Criteria
- [ ] [Specific behavior or outcome 1]
- [ ] [Specific behavior or outcome 2]
- [ ] [Specific behavior or outcome 3]

### Quality Criteria
- [ ] Performance: [specific measure]
- [ ] Security: [specific requirement]
- [ ] Usability: [specific standard]

### Boundary Conditions
- [ ] [What happens in error scenario 1]
- [ ] [What happens at limits/constraints]
- [ ] [What should NOT happen]

## Definition of Done
- [ ] All acceptance criteria pass testing
- [ ] Code reviewed and approved
- [ ] Automated tests created and passing
- [ ] Documentation updated
- [ ] Product owner accepts in sprint review
```

---

### Template 2: Solution Evaluation Criteria Matrix

```markdown
## Decision: [State the decision to be made]

## Options Being Evaluated
1. [Option A]
2. [Option B]
3. [Option C]

## Evaluation Criteria

| Category | Criterion | Weight | Measurement Method | Option A Score | Option B Score | Option C Score |
|----------|-----------|--------|-------------------|----------------|----------------|----------------|
| [Category 1] | [Criterion 1.1] | XX% | [How measured] | [Score] | [Score] | [Score] |
| | [Criterion 1.2] | XX% | [How measured] | [Score] | [Score] | [Score] |
| [Category 2] | [Criterion 2.1] | XX% | [How measured] | [Score] | [Score] | [Score] |
| **Total** | | **100%** | | **[Weighted Total]** | **[Weighted Total]** | **[Weighted Total]** |

## Scoring Scale
- 1 = [Description]
- 2 = [Description]
- 3 = [Description]
- 4 = [Description]
- 5 = [Description]

## Recommendation
[Based on evaluation, which option is recommended and why]

## Sensitivity Analysis
[How robust is this decision if weights or scores change slightly?]

## Risks and Considerations
[Qualitative factors not fully captured in scoring]
```

---

### Template 3: NFR Acceptance Criteria

```markdown
## Non-Functional Requirement: [Name]

### Performance Criteria
- **Response Time:** [specific measure with percentile]
- **Throughput:** [transactions/requests per time period]
- **Concurrency:** [number of concurrent users/sessions]
- **Resource Utilization:** [CPU, memory, storage limits]

### Availability/Reliability Criteria
- **Uptime:** [percentage, time period]
- **MTBF:** [Mean Time Between Failures]
- **MTTR:** [Mean Time To Recovery]
- **RTO/RPO:** [Recovery objectives]

### Scalability Criteria
- **User Growth:** [system handles X users now, must support Y users in Z timeframe]
- **Data Volume:** [current and projected data volumes]
- **Geographic Distribution:** [number of locations, latency requirements]

### Security Criteria
- **Authentication:** [mechanism, standards]
- **Authorization:** [access control model]
- **Encryption:** [data at rest, in transit requirements]
- **Compliance:** [regulations, standards to meet]

### Usability Criteria
- **Accessibility:** [WCAG level, specific standards]
- **Browser/Device Support:** [specific versions, responsive requirements]
- **Training Time:** [time to proficiency for typical user]

### Testability
- **How These Will Be Verified:** [load testing, security testing, usability testing approaches]
- **Success Criteria:** [what passing looks like]
- **Test Environment:** [requirements for realistic testing]
```

---

## Common Mistakes and How to Avoid Them

### Mistake 1: Vague or Subjective Criteria

**Problem:**
- "System should be user-friendly"
- "Performance should be good"
- "Solution should be cost-effective"

**Why It's a Problem:**
- Everyone interprets differently
- Not testable objectively
- Leads to disagreement during acceptance

**How to Fix:**
- Replace subjective terms with measurable specifics
- ❌ "User-friendly" → ✅ "New user completes first transaction within 5 minutes without help documentation"
- ❌ "Fast" → ✅ "Loads within 2 seconds for 95% of requests"
- ❌ "Cost-effective" → ✅ "TCO under $500K over 5 years"

---

### Mistake 2: Criteria Added Too Late

**Problem:**
- Criteria defined during UAT or after development
- Team says "we thought done meant X" and stakeholders say "no, we meant Y"

**Why It's a Problem:**
- Rework is expensive and demoralizing
- Testing is incomplete because criteria weren't known
- Scope creep disguised as "clarifying requirements"

**How to Fix:**
- Define acceptance criteria BEFORE development begins
- Include criteria in Definition of Ready for user stories
- Review criteria in backlog grooming and sprint planning
- Make criteria visible in ticketing system (Jira, Azure DevOps)

---

### Mistake 3: Ignoring Negative and Edge Cases

**Problem:**
- Criteria only cover the happy path
- "User can submit form" but no criteria for:
  - What if required fields are empty?
  - What if user is not authenticated?
  - What if system is down?

**Why It's a Problem:**
- Production defects in edge cases
- Poor user experience in error scenarios
- Security vulnerabilities

**How to Fix:**
- Ask "What could go wrong?" for every criterion
- Add boundary criteria: "System prevents X", "Error message displays when Y"
- Use negative testing scenarios: "User cannot...", "System rejects..."

---

### Mistake 4: Criteria Not Aligned with Business Goals

**Problem:**
- Evaluation criteria focus on features/technology but miss strategic fit
- Acceptance criteria test technical function but ignore business value

**Example:**
- Selecting a CRM based solely on features, ignoring that vendor specializes in B2C when you're B2B
- Building a report that meets technical specs but doesn't answer the business question

**How to Fix:**
- Always tie criteria back to business objectives
- For evaluation: Include strategic fit as explicit criterion
- For acceptance: Define success criteria that prove business value, not just technical function
- Ask: "If all these criteria pass, will the business goal be achieved?"

---

### Mistake 5: Too Many or Too Few Criteria

**Problem:**
- **Too many:** 50 acceptance criteria for a simple feature → paralysis, confusion
- **Too few:** 2 vague criteria for a complex requirement → gaps, ambiguity

**Why It's a Problem:**
- Too many: Diminishing returns, hard to prioritize, slows delivery
- Too few: Incomplete, leaves room for misinterpretation

**How to Fix:**
- Use the "Goldilocks Principle": Just enough to be clear and testable
- Rule of thumb: 
  - Simple story: 3-7 criteria
  - Complex story: 8-15 criteria
  - If more than 15, consider splitting the story
- For evaluation: Focus on differentiating criteria (eliminate criteria where all options score the same)

---

### Mistake 6: Untestable Criteria

**Problem:**
- "System should be secure"
- "Code should be maintainable"
- "Solution should be future-proof"

**Why It's a Problem:**
- QA cannot create objective tests
- Acceptance becomes opinion-based
- Disagreement at sign-off

**How to Fix:**
- For every criterion, ask: "How would QA test this?"
- If the answer is vague, make the criterion more specific
- ❌ "Secure" → ✅ "Passes OWASP Top 10 vulnerability scan with zero high/critical findings"
- ❌ "Maintainable" → ✅ "Code coverage >80%, cyclomatic complexity <10, passes SonarQube quality gate"

---

### Mistake 7: Criteria Changed Mid-Stream Without Impact Analysis

**Problem:**
- Criteria changed during development or testing without considering impact
- "Actually, we need it to support 1000 concurrent users, not 500"

**Why It's a Problem:**
- May require architectural changes
- Testing already completed may be invalid
- Schedule and budget impacts not assessed

**How to Fix:**
- Treat criteria changes as scope changes requiring formal change control
- Assess impact on design, development, testing, schedule, budget
- Get stakeholder agreement on trade-offs before accepting change
- Version criteria and track changes

---

### Mistake 8: Evaluation Criteria Weights Not Validated

**Problem:**
- One person assigns weights without stakeholder input
- Weights don't reflect true priorities
- Result: "Optimal" solution chosen but stakeholders unhappy

**Why It's a Problem:**
- Decision not aligned with real priorities
- Lack of buy-in from stakeholders
- Can't defend decision when questioned

**How to Fix:**
- Facilitate weight assignment workshop with key stakeholders
- Use techniques like pairwise comparison or dot voting
- Test weights: "If Option A is much cheaper but weaker on features, which wins?" to see if weights reflect reality
- Document who agreed to weights and why

---

## Best Practices

### 1. Use the SMART Framework for Individual Criteria
- **Specific:** Clearly defined, no ambiguity
- **Measurable:** Can be objectively verified
- **Achievable:** Realistic given constraints
- **Relevant:** Tied to business goals
- **Time-bound:** (Where applicable) Includes timing expectations

### 2. Involve the Right Stakeholders
- **For Acceptance Criteria:** Product owner, end users, QA, developers, architects
- **For Evaluation Criteria:** Decision-makers, business stakeholders, technical experts, financial analysts
- Facilitate workshops rather than creating criteria in isolation

### 3. Use Examples and Counter-Examples
- Supplement criteria with concrete examples
- "For instance, when user enters invalid email format, system displays: 'Please enter valid email address (example@domain.com)'"
- Show what IS and IS NOT acceptable

### 4. Link Criteria to Tests
- Each acceptance criterion should map to one or more test cases
- Use traceability matrix: Requirement → Criteria → Tests
- Ensures test coverage and validates testability of criteria

### 5. Version and Baseline Criteria
- Establish a baseline set of criteria before work begins
- Version criteria as they evolve
- Use change control for modifications during delivery
- Maintain history for audit and lessons learned

### 6. Prioritize Criteria (Must-Have vs. Nice-to-Have)
- Not all criteria are equally critical
- Use MoSCoW: Must have, Should have, Could have, Won't have
- For evaluation, use weights to reflect priority
- Helps with trade-off decisions during delivery

### 7. Make Criteria Visible
- Don't hide criteria in documents
- Display them prominently:
  - In user story tickets (Jira, Azure DevOps)
  - On team boards during standups
  - In sprint review demos
  - In test management tools

### 8. Review and Retrospect on Criteria Quality
- After delivery, assess: Were the criteria clear? Complete? Testable?
- Learn from disputes or rework caused by unclear criteria
- Improve your criteria-writing skills over time

---

## Tools and Techniques to Support This Technique

### Documentation Tools
- **Jira/Azure DevOps:** Store acceptance criteria directly in user stories
- **Confluence/SharePoint:** Document evaluation criteria matrices and decision records
- **Requirements management tools (Jama, Helix RM):** Formal traceability from requirements to criteria to tests

### Modeling and Analysis Tools
- **Decision matrices/scorecards:** Excel, Google Sheets, or specialized tools (DecisionLens, Pugh Matrix)
- **AHP (Analytic Hierarchy Process) tools:** For complex multi-criteria decisions
- **Weighted scoring models:** Built in Excel or PowerBI

### Testing Tools
- **Test management (TestRail, Zephyr, qTest):** Link test cases to acceptance criteria
- **BDD frameworks (Cucumber, SpecFlow):** Write criteria in Given-When-Then format that becomes executable tests
- **Load testing (JMeter, LoadRunner):** Verify performance criteria
- **Security testing (OWASP ZAP, Burp Suite):** Verify security criteria

### Collaboration Tools
- **Miro/Mural:** Facilitate virtual workshops to define and validate criteria
- **Voting tools (Mentimeter, Slido):** Gather stakeholder input on weights and priorities
- **Version control (Git, GitHub, GitLab):** Track changes to criteria documents over time

---

## Related BABOK Techniques

### Complementary Techniques Often Used Together

**Acceptance and Evaluation Criteria** works well with:

1. **User Stories**
   - Criteria define the "done" conditions for user stories
   - Format: As a [role], I want [feature], so that [benefit] + acceptance criteria

2. **Use Cases and Scenarios**
   - Criteria specify success and failure conditions for use case flows
   - Scenarios illustrate how criteria are met in context

3. **Data Modeling**
   - Criteria may reference data quality, validation rules, or data volume expectations
   - Data model defines the "what", criteria define acceptable data characteristics

4. **Process Modeling**
   - Criteria specify acceptable process performance (cycle time, error rates, throughput)
   - Process models show the flow, criteria measure the outcomes

5. **Non-Functional Requirements Analysis**
   - NFRs are abstract; criteria make them concrete and testable
   - Example: NFR = "system must be scalable" → Criteria = "supports 10,000 concurrent users with <3s response time"

6. **Prototyping**
   - Prototype used to validate whether acceptance criteria are realistic and complete
   - Stakeholder feedback on prototype helps refine criteria

7. **Decision Analysis**
   - Evaluation criteria are the core of formal decision analysis techniques
   - Methods like weighted scoring, decision trees, and sensitivity analysis all rely on well-defined criteria

8. **Metrics and KPIs**
   - Acceptance criteria for a solution become KPIs for measuring post-implementation success
   - Example: "95th percentile response time <2s" becomes operational KPI

9. **Test Plans and Test Cases**
   - Direct translation: Each acceptance criterion → one or more test cases
   - Test coverage analysis ensures all criteria are tested

10. **Definition of Done (Agile)**
    - DoD is a checklist of acceptance criteria that apply to all stories in a sprint/release
    - Combines story-specific criteria with team-wide quality standards

---

## Adapting This Technique Across Methodologies

### Agile/Scrum Context
- **When:** Defined during backlog refinement, before sprint planning
- **Format:** Written directly in user story (often in "Given-When-Then" BDD format)
- **Validation:** Demonstrated in sprint review, accepted by product owner
- **Evolution:** Refined iteratively as understanding increases; earlier stories may have simpler criteria

**Example Agile Format:**
```
User Story: Customer can view order history

Acceptance Criteria:
Given I am a logged-in customer
When I navigate to "My Orders" 
Then I see a list of all my orders from the past 2 years
And each order shows: order number, date, status, total amount
And orders are sorted by date (most recent first)
And I can click an order to view full details
```

### Waterfall/Traditional Context
- **When:** Defined during requirements phase, formalized in requirements documents
- **Format:** Section in BRD/FRD or separate acceptance test plan document
- **Validation:** Formal UAT at end of project, sign-off against criteria
- **Evolution:** Changes require formal change control process

### Lean/Kanban Context
- **When:** Defined as WIP (Work in Progress) items move into "Ready" state
- **Format:** Lightweight, just enough criteria to clarify "done"
- **Validation:** Continuous review as work completes
- **Evolution:** Refined based on feedback, less formal process

### SAFe (Scaled Agile) Context
- **When:** 
  - Features: Acceptance criteria defined at PI Planning
  - Stories: Refined by teams during iteration planning
- **Format:** Criteria at multiple levels (Epic → Feature → Story)
- **Validation:** Demo at iteration review (stories), System demo (features)
- **Evolution:** Refined throughout PI, with dependencies managed across teams

---

## Measuring Success of This Technique

How do you know if your use of Acceptance and Evaluation Criteria is effective?

### Metrics to Track

1. **Defect Leakage Rate**
   - % of defects found in production vs. total defects
   - Good criteria → More defects caught in testing → Lower leakage
   - Target: 80%+ of defects caught before production

2. **UAT Pass Rate (First Time)**
   - % of requirements accepted on first UAT attempt
   - Clear criteria → Higher first-time pass rate
   - Target: 90%+ first-time acceptance

3. **Requirements Rework %**
   - % of requirements changed after development begins
   - Good criteria → Fewer changes due to misunderstanding
   - Target: <10% rework due to unclear requirements

4. **Test Case Coverage**
   - % of acceptance criteria with corresponding test cases
   - Should be 100% for critical criteria
   - Measures testability of criteria

5. **Stakeholder Satisfaction with Decision Process**
   - Survey: "Did evaluation criteria help us make the right choice?"
   - For solution evaluation decisions
   - Target: 80%+ agree criteria were valuable

6. **Sprint Review Acceptance Cycle Time**
   - Time from demo to final acceptance
   - Clear criteria → Faster acceptance, less back-and-forth
   - Target: Acceptance within 2 business days

### Qualitative Indicators

- **Fewer disagreements** during UAT about whether requirements are met
- **Faster sprint reviews** because "done" is already understood
- **Better developer confidence** because they know the target
- **Improved team morale** due to less rework and clearer expectations
- **Easier onboarding** because new team members can read criteria and understand expectations

---

## Real-World Case Examples

### Case Study 1: Financial Services - Payment Processing System

**Context:** Bank implementing new payment processing system to replace legacy mainframe.

**Challenge:** 
- Previous project failed acceptance testing three times
- Stakeholders and IT had different definitions of "correct processing"
- Six months behind schedule due to rework

**Application of Technique:**
- Conducted 3-day workshop with business SMEs, compliance, operations, and IT
- Defined 147 detailed acceptance criteria across 18 functional areas
- Each criterion included: condition, expected result, test data requirements, compliance reference

**Example Criteria:**
- "When customer initiates ACH transfer >$10,000, system requires dual authorization within 24 hours and logs both approvers in audit trail per SOX requirements"
- "System processes 10,000 transactions per hour during month-end with 99.9% success rate, with failed transactions automatically queued for manual review"

**Outcome:**
- UAT passed on first attempt with 98% criteria met (3 criteria deferred to Phase 2 by mutual agreement)
- Go-live on time with zero production defects in first 30 days
- Audit praised clear traceability from regulations → criteria → tests

**Lesson:** Time invested in detailed criteria workshop (3 days) saved 4-6 months of rework.

---

### Case Study 2: Retail - E-commerce Platform Selection

**Context:** Mid-size retailer selecting e-commerce platform (build custom vs. 3 COTS options).

**Challenge:**
- Initial selection based on "gut feel" and vendor presentations
- Selection committee deadlocked between two options
- CEO frustrated by lack of objective justification

**Application of Technique:**
- BA facilitated evaluation criteria workshop with diverse stakeholders
- Defined 25 weighted criteria across 6 categories
- Conducted formal scoring over 2-week evaluation period with vendor demos and reference checks

**Key Criteria:**
| Criterion | Weight | Why It Mattered |
|-----------|--------|-----------------|
| Total Cost of Ownership (5yr) | 20% | Budget constraint: <$2M |
| Mobile commerce capability | 18% | 60% of traffic mobile, strategic priority |
| Integration with existing ERP | 15% | Make-or-break technical requirement |
| Customization flexibility | 12% | Unique business model requirements |
| Time to market | 10% | Seasonal business, must launch in 6 months |

**Outcome:**
- COTS Vendor B selected with clear numerical justification (score: 4.2/5 vs. 3.8 and 3.6)
- CEO approved immediately based on transparent, defensible analysis
- Vendor B wasn't the cheapest but scored highest on strategic priorities (mobile, time-to-market)
- Post-implementation (18 months): Decision validated, system met all critical criteria

**Lesson:** Weighted criteria transformed subjective debate into objective decision, enabling faster approval.

---

### Case Study 3: Healthcare - Patient Portal (Agile)

**Context:** Hospital system building patient portal for appointment scheduling, test results, messaging.

**Challenge:**
- Agile team writing vague acceptance criteria: "User can view test results"
- Frequent disagreements in sprint reviews about whether stories were "done"
- Product owner rejecting 40% of stories, causing frustration

**Application of Technique:**
- BA trained team on writing testable acceptance criteria using Given-When-Then format
- Established Definition of Ready: Story cannot enter sprint unless criteria are clear, testable, and agreed
- Introduced acceptance criteria review as part of backlog refinement

**Example Improvement:**

**Before (vague):**
- "User can view test results"

**After (specific):**
- Given I am a patient logged into the portal
- When I navigate to "Test Results"
- Then I see all test results from the past 12 months
- And each result shows: test name, date, ordering physician, status (final/preliminary)
- And I can filter by date range and test type
- And I can download results as PDF
- And results marked "abnormal" display with visual indicator
- And I cannot view results marked "hold for provider review"
- And results load within 3 seconds
- And system complies with HIPAA audit logging requirements

**Outcome:**
- Sprint review acceptance rate improved from 60% to 95%
- Velocity stabilized (less rework = more predictable delivery)
- QA test coverage improved: Test cases written directly from acceptance criteria
- Product owner and team satisfaction improved significantly

**Lesson:** Investing 15-20 minutes per story in clear criteria saved hours of rework and conflict.

---

## FAQs

**Q: How detailed should acceptance criteria be?**  
**A:** Detailed enough to be testable and unambiguous, but not so detailed that you're writing the design. Focus on "what" and "what quality", not "how". If QA can write a test case from the criterion without asking questions, it's detailed enough.

**Q: Who is responsible for writing acceptance criteria?**  
**A:** Typically the Business Analyst or Product Owner, but it should be a collaborative effort. The best criteria come from workshops with stakeholders, subject matter experts, developers, and QA. The BA facilitates and documents, but doesn't write in isolation.

**Q: Can acceptance criteria change during development?**  
**A:** Changes should be minimized but are sometimes necessary. Treat criteria changes as scope changes:
- Assess impact on design, development, testing, schedule
- Get stakeholder agreement on trade-offs
- Update requirements documentation and tests
- In Agile: Prefer to create a new story for changed requirements rather than changing in-progress story

**Q: What's the difference between acceptance criteria and test cases?**  
**A:** 
- **Acceptance Criteria:** Define what must be true for the requirement to be acceptable (the "what")
- **Test Cases:** Define how you will verify the criteria are met (the "how")
- One acceptance criterion may generate multiple test cases (positive test, negative test, boundary test, etc.)

**Q: How many acceptance criteria should a user story have?**  
**A:** There's no fixed number, but guidelines:
- Too few (<3): Probably too vague or story is too small
- Sweet spot (3-7): Most single-function stories
- Many (8-15): Complex story, but manageable
- Too many (>15): Consider splitting the story

**Q: Should acceptance criteria cover non-functional requirements?**  
**A:** Yes! Criteria should cover both functional behavior AND quality attributes. Examples:
- Performance: "Page loads within 2 seconds"
- Security: "Requires multi-factor authentication"
- Usability: "Completes task without training"
- Compliance: "Meets GDPR data retention rules"

**Q: What if stakeholders can't agree on evaluation criteria weights?**  
**A:** 
- Use facilitation techniques like:
  - Pairwise comparison (compare criteria two at a time)
  - Dot voting (each stakeholder allocates points)
  - Delphi method (anonymous rounds until consensus)
- Escalate to decision authority if consensus isn't possible
- Document dissenting opinions and rationale
- Consider sensitivity analysis: "If we weight X higher, does the decision change?"

**Q: How do I handle criteria that conflict with each other?**  
**A:** 
- Example: "Must be feature-rich" vs. "Must be simple and easy to use"
- Make trade-offs explicit: "Prioritize ease-of-use over feature breadth for version 1"
- Use MoSCoW: Advanced features are "Could have", not "Must have"
- Consider phased delivery: Simple in v1, more features in v2
- Document the deliberate trade-off decision

**Q: What's the difference between Done criteria, Acceptance Criteria, and Definition of Done?**  
**A:**
- **Acceptance Criteria:** Specific to a single requirement/story (varies per story)
- **Definition of Done:** Checklist that applies to ALL stories (consistent across team)
  - Example DoD: "Code reviewed, unit tests pass, deployed to test environment, documentation updated"
- **Done Criteria:** General term that could mean either of the above depending on context

**Q: Should evaluation criteria always be weighted?**  
**A:** Not always, but usually helpful:
- **Use weights** when: Criteria have different importance, need objective scoring, formal decision required
- **Skip weights** when: All criteria are equal priority, simple pass/fail evaluation, informal decision
- When in doubt, use weights—it forces explicit priority discussions

---

## Key Takeaways

1. **Transform Subjectivity into Objectivity:** Acceptance and evaluation criteria convert stakeholder expectations and opinions into measurable, testable conditions that everyone can agree on.

2. **Define "Done" Before You Start:** The most expensive rework comes from discovering late that stakeholders meant something different. Define clear criteria before development begins.

3. **Make Criteria Testable:** Every criterion should answer: "How will we verify this objectively?" If QA can't test it, refine it.

4. **Cover the Whole Picture:** Include functional, quality, boundary, and exception conditions. Don't just test the happy path.

5. **Use Criteria to Enable Better Decisions:** Evaluation criteria make solution selection transparent, defensible, and aligned with business priorities.

6. **Collaborate on Criteria:** The best criteria come from workshops with diverse perspectives—not from BAs writing alone in a room.

7. **Iterate and Improve:** Your first criteria won't be perfect. Learn from disputes, rework, and defects to write better criteria next time.

8. **Link Criteria to the Bigger Picture:** Always tie criteria back to business objectives. If all criteria pass but business value isn't achieved, the criteria were wrong.

---

## Additional Resources

### BABOK References
- **BABOK v3:**
  - 10.2 Acceptance and Evaluation Criteria (primary)
  - 10.1 Acceptance Testing
  - 9.23 Non-Functional Requirements Analysis
  - 9.9 Decision Analysis
  - 10.41 User Stories

### Recommended Reading
- **"User Stories Applied" by Mike Cohn:** Chapter on acceptance criteria for agile teams
- **"Writing Effective Use Cases" by Alistair Cockburn:** Success and failure guarantees (similar to acceptance criteria)
- **"The Art of Agile Development" by James Shore:** Section on "Done Done" and acceptance
- **"Software Requirements" by Karl Wiegers:** Chapters on acceptance testing and non-functional requirements

### Standards and Frameworks
- **ISO/IEC/IEEE 29148:** Requirements engineering standard (includes acceptance criteria)
- **ISTQB:** Test design techniques based on acceptance criteria
- **Agile Alliance:** Resources on Definition of Done and acceptance criteria

### Online Resources
- **IIBA:** Case studies and webinars on effective requirements practices
- **Atlassian Agile Coach:** Guides on writing acceptance criteria in Jira
- **Ministry of Testing:** Community discussions on acceptance testing

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [Date] | [Your Name] | Initial comprehensive documentation |

---

## How to Use This Document

**For BAs Learning the Technique:**
1. Read "Overview" and "Why This Matters" first
2. Study the step-by-step "How to Apply" section
3. Review the practical examples
4. Try the templates on a real project
5. Learn from "Common Mistakes" section

**For Teams Applying the Technique:**
1. Use the templates as starting points
2. Adapt the step-by-step process to your methodology (Agile/Waterfall/etc.)
3. Refer to examples when writing your own criteria
4. Use the checklists in workshops

**For Stakeholders and Product Owners:**
1. Understand "Why This Matters" to appreciate the value
2. Review examples to see what good criteria look like
3. Use the validation questions to review criteria with your team

**For QA/Testers:**
1. Use acceptance criteria to create test cases
2. Reference "Common Mistakes" to help improve criteria quality
3. Provide feedback to BAs on testability of criteria

**For Trainers and Coaches:**
1. Use the "Step-by-Step" section as training curriculum
2. Leverage examples and case studies in workshops
3. Use "Common Mistakes" as cautionary tales
4. Assign templates as practice exercises

---

## Feedback and Contributions

This is a living document. If you have:
- Additional examples or case studies
- Corrections or clarifications
- Tool recommendations
- Questions to add to FAQ

Please [contribute to the repository / contact the documentation owner].

---

**End of Document**
