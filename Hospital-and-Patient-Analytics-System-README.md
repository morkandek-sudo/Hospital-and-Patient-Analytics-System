# 🏥 Hospital & Patient Analytics System

A **MySQL-based Hospital Management and Patient Analytics System**
designed to manage hospital operations, patient care workflows,
laboratory activity, admissions, billing, insurance claims, user access,
and audit information.

This project demonstrates practical **SQL database design, relational
data modeling, joins, aggregation, subqueries, reporting, and
analytics** using a realistic hospital-management dataset.

> **Portfolio focus:** SQL / MySQL • Relational Database Design • Data
> Analysis • Healthcare Analytics

------------------------------------------------------------------------

## 📌 Project Overview

The Hospital & Patient Analytics System models the complete journey of a
patient through a hospital:

**Hospital → Department → Doctor → Patient → Appointment → Encounter →
Diagnosis / Vitals / Clinical Notes → Prescription → Laboratory →
Admission → Discharge → Services → Invoice → Payment → Insurance Claim**

It also includes **users, roles, permissions, and audit logging** for
administrative and security-related activities.

The project is suitable for:

-   SQL practice
-   MySQL database projects
-   Data Analyst portfolios
-   SQL interview preparation
-   Healthcare analytics demonstrations
-   Power BI / reporting preparation

------------------------------------------------------------------------

## 🎯 Project Objectives

1.  Store and manage hospital master data.
2.  Maintain patient and insurance information.
3.  Manage doctors, departments, wards, rooms, and beds.
4.  Track appointments and patient encounters.
5.  Store diagnoses, vitals, clinical notes, and prescriptions.
6.  Manage laboratory tests, orders, and results.
7.  Track admissions, bed assignments, and discharges.
8.  Manage hospital services and billing.
9.  Track invoices, invoice items, payments, and insurance claims.
10. Maintain users, roles, permissions, and audit activity.
11. Enable SQL-based operational and analytical reporting.

------------------------------------------------------------------------

## 🛠️ Technologies Used

  Technology             Purpose
  ---------------------- ----------------------------------------------------
  **MySQL**              Relational database
  **MySQL Workbench**    Database development and SQL execution
  **SQL**                Data definition, manipulation, joins and analytics
  **GitHub**             Version control and project portfolio
  **Power BI / Excel**   Optional reporting and visualization layer

------------------------------------------------------------------------

## 🗄️ Database Scope

The project contains **31 major tables** covering hospital operations,
patient care, laboratory, admission, billing, insurance, and security.

### 🏢 Organization & Infrastructure

-   `Hospital`
-   `Department`
-   `Ward`
-   `Room`
-   `Bed`

### 👨‍⚕️ Medical & Master Data

-   `Doctor`
-   `Medicine`
-   `Lab_Test`
-   `Service`

### 👤 Patient Management

-   `Patient`
-   `Patient_Insurance`

### 🔐 Users & Security

-   `User`
-   `Role`
-   `Permission`
-   `Audit_Log`

### 🩺 Clinical Workflow

-   `Appointment`
-   `Encounter`
-   `Diagnosis`
-   `Vital`
-   `Clinical_Note`
-   `Prescription`
-   `Prescription_Item`

### 🧪 Laboratory

-   `Lab_Order`
-   `Lab_Result`

### 🛏️ Admission & Discharge

-   `Admission`
-   `Bed_Assignment`
-   `Discharge`

### 💰 Billing & Insurance

-   `Invoice`
-   `Invoice_Item`
-   `Payment`
-   `Insurance_Claim`

------------------------------------------------------------------------

## 📊 Dataset Size

