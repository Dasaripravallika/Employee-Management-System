# Employee-Management-System(EMS) – SQL Project
📌 Project Overview

The Employee Management System (EMS) is a relational database project designed to manage employee information, job departments, salaries, qualifications, leaves, and payroll records.

This project demonstrates database design, table relationships, and analytical SQL queries used to generate insights about employees, departments, salaries, and workforce trends.

🗂️ Database Name
EMS
🏗️ Database Schema
👨‍💼 Employee

Stores employee personal information.

Column	Description
emp_ID	Unique employee ID
firstname	Employee first name
lastname	Employee last name
gender	Gender
age	Employee age
contact_add	Address
emp_email	Email ID
emp_pass	Password
Job_ID	Job role reference
🏢 Job Department

Stores department and job role information.

Column	Description
Job_ID	Job ID
jobdept	Department name
name	Job role
description	Job description
salaryrange	Salary range
💰 SalaryBonus

Stores salary and bonus information for job roles.

Column	Description
salary_ID	Salary ID
Job_ID	Job reference
amount	Base salary
annual	Annual salary
bonus	Bonus amount
🎓 Qualification

Stores employee qualifications and skills.

Column	Description
QualID	Qualification ID
Emp_ID	Employee ID
Position	Qualification title
Requirements	Skills/requirements
Date_In	Date added
🌴 Leaves

Tracks employee leave records.

Column	Description
leave_ID	Leave ID
emp_ID	Employee ID
date	Leave date
reason	Reason for leave
💳 Payroll

Stores employee payroll details.

Column	Description
payroll_ID	Payroll ID
emp_ID	Employee ID
job_ID	Job reference
salary_ID	Salary reference
leave_ID	Leave reference
date	Payroll date
report	Payroll report
total_amount	Final payment
🔗 Database Relationships

Key relationships in the database:

Employee → JobDepartment

SalaryBonus → JobDepartment

Qualification → Employee

Leaves → Employee

Payroll → Employee / SalaryBonus / JobDepartment / Leaves

These relationships ensure data consistency and integrity using foreign keys.

📊 SQL Analysis Performed
👨‍💼 Employee Insights

✔ Total number of employees
✔ Employees per department
✔ Average salary per department
✔ Top 5 highest paid employees
✔ Total salary expenditure

🏢 Job Role & Department Analysis

✔ Number of roles per department
✔ Average salary by department
✔ Highest paying roles
✔ Total department salary distribution

🎓 Qualification & Skills Analysis

✔ Employees with qualifications
✔ Most common qualifications
✔ Employees with highest number of qualifications

🌴 Leave & Absence Analysis

✔ Leave trends by year
✔ Average leaves by department
✔ Employees with highest leaves
✔ Total leave records

💰 Payroll & Compensation Analysis

✔ Monthly payroll trends
✔ Average bonus by department
✔ Highest bonus department
✔ Average final salary by department

🛠️ Technologies Used

🐬 MySQL

📊 SQL Queries

🗄️ Relational Database Design

📈 Project Highlights

✔ Database normalization
✔ Multiple table relationships
✔ Foreign key constraints
✔ Analytical SQL queries
✔ Workforce insights

🚀 How to Run the Project

1️⃣ Create database

CREATE DATABASE EMS;

2️⃣ Use database

USE EMS;

3️⃣ Run the SQL file

EMSproject.sql

4️⃣ Execute analysis queries.

📌 Future Improvements

✨ Add employee attendance tracking
✨ Create HR dashboard (Power BI / Tableau)
✨ Implement stored procedures
✨ Add triggers for payroll automation

👩‍💻 Author

Dasari Pravallika

Aspiring Data Analyst skilled in:

SQL

Power BI

Data Analysis

Data Visualization
