# Week 1 – Understanding the Business Problem
### E-Commerce Order Management Database System

## Project Overview
This repository contains the Week 1 deliverables for the **E-Commerce Order Management Database
System** semester project. The goal of Week 1 is to analyze the business requirements of the
proposed system and produce the documentation that will guide the database design, ER modelling,
normalization, and SQL implementation in later weeks.

## Business Scenario
A rapidly growing e-commerce company needs a centralized database to manage customer
registration, product and category management, supplier and inventory tracking, order
processing, payment management, shipment tracking, and customer reviews — with the goal of
reducing data redundancy, improving accuracy, and enabling reliable business reporting.

## Core Entities
The project uses nine fixed core entities (no entities or attributes may be added, removed, or
renamed):

| Entity | Key Attributes |
|---|---|
| Customer | Customer ID, Name, Email, Mobile Number, Address, Registration Date |
| Category | Category ID, Category Name, Description |
| Product | Product ID, Product Name, Price, Stock Quantity, Category ID |
| Supplier | Supplier ID, Supplier Name, Contact Information |
| Order | Order ID, Customer ID, Order Date, Total Amount, Order Status |
| Order Details | Order Detail ID, Order ID, Product ID, Quantity, Unit Price |
| Payment | Payment ID, Order ID, Payment Method, Payment Date, Payment Status |
| Shipment | Shipment ID, Order ID, Delivery Address, Shipment Date, Delivery Status |
| Review | Review ID, Customer ID, Product ID, Rating, Comments |

## Repository Structure
```
Week1/
├── Requirement_Analysis_Report.pdf     # Business scenario analysis, entity purposes,
│                                        # business processes, stakeholder analysis
├── Business_Requirement_Document.pdf   # Functional & non-functional requirements,
│                                        # project scope, assumptions & constraints
├── SRS_Document.pdf                    # Formal Software Requirement Specification
└── README.md                           # This file
```

## Document Summaries

**Requirement_Analysis_Report.pdf**
- Business scenario analysis
- Purpose of each core entity
- Major business processes
- Stakeholder analysis

**Business_Requirement_Document.pdf**
- Functional requirements (by module: Customer, Product/Category, Supplier, Inventory, Order,
  Payment, Shipment, Review, Reporting)
- Non-functional requirements (performance, security, scalability, usability, etc.)
- Project scope (in-scope / out-of-scope)
- Assumptions and constraints

**SRS_Document.pdf**
- Introduction (purpose, scope, definitions, references)
- Overall description (product perspective, user classes, operating environment, constraints)
- Specific requirements (functional requirements, entity/attribute data requirements,
  non-functional requirements)
- Appendix (entity-relationship summary)

## How to Use
1. Read `Requirement_Analysis_Report.pdf` for the business context and entity/stakeholder
   analysis.
2. Read `Business_Requirement_Document.pdf` for the detailed requirement list and scope.
3. Read `SRS_Document.pdf` for the consolidated, formal specification used as the baseline for
   Week 2 (ER Modelling) and beyond.

## Project Roadmap
- **Week 1:** Business requirement analysis & SRS (this submission)
- **Week 2+:** ER modelling, normalization, SQL schema implementation, and report generation
  (to follow in subsequent weeks)

## Author
Prepared as an original submission for the E-Commerce Order Management Database System semester
project

Name: Akash raj T

Course: Database Management System (DBMS)

Project: E-Commerce Order Management Database System

Week 1: – Understanding the Business Problem.

# Week 2 – Entity and Relationship Analysis
### E-Commerce Order Management Database System

## Project Overview
This folder contains the Week 2 deliverables for the **E-Commerce Order Management Database
System** semester project. Building on the Week 1 Software Requirement Specification (SRS), Week
2 identifies every entity's attributes, keys, and constraints, and analyzes the relationships and
cardinalities between entities in preparation for normalization and SQL implementation.

## Scope of This Week
- Identification of all entities required for the system
- Full attribute list for each entity
- Primary Key (PK) identification, including NOT NULL, UNIQUE, CHECK, and DEFAULT constraints
- Foreign Key (FK) identification wherever applicable
- Relationship analysis between entities
- Cardinality analysis (One-to-One, One-to-Many, Many-to-Many)
- Consolidated Entity-Relationship (ER) diagram

## Repository Structure
```
Week2/
├── Entity_Analysis_Report.pdf          # Entity identification, attribute list,
│                                        # PK/FK identification with constraints
├── Entity_Relationship_Analysis.pdf    # Relationship analysis, cardinality analysis,
│                                        # and consolidated ER diagram
└── README.md                           # This file
```

## Document Summaries

**Entity_Analysis_Report.pdf**
- Entity identification (all 9 core entities and their role: master vs. transaction)
- Full attribute list per entity, with SQL data types
- Primary Key, Foreign Key, NOT NULL, UNIQUE, CHECK, and DEFAULT constraints for every attribute
- Consolidated PK/FK summary table
- Notes and assumptions (including the Supplier–Product linkage limitation, see below)

**Entity_Relationship_Analysis.pdf**
- Relationship analysis for every foreign key link between entities
- Cardinality analysis (1:1, 1:M, M:N) with participation rules
- Entity-Relationship diagram covering all 9 entities
- Summary of the overall data model

## Key Findings
- **9 entities**, **8 enforceable relationships**: 6 one-to-many, 2 one-to-one, and 1 many-to-many
  (Order ↔ Product) resolved through the **Order Details** associative entity.
- **Supplier** could not be linked via foreign key to any other entity because the fixed Week 1
  attribute list does not include a `Supplier_ID` attribute on `Product`. This is documented as a
  known limitation of the current fixed schema, carried forward from Week 1, rather than a
  modelling omission.

## How to Use
1. Read `Entity_Analysis_Report.pdf` for the full attribute-level data dictionary (types, keys,
   constraints) for every entity.
2. Read `Entity_Relationship_Analysis.pdf` for how the entities connect to one another and the ER
   diagram that will drive schema implementation.

## Project Roadmap
- **Week 1:** Business requirement analysis & SRS ✅
- **Week 2:** Entity and relationship analysis (this submission) ✅
- **Week 3+:** Normalization and SQL schema implementation (to follow)

## Author
Prepared as an original submission for the E-Commerce Order Management Database System semester
project.
Name: Akash raj T

Course: Database Management System (DBMS)

Project: E-Commerce Order Management Database System

Week 2: Entity and Relationship Analysis