The supplied hospital data contains approximately **36,811 inserted
records** across the 31 tables.

  Table                 Records
  ------------------- ---------
  Hospital                    1
  Department                 50
  Ward                       50
  Room                      200
  Bed                     1,000
  Doctor                     50
  Medicine                1,500
  Patient                 2,000
  Patient_Insurance          20
  User                       20
  Role                       20
  Permission                 50
  Appointment             3,000
  Encounter               2,500
  Diagnosis               2,500
  Vital                   2,500
  Clinical_Note           2,500
  Prescription            2,000
  Prescription_Item       4,000
  Lab_Test                   50
  Lab_Order               3,000
  Lab_Result              2,500
  Admission                 500
  Bed_Assignment            500
  Discharge                 250
  Service                    50
  Invoice                 1,000
  Invoice_Item            2,000
  Payment                 1,500
  Insurance_Claim           500
  Audit_Log               1,000

------------------------------------------------------------------------

## 🔗 Main Relationships

The database follows a relational structure where operational entities
are connected using primary and foreign keys.

### Core relationships

``` text
Hospital
   │
   ├── Department
   │      ├── Doctor
   │      └── Ward
   │             └── Room
   │                    └── Bed
   │
   └── Patient
          │
          ├── Patient_Insurance
          ├── Appointment
          │      └── Encounter
          │             ├── Diagnosis
          │             ├── Vital
          │             ├── Clinical_Note
          │             └── Prescription
          │                    └── Prescription_Item
          │
          ├── Lab_Order
          │      └── Lab_Result
          │
          ├── Admission
          │      ├── Bed_Assignment
          │      └── Discharge
          │
          └── Invoice
                 ├── Invoice_Item
                 ├── Payment
                 └── Insurance_Claim
```

------------------------------------------------------------------------

## 🧩 Functional Modules

### 1. Hospital & Department Management

Stores hospital information and organizes departments by type, floor,
and contact details.

### 2. Ward, Room & Bed Management

Tracks wards, rooms, room types, charges, and bed allocation.

### 3. Doctor Management

Maintains doctor information and connects doctors with departments and
appointments.

### 4. Patient Management

Stores patient demographic and contact information and connects patients
to appointments, clinical records, admissions, billing, and insurance.

### 5. Appointment & Encounter Management

Tracks scheduled appointments and the resulting patient encounters.

### 6. Clinical Management

Stores:

-   Diagnoses
-   Vital signs
-   Clinical notes
-   Prescriptions
-   Prescription items

### 7. Laboratory Management

Tracks laboratory tests, lab orders, and laboratory results.

### 8. Admission Management

Handles admissions, bed assignments, and discharge records.

### 9. Billing Management

Tracks:

-   Services
-   Invoices
-   Invoice items
-   Payments

### 10. Insurance Management

Tracks patient insurance policies and insurance claims.

### 11. Security & Audit Management

Tracks users, roles, permissions, and audit events such as:

-   `LOGIN`
-   `VIEW`
-   `INSERT`
-   `UPDATE`
-   `DELETE`

------------------------------------------------------------------------

## 💡 SQL Concepts Demonstrated

This project can be used to demonstrate the following SQL skills:

### Basic SQL

-   `SELECT`
-   `INSERT`
-   `UPDATE`
-   `DELETE`
-   `WHERE`
-   `ORDER BY`
-   `LIMIT`
-   `DISTINCT`

### Filtering & Operators

-   `IN`
-   `BETWEEN`
-   `LIKE`
-   `IS NULL`
-   `IS NOT NULL`
-   Comparison operators
-   Logical operators

### Aggregation

-   `COUNT()`
-   `SUM()`
-   `AVG()`
-   `MIN()`
-   `MAX()`
-   `GROUP BY`
-   `HAVING`

### Joins

-   `INNER JOIN`
-   `LEFT JOIN`
-   `RIGHT JOIN`
-   Self Join
-   Cross Join
-   Multi-table joins

### Advanced SQL

-   Subqueries
-   Correlated subqueries
-   `EXISTS`
-   `IN`
-   `ANY`
-   `ALL`
-   `UNION`
-   `UNION ALL`
-   `CASE`
-   `COALESCE`
-   Common Table Expressions (CTEs)
-   Window functions
-   Views
-   Indexes
-   `EXPLAIN`
-   Transactions

------------------------------------------------------------------------

## 📈 Example Analytical Questions

The database can answer business questions such as:

