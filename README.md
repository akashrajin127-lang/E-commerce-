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

Week: 1 – Understanding the Business Problem.
