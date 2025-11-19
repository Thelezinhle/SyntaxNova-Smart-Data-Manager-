Reflection
Overview

This project spanned from 12 November 2025 (Wednesday) to 18 November 2025 (Tuesday) and involved building the SYNTAX Data Manager, an internal business data management system integrating Power Apps, Azure SQL, Python ETL pipelines, and Power BI dashboards. The journey was as chaotic as any reasonable software project, but every challenge contributed to my technical and collaborative growth.

What Went Well
1. Smooth Collaboration Across Roles

Each team member had a distinct role:

Lerato Matamela: Python ETL, data cleaning, SQL loading, Power BI analytics

Thelezinhle Buthelezi: Database modelling, ERD/DFD diagrams, SQL structure

Thato Rapholo: Power App interface, CRUD forms, navigation

The clear division meant fewer collisions and more focused contributions.

2. Successful Data Cleaning and Transformation

Using Python, I removed duplicates, cleaned fields, fixed inconsistent statuses, repaired dates, and calculated profit values.
The cleaned dataset integrated cleanly into the Azure SQL database, enabling reliable CRUD operations in the Power App.

3. Full Pipeline Integration

The project achieved the full end-to-end pipeline:

Raw CSV → Python cleaning → Azure SQL → Power Apps CRUD → Power BI Insights
Seeing everything connect without exploding felt like a personal victory.

4. Strong Documentation

The GitHub repository includes:

Screenshots of the Power App

.msapp file

Raw and cleaned CSV files

ETL notebook

ER and DFD diagrams

README.md

reflection.md

The repository feels professional and complete.

Challenges Faced
1. Azure SQL Connection Frustrations

Connection strings fought back like they had something to prove.
Between drivers, encoding, and certificate settings, debugging took time.
Eventually, proper pyodbc formatting solved the issue.

2. Designing a Usable Power App UI

Creating forms that link correctly to SQL, validate inputs, and don’t break the schema took refinement.
Dropdown relationships (Supervisor → Orders) required careful lookups.

3. Data Standardization

Fixing inconsistent formats like:

differently written status values

missing supervisor names

mixed date formats

This slowed down ETL but improved final quality.

4. Time Pressure

One week is short for building a full data system.
Prioritizing critical features over “nice to haves” was necessary.

What I Learned
1. Real ETL Flow and Business Data Handling

I now understand how raw business data transforms into:

structured tables

dashboards

app-ready interfaces

Python’s pandas + SQLAlchemy workflow is now second nature.

2. Power Apps CRUD Architecture

I learned to:

connect apps to Azure SQL

build forms

patch data

configure navigation

It gave me a solid foundation for future low-code solutions.

3. SQL Modelling and Normalization

Working with the ERD taught me how tables relate in actual business systems:
Orders → Customers
Orders → Supervisors
Products → Categories
It was satisfying to see the model reflected in the running app.

4. Power BI Sales and Operations Analytics

Sales trends, supervisor performance, profit metrics — turning cleaned data into insights felt meaningful.

What I Would Improve Next Time

Add authentication roles (Manager / Supervisor / Staff)

Add automated alerts or workflows using Power Automate

Add more advanced measures, like forecasted sales

Document the SQL schema even more deeply

Expand the app UI for tablet mode

Final Thoughts

This project taught me how multiple platforms can combine into a cohesive business system.
Even though the deadline was tight, the final product works end-to-end:
data → storage → app → insight.

There were moments where the tech stack felt like a stubborn toddler, but solving each problem made the final result more rewarding.
The SYNTAX Data Manager project strengthened my confidence in data engineering, collaboration, and full lifecycle design.
