# Data Dictionary (BABOK® Technique)

## 1. What This Technique Is

A Data Dictionary is a **centralized repository of data definitions** that describes the meaning, format, and usage of data elements used by the business and its systems.  
It provides a **single source of truth** for how data is understood across stakeholders.

Unlike concept models (which define business concepts), a data dictionary focuses on **data elements and their attributes**.

---

## 2. Why This Technique Exists

Data-related issues commonly occur because:
- The same data element is defined differently across teams
- Field meanings are assumed rather than documented
- Reports and systems use inconsistent definitions

The Data Dictionary exists to help a BA:
- Ensure consistent understanding of data
- Reduce misinterpretation in requirements and reporting
- Support integration across systems
- Improve data quality and governance

BABOK includes this technique because **clear data definitions are critical to reliable solutions**.

---

## 3. When to Use a Data Dictionary

A Data Dictionary is most effective when:
- Working on data-heavy initiatives
- Building or modifying reports and dashboards
- Integrating multiple systems
- Supporting regulatory or compliance reporting
- Defining data requirements

Common BA scenarios:
- Banking and financial services
- Business intelligence and analytics
- Data migration projects
- Enterprise platforms

---

## 4. When NOT to Use a Data Dictionary

This technique may add limited value when:
- The solution involves minimal data
- Data definitions are already standardized and governed
- The initiative is very small in scope

In such cases, **inline data definitions** may be sufficient.

---

## 5. Typical Components of a Data Dictionary

A data dictionary commonly includes:
- Data element name
- Business definition
- Data type and format
- Allowed values or domains
- Source system
- Usage context
- Ownership and stewardship

---

## 6. How to Apply a Data Dictionary – Step by Step

### Step 1: Identify Key Data Elements
Extract data elements from:
- Requirements
- Reports
- Interfaces
- Existing systems

### Step 2: Define Each Data Element
Document:
- Clear business definition
- Avoid technical jargon where possible

### Step 3: Capture Attributes
Include:
- Data type
- Length or format
- Valid values
- Defaults

### Step 4: Identify Source and Usage
Record:
- Source systems
- Downstream usage
- Reporting dependencies

### Step 5: Review and Validate
Confirm definitions with:
- Business stakeholders
- Data owners
- Technical teams

### Step 6: Maintain and Govern
Ensure:
- Version control
- Change management
- Ongoing ownership

---

## 7. Inputs

Typical inputs include:
- Concept models
- Requirements documents
- Existing data models
- Reports and dashboards
- Stakeholder interviews

---

## 8. Outputs

Typical outputs include:
- Approved data dictionary
- Standardized data definitions
- Inputs to data models and requirements
- Reduced data ambiguity

---

## 9. Common Mistakes by Business Analysts

- Mixing business definitions with technical implementation details
- Failing to assign ownership
- Allowing duplicate or conflicting definitions
- Treating the data dictionary as static
- Not validating definitions with stakeholders

---

## 10. Real-World Example (Banking / IT)

**Scenario:** Regulatory liquidity reporting

Different teams define “Available Balance” differently:
- Operations: cleared funds
- Treasury: projected funds
- IT: system-calculated value

A data dictionary:
- Standardizes definitions
- Aligns reporting logic
- Reduces regulatory reporting risk

---

## 11. Mapping to BABOK Knowledge Areas

The Data Dictionary supports:
- Elicitation and Collaboration
- Requirements Analysis and Design Definition
- Solution Evaluation

---

## 12. Interview Tips (For Job Interviews)

Example response:

> “I use a data dictionary to ensure consistent understanding of data across stakeholders, especially in reporting, integration, and regulatory initiatives.”

---

## 13. Related Techniques

Often combined with:
- Concept Modelling
- Data Modelling
- Glossary
- Document Analysis
- Business Rules Analysis

---

## 14. Key Takeaways

- A data dictionary provides a single source of truth for data definitions
- Essential for data quality and integration
- Must be governed and maintained
- Reduces reporting and compliance risks
