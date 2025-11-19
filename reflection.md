# Reflection

## Overview
This project, **SYNTAX Data Manager**, required us to build a complete internal data management ecosystem using Power Apps, Azure SQL, Python ETL, and Power BI. The goal was to centralize business data, support CRUD operations, clean raw datasets, and deliver analytics dashboards. The work demanded technical coordination across development, database design, and analytics.

## What Went Well

### Team Collaboration
Each team member worked within a clearly defined role:
- **Lerato Matamela** handled data cleaning, Python ETL, SQL data loading, and analytics.
- **Thelezinhle Buthelezi** designed the database structure, ER diagram, and DFD.
- **Thato Rapholo** created the Power App, built navigation, and implemented CRUD logic.

This separation of responsibilities made the workflow efficient and reduced confusion.

### ETL and Data Cleaning
The dataset was successfully cleaned and transformed:
- Fixed inconsistent statuses  
- Removed duplicates and blank rows  
- Standardized data types  
- Added calculated fields such as total amounts and profits  

The final dataset loaded into Azure SQL without structural issues.

### System Architecture
The ERD and DFD aligned well with the solution design. Normalizing the tables created a stable database that supported Power Apps forms and Power BI dashboards.

## Challenges Faced

### Azure SQL Connectivity Errors
Connecting Python to Azure SQL was the most time-consuming challenge. We dealt with:
- Timeouts  
- Incorrect driver configuration  
- Firewall restrictions  
- Special character issues in connection strings  

The problem was eventually solved using a properly encoded ODBC connection string.

### Cleaning an Inconsistent Dataset
The raw CSV had multiple issues that required attention:
- Missing customer or product details  
- Mismatched supervisor names  
- Wrong data types  
- Status values written differently  

Ensuring that the final cleaned CSV was usable took careful verification.

### Power Apps Database Integration
Building the CRUD interface required:
- Correct SQL table relationships  
- Delegation-safe formulas  
- Lookups for dropdown selections  
- Input validation  
- Testing different form modes  

Understanding Power Apps–SQL delegation rules was essential.

## Lessons Learned

### Technical Lessons
- How to build and execute a Python ETL pipeline  
- How to design a normalized SQL database  
- How Power Apps interacts with Azure SQL  
- How to develop DAX-powered dashboards in Power BI  
- Importance of indexing and foreign keys  
- Value of consistent data formats before migration  

### Project Skills
- Sprint planning and task assignment  
- Clean documentation for GitHub  
- Clear communication between roles  
- Version control and structuring repositories  

## Improvements for Future Versions

### Earlier Database Setup
The SQL schema should be finalized earlier to avoid delays when building Power Apps screens and loading data.

### Stronger Automation
Future updates could add:
- Automated ETL scheduling  
- Stored procedures and triggers  
- Error-logging mechanisms  
- Automatic integrity audits  

### Improved Power Apps UI
The app could use:
- Better layout spacing  
- Icons and consistent theming  
- More advanced filtering and search features  

## Final Reflection
The SYNTAX Data Manager project successfully combined multiple technologies into a single functioning pipeline. It demonstrated how raw data can evolve into a cleaned dataset, become part of a structured SQL database, fuel an interactive Power App, and empower decision-making through dashboards.

The project strengthened our skills in data engineering, database development, analytics, documentation, and teamwork. Despite technical frustrations along the way, the final solution is functional, scalable, and aligned with real business needs.
