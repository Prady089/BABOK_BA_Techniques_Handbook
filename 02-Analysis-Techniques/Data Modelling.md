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

## 5. Types of Data Models (Detailed)

Data models can be created at different levels of abstraction depending on **purpose, audience, and stage of the initiative**.  
Understanding these types helps a Business Analyst choose the **right level of detail at the right time**.

![ChatGPT Image Dec 29, 2025, 12_23_53 PM](https://github.com/user-attachments/assets/5dbd720a-3d29-42a3-9376-173807bc5a43)

---

### 5.1 Conceptual Data Model

A Conceptual Data Model provides a **high-level, business-focused view** of the key entities and how they relate to each other.  
It focuses on **what data exists**, not how it is stored or implemented.

**What it includes:**
- Core business entities
- High-level relationships between entities
- Business terminology

**What it deliberately excludes:**
- Attributes
- Data types
- Keys
- Technical constraints

**Primary audience:**
- Business stakeholders
- Product owners
- Senior management

**When to use:**
- Early stages of an initiative
- During discovery or strategy analysis
- When establishing a shared business vocabulary
- Before detailed requirements are defined

**Advantages:**
- Easy for non-technical stakeholders to understand
- Establishes common language
- Prevents misunderstanding of core concepts

**Limitations:**
- Not detailed enough for system design
- Cannot be directly implemented

**Example (Banking / IT):**
Entities such as **Customer**, **Account**, **Transaction**, and **Product**, with simple relationships like “Customer owns Account”.

---

### 5.2 Logical Data Model

A Logical Data Model expands on the conceptual model by defining **attributes, relationships, and business rules**, while remaining **independent of specific technology or databases**.

It represents **how data is logically structured** from a business perspective.

**What it includes:**
- Entities and attributes
- Primary and foreign keys (logical)
- Relationships and cardinality
- Business rules and constraints

**What it excludes:**
- Database-specific data types
- Indexes
- Storage or performance considerations

**Primary audience:**
- Business Analysts
- Data Analysts
- Solution Architects
- Designers

**When to use:**
- During requirements analysis
- When defining data requirements
- Before physical database design
- When integrating multiple systems

**Advantages:**
- Clear and detailed
- Technology-agnostic
- Bridges business and technical understanding

**Limitations:**
- Requires more effort and validation
- Still not directly deployable

**Example (Banking / IT):**
Defining **Account** with attributes such as Account_Number, Account_Type, Balance, and Status, including rules like “Account_Number must be unique”.

---

### 5.3 Physical Data Model

A Physical Data Model represents **how data is actually stored and implemented** in a specific database or system.  
It translates the logical model into a **technology-specific design**.

This model is typically owned and maintained by **technical teams**, with BA involvement for validation.

**What it includes:**
- Tables and columns
- Data types and sizes
- Indexes
- Constraints
- Database-specific features

**Primary audience:**
- Database designers
- Developers
- Data engineers

**When to use:**
- During system design and build
- When implementing databases
- For performance and storage optimization

**Advantages:**
- Directly implementable
- Optimized for performance and storage

**Limitations (from BA perspective):**
- Highly technical
- Less accessible to business stakeholders
- Tied to specific technology

**Example (Banking / IT):**
SQL tables such as `CUSTOMER_TBL` and `ACCOUNT_TBL` with defined column types, indexes, and constraints.

---

## 5.4 Comparison of Data Model Types

| Aspect | Conceptual | Logical | Physical |
|------|-----------|---------|----------|
| Level of Detail | Very High-level | Detailed | Very Detailed |
| Business Focus | High | Medium | Low |
| Technical Focus | None | Low | High |
| Attributes Included | No | Yes | Yes |
| Technology Dependent | No | No | Yes |
| Primary Owner | Business Analyst | BA / Architect | Technical Teams |
| Used For | Shared understanding | Requirements & design | Implementation |

---

## Key Takeaway

Data modelling progresses from **conceptual → logical → physical** as understanding and design maturity increase.  
Business Analysts primarily focus on **conceptual and logical models**, ensuring business meaning and data requirements are correct before technical implementation begins.


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
