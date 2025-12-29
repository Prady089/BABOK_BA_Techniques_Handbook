# Interviews (BABOK® Technique)

## 1. What This Technique Is

Interviews are **structured or semi-structured conversations** conducted by a Business Analyst to elicit detailed information from stakeholders.  
They are one of the most fundamental and widely used techniques in business analysis because they allow **direct, focused, and contextual understanding** of stakeholder needs, concerns, and expectations.

Unlike workshops or surveys, interviews provide **depth over breadth** and are especially effective when individual perspectives matter.

---

## 2. Why This Technique Exists

Business problems are rarely fully understood through documents alone.  
Interviews exist to help a BA:

- Uncover **real needs behind stated requests**
- Explore **assumptions, constraints, and motivations**
- Understand **individual stakeholder perspectives**
- Build **trust and credibility** early in an initiative

BABOK emphasizes interviews because **stakeholders often describe solutions**, not problems. Interviews help the BA uncover the **true underlying need**.

---

## 3. When to Use Interviews

Interviews are most effective when:

- Requirements are **unclear or ambiguous**
- Stakeholders have **unique or specialized knowledge**
- Topics are **sensitive or political**
- You need **deep understanding**, not consensus
- Stakeholders are **not comfortable speaking in groups**
- The initiative is in an **early discovery phase**

They are commonly used during:
- Strategy Analysis
- Elicitation & Collaboration
- Requirements Analysis
- Solution Evaluation (feedback interviews)

---

## 4. When NOT to Use Interviews

Interviews may NOT be the best choice when:

- You need **alignment across many stakeholders** (workshops are better)
- Time is extremely limited and broad input is needed (surveys)
- Stakeholders already agree and information is well-documented
- The goal is **decision-making**, not discovery

Relying only on interviews in large initiatives can lead to **fragmented understanding** if results are not consolidated properly.

---

## 5. Types of Interviews – Structure Overview



