# Assignment_09_033_PIJL

# Java + MySQL Student Management System

**Name:** Dhaerya More  
**PRN:** 23070126033  
**Batch:** A2  

---

## Overview

This project is a **Java-based student record management system** connected to a **MySQL database**. It allows users to:

- Add a new student
- Display all students
- Search student by PRN
- Delete student by ID

The program uses JDBC to connect to MySQL and performs all operations on a table named `students`.

---

## Files in the Project

| File                | Description |
|---------------------|-------------|
| `Main.java`         | Launches the application via the `menu()` method in `StudentApp` |
| `Student.java`      | Java Bean class with student properties (`id`, `name`, `prn`, `age`) |
| `DBConnection.java` | Provides a static method to return a MySQL database connection |
| `StudentApp.java`   | Contains menu, logic, and methods to add, display, search, and delete students |

---

## MySQL Database Details

You should create the following MySQL table before running the program:

```sql
CREATE DATABASE studentdb;

USE studentdb;

CREATE TABLE students (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  prn VARCHAR(20),
  age INT
);
