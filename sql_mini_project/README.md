# Digital Library Audit System (SQL Mini Project)

## Project Overview

The **Digital Library Audit System** is a SQL-based mini project designed to manage and analyze library operations in a community college. It helps track book borrowings, identify overdue books, calculate penalties, and analyze book popularity.

This project demonstrates practical use of **relational database design, SQL queries, and data analysis techniques**.

---

## Objectives

* Design a structured relational database for library management
* Track issued and returned books
* Identify overdue books and generate penalty reports
* Analyze most popular book categories
* Maintain and clean inactive student records

---

## Database Schema

### 1. **Books Table**

Stores details about books available in the library.

* `BookID` (Primary Key)
* `Title`
* `Author`
* `Category`
* `AvailableCopies`

### 2. **Students Table**

Stores student information.

* `StudentID` (Primary Key)
* `Name`
* `Email`
* `Department`
* `JoinDate`
* `Status` (Active / Inactive)

### 3. **IssuedBooks Table**

Tracks book borrowing records.

* `IssueID` (Primary Key)
* `BookID` (Foreign Key)
* `StudentID` (Foreign Key)
* `IssueDate`
* `ReturnDate`

---

## ⚙️ Features Implemented

### 1. Table Creation (DDL)

* Created relational tables with primary and foreign keys
* Ensured proper data organization

### 2. Overdue Book Detection

* Identifies books not returned within **14 days**
* Displays student name, book title, and overdue days

### 3. Penalty Report

* Calculates penalty based on overdue duration
* Rule: ₹5 per day after 14 days

### 4. Book Popularity Analysis

* Uses `COUNT()` and `GROUP BY`
* Finds most borrowed book categories

### 5. Inactive Student Management

* Marks students as **Inactive** if no borrowing in last 3 years

### 6. View Creation

* Created `OverdueReport` view for quick access to overdue data

---

## Technologies Used

* **Database:** MySQL
* **Tool:** MySQL Workbench
* **Language:** SQL

---

## How to Run the Project

1. Open **MySQL Workbench**
2. Copy and paste the provided `.sql` file
3. Execute the script (Run All)
4. Run SELECT queries to view:

   * Overdue books
   * Penalty report
   * Category analysis

---

## Sample Queries Included

* Overdue book detection
* Penalty calculation
* Category-wise borrowing count
* Inactive student identification
---

## Future Enhancements

* Add **Triggers** for automatic fine calculation
* Implement **Stored Procedures** for reports
* Build a **GUI (Java/Python)** for user interaction
* Integrate **login/authentication system**
* Add **real-time notifications for overdue books**

---

## Learning Outcomes

* Understanding of relational database design
* Hands-on experience with SQL queries and joins
* Real-world problem solving using data analysis
* Knowledge of data maintenance and auditing

---

## Conclusion

This project successfully demonstrates how SQL can be used to build a **functional and analytical library system**. It improves efficiency in tracking records, supports decision-making, and ensures better data management.

---

## Author

**Name:** (Siddharth V)
**Course:** B.E. Computer Science and Engineering
**Project Type:** SQL Mini Project

---
