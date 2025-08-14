
# Java JDBC - Employee Database Application

This project is a Java-based console application for managing employee records in a database. 
It demonstrates the use of JDBC (Java Database Connectivity) to connect to a MySQL database 
and perform basic CRUD operations.

## Features
- Add a new employee record
- Display all employees
- Update an employee's information
- Delete an employee from the database

## Requirements
- Java Development Kit (JDK) 8 or above
- MySQL database server
- MySQL Connector/J JDBC driver
- Code editor such as VS Code, IntelliJ IDEA, or Eclipse

## Database Setup
1. Create a database in MySQL:
   ```sql
   CREATE DATABASE employee_db;
   USE employee_db;
   ```

2. Create the table structure:
   ```sql
   CREATE TABLE employees (
       id INT PRIMARY KEY AUTO_INCREMENT,
       name VARCHAR(100) NOT NULL,
       department VARCHAR(100),
       salary DOUBLE
   );
   ```

3. Optional: Insert sample data for testing.

## How to Run
1. Download the MySQL Connector/J and add it to your project's classpath.
2. Update the database credentials in the Java code:
   ```java
   private static final String URL = "jdbc:mysql://localhost:3306/employee_db";
   private static final String USER = "root";
   private static final String PASSWORD = "your_password";
   ```
3. Compile and run the program from your terminal or IDE:
   ```bash
   javac EmployeeDBApp.java
   java EmployeeDBApp
   ```

## Example Menu
```
1. Add Employee
2. View Employees
3. Update Employee
4. Delete Employee
5. Exit
```

