# Boston Transit Database System

A comprehensive SQL-based data management and analytics project designed to model and support the operations of a metropolitan transportation system. This project implements a full relational database with business rules, data integrity constraints, security mechanisms, and analytics-ready views commonly used in real-world Business Intelligence and Data Engineering environments.

---

##  Project Overview
This system captures key components of a transit network—users, tickets, cards, passes, routes, lines, stations, vehicles, drivers, and operational activity.  
It includes end-to-end SQL development:

- Relational schema design  
- Entity–relationship modeling  
- Data insertion and validation  
- Stored procedures for operational automation  
- Triggers for automatic business rule enforcement  
- Views for analytics, reporting, and dashboard use  
- User-defined functions for reusable logic  
- Encryption of sensitive data  
- Performance indexing for optimization  

The project mirrors real-world database scenarios used in healthcare, public transit, and enterprise BI systems.

---
##  Entity–Relationship Diagram (ERD)

The following ERD represents the complete relational model of the Boston Transit Database System.  
It illustrates all primary entities, their attributes, and the relationships between users, tickets, operations, routes, lines, stations, transportation methods, and drivers.

### ** ER Diagram**

![ER Diagram](279551077-1cebefcc-f435-4010-a34e-ac34f18289fd.png)

### **ERD Summary**
- **USERS** perform **OPERATIONS** using tickets.
- **TICKETS** can be of type **CARD** or **PASS**, with recharge activity tracked.
- **OPERATIONS** authorize **TRANSIT** events.
- **ROUTE** and **LINE** tables connect to **STATION** via associative tables.
- **BUS** and **TRAIN** tables store vehicle details.
- **DRIVER** entities link to vehicles via many-to-many relationships.

This ERD demonstrates a well-structured, normalized relational schema designed to support analytics, operational reporting, and business rules enforcement.

---

##  Key Features

###  **Relational Schema**
Normalized tables with foreign key relationships, constraints, and well-defined business rules.

###  **Operational SQL Components**
- **Stored Procedures:** Automated recharge logic, revenue aggregation, route/line utilization insights.
- **Triggers:** Auto-expiration of tickets based on card/pass updates.
- **UDFs:** Fare deductions and reusable calculation functions.

###  **Analytics & Reporting**
Includes BI-ready SQL views such as:
- User operations with ticket details  
- Spending habits and recharge summaries  
- Route and transportation availability  
- Station-level traffic analysis  

These support dashboarding tools like Tableau, Power BI, and Looker.

###  **Data Security**
AES-256 encryption of sensitive user data, ensuring privacy and compliance.

###  **Performance Optimization**
Non-clustered indexes added to speed up common lookups and analytical queries.


##  Project Structure
 Boston-Transit-Database-Project
┣  SchemaANDInsertionQueries.sql
┣  DMDD Final Project SP.sql
┣  dmdd final project trigger.sql
┣  DMDD Final Project view.sql
┣  UDF.sql
┣  non-clustered index.sql
┣  data encryption dmdd final project.sql
┗  README.md
##  Example Use Cases

- Identify high-utilization transit users  
- Monitor revenue by line or route  
- Detect unauthorized operations  
- Analyze station traffic patterns  
- Generate BI dashboards for operations & finance  
- Validate ticket/pass activity in real time  

---

##  Tech Stack

**Languages:** SQL (T-SQL)  
**Tools:** Microsoft SQL Server, SSMS  
**Concepts:** Database Design, Data Modeling, BI Analytics, Encryption, Indexing, ETL Logic  

---

##  Acknowledgements
Built as part of an academic database design project with real-world applicability for Business Intelligence, analytics, and operational reporting.

---

If you found this project helpful or insightful, consider starring ⭐ the repository!
