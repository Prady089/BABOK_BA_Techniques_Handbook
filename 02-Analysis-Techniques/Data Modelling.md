# Data Modelling (BABOK® Technique)

## 1. What This Technique Is

Data Modelling is a technique used by Business Analysts to **define, organize, and structure data** required by the business and its systems.  
It represents **data entities, their attributes, and relationships**, independent of technical implementation.

Data models help ensure that data requirements are **complete, consistent, and shared** across business and IT stakeholders.

---

## 2. Why This Technique Exists

Data-related problems often occur because:
- Data requirements are implicit or unclear
- Different systems interpret data differently
- Relationships between data elements are misunderstood
- Data definitions are inconsistent

Data Modelling exists to help a BA:
- Clarify data requirements early
- Reduce integration and reporting issues
- Support system design and automation
- Enable consistent data usage across the organization

BABOK includes Data Modelling because **data is foundational to most business solutions**.

---

## 3. When to Use Data Modelling

Data Modelling is most effective when:
- Building or modifying data-intensive systems
- Integrating multiple systems
- Designing reports, analytics, or dashboards
- Migrating or consolidating data
- Supporting regulatory or compliance reporting

Common BA scenarios:
- Core banking platforms
- Data warehouses and lakes
- Customer master data initiatives
- Regulatory reporting systems

---

## 4. When NOT to Use Data Modelling

Data Modelling may add limited value when:
- The solution is simple with minimal data
- Data structures are already standardized and stable
- The initiative does not involve data changes

In such cases, **lightweight data definitions** may be sufficient.

---

## 5. Types of Data Models

### Conceptual Data Model
High-level view of key business entities and relationships, without attributes.

### Logical Data Model
Defines entities, attributes, relationships, and business rules, independent of technology.

### Physical Data Model
Represents how data is stored in a specific system or database (usually owned by technical teams).

---

## 6. How to Apply Data Modelling – Step by Step

### Step 1: Identify Business Entities
Extract entities from:
- Business processes
- Requirements
- Concept models
- Stakeholder discussions

### Step 2: Define Attributes
For each entity, identify:
- Key data elements
- Business definitions
- Optional vs mandatory fields

### Step 3: Identify Relationships
Determine:
- How entities relate
- Cardinality (one-to-one, one-to-many)
- Optionality

### Step 4: Apply Business Rules
Incorporate:
- Validation rules
- Constraints
- Derivations

### Step 5: Create the Data Model
Develop:
- Conceptual or logical data models
- Clear, business-friendly diagrams

### Step 6: Validate with Stakeholders
Review with:
- Business users
- Data owners
- Technical teams

---

## 7. Inputs

Typical inputs include:
- Concept models
- Data dictionary
- Business rules
- Requirements documentation
- Stakeholder interviews

---

## 8. Outputs

Typical outputs include:
- Conceptual and logical data models
- Clarified data requirements
- Inputs to physical data design
- Improved data consistency

---

## 9. Common Mistakes by Business Analysts

- Jumping directly to physical data design
- Using technical jargon in business models
- Ignoring data quality and governance
- Missing relationships or constraints
- Skipping stakeholder validation

---

## 10. Real-World Example (Banking / IT)

**Scenario:** Customer data consolidation

Multiple systems maintain customer information differently.

Data modelling:
- Defines a single customer entity
- Clarifies relationships with accounts and products
- Supports master data management
- Reduces duplication and reporting inconsistencies

---

## 11. Mapping to BABOK Knowledge Areas

Data Modelling supports:
- Requirements Analysis and Design Definition
- Strategy Analysis
- Solution Evaluation

---

## 12. Interview Tips (For Job Interviews)

Example response:

> “I use data modelling to clarify and validate data requirements early, ensuring consistent understanding across business and IT before system design.”

---

## 13. Related Techniques

Often combined with:
- Concept Modelling
- Data Dictionary
- Data Flow Diagrams
- Interface Analysis
- Business Rules Analysis

---

## 14. Key Takeaways

- Data modelling structures business data clearly
- Conceptual and logical models belong to BA work
- Reduces integration and reporting issues
- Foundation for reliable system design