```mermaid
flowchart TD
    A[Interview Technique] --> B{Level of Structure Needed?}

    B -->|High| C[Structured Interview]
    B -->|Medium| D[Semi-Structured Interview]
    B -->|Low| E[Unstructured Interview]

    C --> C1[Predefined Questions]
    C --> C2[Same Questions for All Stakeholders]
    C --> C3[Minimal Follow-ups]
    C --> C4[Focus: Consistency & Validation]

    D --> D1[Prepared Question Guide]
    D --> D2[Flexible Follow-up Questions]
    D --> D3[Adaptive Based on Responses]
    D --> D4[Focus: Balance of Depth & Control]

    E --> E1[Open Conversation]
    E --> E2[Exploratory Questions]
    E --> E3[Free Flow Discussion]
    E --> E4[Focus: Discovery & Insight]




## Types of Interviews

Business Analysts use different types of interviews depending on the **level of structure, clarity of the problem space, and need for flexibility**. The three commonly used interview types are **Structured**, **Semi-Structured**, and **Unstructured** interviews.

---

## Structured Interviews

Structured interviews are used when **consistency and comparability** of information are critical.  
In this approach, the Business Analyst asks the **same predefined questions** to all stakeholders, following a fixed sequence and format.

This makes it easier to:
- Validate responses
- Compare inputs across stakeholders
- Identify gaps or inconsistencies

Structured interviews are most effective when the BA already has a **clear understanding of the problem space** and needs **confirmation rather than exploration**.

### Key Characteristics
- Predefined and fixed set of questions  
- Consistent format across all stakeholders  
- Minimal deviation or follow-up questions  
- Strong focus on validation and confirmation  

### Typical Use Cases
- Validation of requirements  
- Compliance and regulatory initiatives  
- Confirmation of known or well-defined requirements  

---

## Semi-Structured Interviews (Most Common for BAs)

Semi-structured interviews are used when both **structure and flexibility** are required.  
The Business Analyst prepares a set of key questions or themes but adapts follow-up questions based on stakeholder responses.

This approach allows the BA to:
- Maintain focus on objectives
- Explore new insights as they emerge
- Balance control with discovery

Because of this balance, semi-structured interviews are the **most commonly used interview type** in real-world business analysis.

### Key Characteristics
- Prepared question guide or agenda  
- Flexible follow-up questions  
- Adaptive flow based on responses  
- Balance between consistency and exploration  

### Typical Use Cases
- Requirements elicitation  
- Stakeholder analysis  
- Early to mid-stage discovery activities  

---

## Unstructured Interviews

Unstructured interviews are used primarily for **exploration and learning**, especially when the problem space or domain is unclear or unfamiliar.  
The Business Analyst guides the conversation lightly, allowing stakeholders to speak freely and surface insights organically.

This approach prioritizes **discovery over control** and is most effective during the **early stages** of an initiative.

Because there is minimal structure, this interview type requires strong listening and facilitation skills to avoid missing critical topics.

### Key Characteristics
- Open-ended, free-flow conversations  
- Minimal predefined questions  
- High flexibility and adaptability  
- Greater risk of missing key topics if poorly facilitated  

### Typical Use Cases
- Early discovery  
- Innovation and ideation  
- Understanding unfamiliar or complex domains  

---
## Comparison of Interview Types

| Aspect | Structured Interviews | Semi-Structured Interviews | Unstructured Interviews |
|------|----------------------|---------------------------|-------------------------|
| Level of Structure | High | Medium | Low |
| Question Format | Fully predefined | Prepared guide with flexibility | Open-ended conversation |
| Flexibility | Very limited | Moderate | High |
| Consistency Across Stakeholders | High | Medium | Low |
| Depth of Exploration | Low | Medium to High | High |
| Comparability of Responses | High | Medium | Low |
| Control by BA | High | Balanced | Low |
| Risk of Missing Key Topics | Low | Low to Medium | High |
| Stakeholder Comfort | Medium | High | High |
| BA Skill Required | Low to Medium | Medium | High |
| Best Used When | Validation and compliance are critical | Balance of discovery and control is needed | Problem space is unclear or exploratory |
| Typical BA Usage | Formal validation | Most common real-world usage | Early discovery and innovation |

flowchart TD
    A[Need to Elicit Information from Stakeholders] --> B{Is the problem space clearly understood?}

    B -->|Yes| C{Is consistency and comparability critical?}
    B -->|No| D{Is the goal exploration and learning?}

    C -->|Yes| E[Choose Structured Interviews]
    C -->|No| F[Choose Semi-Structured Interviews]

    D -->|Yes| G[Choose Unstructured Interviews]
    D -->|No| F[Choose Semi-Structured Interviews]


## 6. How to Apply Interviews – Step by Step

### Step 1: Define the Purpose
Clearly identify:
- What you want to learn
- How the information will be used
- Which BABOK task this supports

### Step 2: Identify the Right Stakeholders
Choose stakeholders based on:
- Role
- Influence
- Knowledge
- Impact of the change

### Step 3: Prepare Questions
- Start with **open-ended questions**
- Avoid leading questions
- Group questions by theme
- Prepare follow-ups

Example:
> “Can you walk me through how you currently perform this task?”

### Step 4: Conduct the Interview
- Set expectations
- Actively listen
- Observe tone and hesitation
- Ask “why” and “can you elaborate?”

### Step 5: Capture Information
- Take structured notes
- Capture assumptions and concerns
- Avoid interpreting during the interview

### Step 6: Analyze and Consolidate
- Identify patterns
- Resolve contradictions
- Separate needs from solutions

### Step 7: Confirm Understanding
- Share summaries
- Ask for validation
- Correct misunderstandings early

---

## 7. Inputs

Typical inputs include:
- Business objectives
- Stakeholder list
- Existing documentation
- Problem statements
- Assumptions and risks

---

## 8. Outputs

Typical outputs include:
- Elicitation notes
- Identified requirements
- Stakeholder concerns
- Assumptions and constraints
- Follow-up questions
- Input to models or user stories

---

## 9. Common Mistakes by Business Analysts

- Asking **leading or biased questions**
- Turning interviews into solution discussions
- Not preparing adequately
- Talking more than listening
- Failing to validate understanding
- Treating one stakeholder’s view as the truth
- Skipping documentation or consolidation

---

## 10. Real-World Example (Banking / IT)

**Scenario:** Regulatory reporting enhancement

- Interviews with compliance reveal interpretation gaps
- Operations interviews expose manual workarounds
- IT interviews identify system constraints

Without interviews:
- Solution addresses symptoms only

With interviews:
- Root causes identified
- Reporting logic clarified
- Regulatory risk reduced

---

## 11. Mapping to BABOK Knowledge Areas

Interviews support multiple knowledge areas:

- Business Analysis Planning & Monitoring
- Elicitation & Collaboration
- Strategy Analysis
- Requirements Analysis & Design Definition
- Solution Evaluation

This makes interviews one of the **most reusable techniques** in BABOK.

---

## 12. Interview Tips (For Job Interviews)

How to explain interviews in interviews:

- Emphasize **preparation and purpose**
- Mention **open-ended questioning**
- Highlight **validation and consolidation**
- Explain how you **handle conflicting inputs**

Example answer:
> “I use semi-structured interviews to uncover underlying needs, validate assumptions, and build stakeholder trust, especially in early discovery and complex domains.”

---

## 13. Variations & Related Techniques

Often used together with:
- Workshops
- Observation
- Document Analysis
- Process Modelling
- Root Cause Analysis

Interviews provide **depth**, while these techniques add **breadth and structure**.

---

## 14. Key Takeaways

- Interviews are about **discovery, not confirmation**
- Preparation determines success
- Listening matters more than questioning
- Validation prevents rework
- Interviews are foundational to BA effectiveness