1.  How many patients are registered?
2.  How many appointments are scheduled for each doctor?
3.  Which departments have the highest number of appointments?
4.  Which doctors have the highest workload?
5.  Which patients have never had an appointment?
6.  What is the average doctor salary?
7.  What are the top 5 highest-paid doctors?
8.  Which patients have multiple appointments?
9.  Which laboratory tests are ordered most frequently?
10. Which medicines are prescribed most frequently?
11. How many admissions occur each month?
12. What is the average hospital stay?
13. Which beds are currently occupied?
14. Which rooms are available?
15. What is the total invoice amount for each patient?
16. How much payment has been received for each invoice?
17. Which invoices are pending or partially paid?
18. What is the monthly hospital revenue?
19. Which insurance claims are approved, partially approved, or
    rejected?
20. Which users generate the most audit activity?

------------------------------------------------------------------------

## 🔍 Sample SQL Queries

### Total Number of Patients

``` sql
SELECT COUNT(*) AS total_patients
FROM Patient;
```

### Patients by Gender

``` sql
SELECT gender, COUNT(*) AS patient_count
FROM Patient
GROUP BY gender;
```

### Doctors by Department

``` sql
SELECT
    d.department_name,
    COUNT(doc.doctor_id) AS doctor_count
FROM Department d
LEFT JOIN Doctor doc
    ON d.department_id = doc.department_id
GROUP BY d.department_id, d.department_name
ORDER BY doctor_count DESC;
```

### Appointment Report

``` sql
SELECT
    a.appointment_id,
    p.patient_name,
    doc.doctor_name,
    d.department_name,
    a.appointment_date
FROM Appointment a
JOIN Patient p
    ON a.patient_id = p.patient_id
JOIN Doctor doc
    ON a.doctor_id = doc.doctor_id
JOIN Department d
    ON doc.department_id = d.department_id
ORDER BY a.appointment_date;
```

### Patients With No Appointment

``` sql
SELECT
    p.patient_id,
    p.patient_name
FROM Patient p
LEFT JOIN Appointment a
    ON p.patient_id = a.patient_id
WHERE a.appointment_id IS NULL;
```

### Total Payment by Invoice

``` sql
SELECT
    invoice_id,
    SUM(amount) AS total_paid
FROM Payment
GROUP BY invoice_id;
```

### Monthly Revenue

``` sql
SELECT
    YEAR(payment_date) AS payment_year,
    MONTH(payment_date) AS payment_month,
    SUM(amount) AS monthly_revenue
FROM Payment
GROUP BY YEAR(payment_date), MONTH(payment_date)
ORDER BY payment_year, payment_month;
```

### Top 3 Doctors by Salary

``` sql
SELECT
    doctor_id,
    doctor_name,
    salary
FROM Doctor
ORDER BY salary DESC
LIMIT 3;
```

------------------------------------------------------------------------

## 📊 Potential Power BI Dashboard

The SQL database can be connected to Power BI to create a hospital
analytics dashboard.

### KPI Cards

-   Total Patients
-   Total Doctors
-   Total Appointments
-   Total Admissions
-   Total Revenue
-   Total Payments
-   Pending Invoices
-   Insurance Claims

### Recommended Visuals

  Dashboard Area               Suggested Visualization
  ---------------------------- -------------------------
  Patient Overview             KPI Cards
  Patients by Gender           Donut / Pie Chart
  Patients by City             Bar Chart
  Appointments by Department   Column Chart
  Doctor Workload              Bar Chart
  Monthly Appointments         Line Chart
  Monthly Revenue              Line Chart
  Invoice Status               Donut Chart
  Bed Availability             Stacked Bar Chart
  Lab Test Usage               Bar Chart
  Insurance Claim Status       Column / Donut Chart
  Audit Activity               Line / Column Chart

------------------------------------------------------------------------

## 🧠 Data Analyst Skills Demonstrated

This project demonstrates practical experience with:

