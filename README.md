# motor_corp_MSSQL_project
MS SQL Course Motors Certification Database Project

## 📚 Introduction

This project was created as part of the **Microsoft SQL Server Certification Course** by Brain4ce Education Solutions Pvt. Ltd. It focuses on designing and managing a relational database for **HerculesMotoCorp**, a major retailer and garage service provider in the United States.

The goal of the project is to build a robust, scalable, and query-efficient SQL Server database that not only fulfills internal data management needs but also supports insights for external stakeholders like shareholders and government authorities.

## 🧾 Scenario

**HerculesMotoCorp** deals with a wide range of automobiles and custom vehicles. Given the nature of their business and legal obligations, they require a structured and maintainable database system. As the designated **Database Administrator**, your role is to design, implement, and manage the database system effectively.

## 🎯 Tasks

The following tasks were completed in the project:

### 📌 Database & Schema Design
* Database created as **MotorsCertification**
* ER diagram designed with proper relationships, keys, and indexing
* Tables created:
  * `orderdetails`
  * `customers`
  * `employees`
  * `orders`
  * `offices`
  * `payments`
  * `productlines`
  * `products`

### 🧩 Data Operations
* Records inserted into the tables using provided CSV files
* Insert operations verified with `SELECT` queries
* Useless columns removed from `productlines`

### 🔍 Queries & Views
* Retrieved highest and lowest payment amounts
* Calculated unique count of customer names
* Created and managed a view: `cust_payment`
* Dropped the view after operation

### ⚙️ Stored Procedure, Functions, Triggers
* **Stored Procedure:** Display `productLine` for 'Classic Cars'
* **Function:** Fetch customers with `creditLimit` less than 96800
* **Triggers:**
  * On insert into `employees` to log transaction info
  * On high payment (`amount > 10000`) to log `customerNumber`

### 👤 Security & Access Control
* Created roles and logins:
  * `Admin`: Full access
  * `HR`: Access to `employees` and `offices` only
  * `Employee`: Read-only access to all tables
* Role-based access control implemented

### ⏱️ Maintenance & Monitoring
* Scheduled SQL Job for database backups
* Used Activity Monitor for system diagnostics:
  * Tracked processes, resource waits, and expensive queries

### ☁️ Cloud Migration
* Migrated the SQL Server workload to **Azure SQL Database**

## 🛠️ Tools Used
* Microsoft SQL Server Management Studio (SSMS)
* Azure SQL Database
* Windows Task Scheduler / SQL Server Agent (for job scheduling)

## 📌 Note
> All operations and implementations have been performed from the **Admin role** to ensure consistent access privileges and database integrity.

