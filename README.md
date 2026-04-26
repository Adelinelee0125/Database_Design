# Database Design Workshop 4 - Relational Schema

## Project Overview
This project is based on the [Modern Database Management] case study, focusing on logical database design. By applying EER modeling, relational mapping, and 3NF normalization, I have constructed an efficient database architecture that manages customers, vendors, inventory, and employee roles.

## Core Design Highlights
- **3NF Normalization**: Achieved Third Normal Form (3NF) by identifying and eliminating partial and transitive dependencies, ensuring atomic and non-redundant data storage.
- **Employee Role Management**: Utilized Supertype/Subtype modeling to effectively handle specialized attributes for Drivers, Customer Service, and Accountants, ensuring structural scalability.
- **Referential Integrity (RI)**: Implemented strict foreign key constraints and business rules to maintain data consistency across all related entities.

## Technical Challenges & Solutions
- **Challenge**: Managing complex Many-to-Many (M:N) relationships and heterogeneous employee data.
- **Solution**: Designed an `INVENTORY` associative entity to map Vendors to Products and employed Disjoint (d) constraints for the Employee hierarchy, reducing data maintenance complexity.

## Contents
- `workshop4_schema.sql`: Complete DDL script for database creation.
- `Relational_Schema_Design.pdf`: Logical design diagrams, EER modeling analysis, and functional dependency mapping.

## Environment
- Database: MySQL 8.0 / SQL Server 2022+
