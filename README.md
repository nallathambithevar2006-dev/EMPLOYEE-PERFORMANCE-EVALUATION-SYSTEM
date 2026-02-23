# EMPLOYEE-PERFORMANCE-EVALUATION-SYSTEM

The **Employee Performance Evaluation System** is a database-driven project developed using **MySQL**. It is designed to store, manage, and analyze employee performance data in a structured and efficient way.
This system replaces manual record-keeping methods with a relational database approach, ensuring data accuracy, consistency, and easy report generation.

##  Objectives

* Design a structured relational database.
* Store employee and evaluation details efficiently.
* Implement SQL queries for data manipulation.
* Maintain data integrity using constraints.
* Generate performance reports for decision-making.


##  Technologies Used

* **MySQL Server**
* **MySQL Workbench**
* **SQL (Structured Query Language)**
* Windows / Linux Operating System


##  Database Structure

The system consists of four main tables:

### 1️ Department

* Department_ID (Primary Key)
* Department_Name

### 2️ Employee

* Employee_ID (Primary Key)
* Employee_Name
* Department_ID (Foreign Key)
* Designation
* Date_Of_Joining

### 3️ Evaluator

* Evaluator_ID (Primary Key)
* Evaluator_Name
* Role

### 4️ Evaluation

* Evaluation_ID (Primary Key)
* Employee_ID (Foreign Key)
* Evaluator_ID (Foreign Key)
* Performance_Score (0–100)
* Remarks
* Evaluation_Date

---

##  Constraints Used

* **PRIMARY KEY** – Ensures unique records
* **FOREIGN KEY** – Maintains relationships between tables
* **NOT NULL** – Prevents empty values
* **CHECK** – Restricts performance score between 0 and 100

---

##  How to Run

1. Install MySQL Server and MySQL Workbench.
2. Create the database:

   ```sql
   CREATE DATABASE EmployeeEvaluation;
   USE EmployeeEvaluation;
   ```
3. Run table creation queries.
4. Insert sample data.
5. Execute SELECT queries to generate reports.

---

##  Sample Query

```sql
SELECT Employee_Name, Performance_Score
FROM Employee
JOIN Evaluation 
ON Employee.Employee_ID = Evaluation.Employee_ID;
```

This query retrieves employee names along with their performance scores.

---

##  Features

* Structured database design
* Efficient data storage and retrieval
* JOIN operations and advanced queries
* View creation for simplified reporting
* Basic security using user privileges
* Backup using `mysqldump`


##  Future Scope

* Web-based interface
* Graphical performance reports
* Automated performance analytics
* Integration with payroll system

---

## Author

**Mr. Nallathambi Shanmugavel Thevar**
S.Y. Information Technology (SYIT)
Roll No: 2542048