-   Relational database design
-   Data modeling
-   Data cleaning concepts
-   SQL querying
-   Data aggregation
-   Multi-table joins
-   Healthcare data analysis
-   KPI development
-   Business reporting
-   Analytical problem solving
-   Database normalization
-   Referential integrity
-   Query optimization concepts
-   Data visualization preparation

------------------------------------------------------------------------

## 🚀 How to Run the Project

### Step 1 --- Install MySQL

Install:

-   MySQL Server
-   MySQL Workbench

### Step 2 --- Create the Database

``` sql
CREATE DATABASE Hospital_Management;
USE Hospital_Management;
```

### Step 3 --- Create Tables

Run the table-creation / schema SQL script first, if provided
separately.

### Step 4 --- Load the Data

Run the hospital data SQL file after the required tables have been
created.

The recommended loading order follows the dependency structure:

``` text
Hospital
→ Department
→ Ward
→ Room
→ Bed
→ Doctor / Medicine / Patient
→ Appointment
→ Encounter
→ Clinical tables
→ Laboratory
→ Admission
→ Billing
→ Insurance
→ Audit
```

### Step 5 --- Verify the Data

``` sql
SHOW TABLES;

SELECT COUNT(*) FROM Patient;
SELECT COUNT(*) FROM Appointment;
SELECT COUNT(*) FROM Invoice;
SELECT COUNT(*) FROM Payment;
```

------------------------------------------------------------------------

## 📁 Recommended GitHub Repository Structure

``` text
Hospital-and-Patient-Analytics-System/
│
├── README.md
│
├── SQL/
│   ├── 01_Create_Database.sql
│   ├── 02_Create_Tables.sql
│   ├── 03_Insert_Data.sql
│   └── 04_Analytics_Queries.sql
│
├── Documentation/
│   └── Hospital_Project_Documentation.pdf
│
├── ER_Diagram/
│   └── Hospital_ER_Diagram.png
│
└── Screenshots/
    ├── Database.png
    ├── Tables.png
    └── Query_Results.png
```

> If your current repository contains one combined SQL file, you can
> keep it initially and split it into the above files later for easier
> navigation.

------------------------------------------------------------------------

## 🔐 Data Privacy Note

This repository is intended for **educational and portfolio purposes**.

The dataset should contain **synthetic/demo data only**. Do not upload
real patient records, medical reports, phone numbers, email addresses,
credentials, API keys, passwords, or other personally identifiable
information to a public repository.

------------------------------------------------------------------------

## 🔮 Future Improvements

Possible extensions include:

-   Build a Power BI hospital dashboard
-   Add stored procedures
-   Add database views for reporting
-   Add triggers for audit automation
-   Add indexes for high-volume queries
-   Add role-based access control
-   Add automated database backup
-   Add query-performance analysis using `EXPLAIN`
-   Build a Python backend/API
-   Add a web-based patient portal
-   Add automated ETL/data pipelines
-   Add advanced healthcare KPIs

------------------------------------------------------------------------

## 📚 Project Learning Outcomes

After completing this project, the following concepts can be
demonstrated in an interview:

-   How primary and foreign keys maintain relationships
-   How normalized tables reduce data duplication
-   How to join multiple hospital tables
-   How to use `GROUP BY` and `HAVING`
-   How to write subqueries and CTEs
-   How to use window functions
-   How to calculate hospital KPIs
-   How to analyze revenue and payments
-   How to identify patients without appointments
-   How to analyze doctor workload
-   How to analyze bed utilization
-   How to analyze insurance claims
-   How to optimize SQL queries

------------------------------------------------------------------------

## 👨‍💻 Author

**Morkande Kalyan**

Aspiring Data Analyst \| SQL \| MySQL \| Excel \| Python \| Power BI

------------------------------------------------------------------------

## ⭐ Portfolio

If you find this project useful, feel free to **star the repository**
and explore the SQL queries.

------------------------------------------------------------------------

## 📌 Repository

**Hospital & Patient Analytics System**

`Hospital-and-Patient-Analytics-System`

Built with **MySQL and SQL** for learning, analytics, and portfolio
development.
