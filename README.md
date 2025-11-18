# SyntaxNova-Smart-Data-Manager-
# Syntax Data Manager

## Overview
Syntax Data Manager is a data-driven solution designed to simplify how organizations collect, manage, visualize, and interact with business data. The system integrates Azure SQL Database, Power BI, and Power Apps to deliver a seamless workflow for storing, analyzing, and presenting operational data.

---

## Project Purpose
The goal of the Syntax Data Manager is to build an efficient and scalable data platform that:
- Stores structured business data in Azure SQL.
- Allows interaction through a Power App interface.
- Provides insights through Power BI dashboards.
- Ensures structured data flow using ERDs and DFDs.

---

## Team Roles

### **Lerato Matamela – Data Engineer & Data Analyst**
- Cleaned and transformed datasets.
- Built Python scripts for Azure SQL ingestion.
- Designed and implemented SQL tables.
- Created DAX measures and Power BI reports.

### **Thelezinhle Buthelezi – Database Architect**
- Designed the ERD and DFD diagrams.
- Developed table structures and relationships.
- Supported Azure SQL configuration.

### **Thato Rapholo – Power App Developer**
- Developed the Power App interface.
- Connected the app to Azure SQL.
- Designed UI screens, forms, and CRUD logic.

---

## System Architecture

### **1. Azure SQL Database**
- Secure cloud-based storage.
- Relational structure defined by ERD.
- Integrated seamlessly with Power BI and Power Apps.

### **2. Power BI Analytics Dashboard**
- Overview page with KPIs.
- Sales and orders visual analytics.
- DAX-driven insights.

### **3. Power App Interface**
- Allows adding, editing, and viewing records.
- Validates and sends data to Azure SQL.
- Intuitive UI for non-technical users.

---

## Technologies Used
- Python (Pandas, SQLAlchemy, PyODBC)
- Azure SQL Database
- Power BI
- Power Apps
- SQL
- ERD and DFD modelling tools

---

## Key Features
- Automated data cleaning and transformation.
- Cloud-hosted SQL tables.
- Power BI dashboards with KPIs.
- Power App for CRUD operations.
- Secure and scalable architecture.

---

## Database Ingestion (Python Example)

```python
from sqlalchemy import create_engine

data.to_sql(
    "Orders",
    con=engine,
    if_exists="replace",
    index=False
)
