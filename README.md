# Student Management System

This is a terminal-based application for managing student records using MySQL as the database with JDBC connection.

## Features

- Add new students to the database.
- Display all existing students.
- Get student details based on their roll number.
- Delete students from the database.
- Update student information.
- Exit the application.

## Requirements

- MySQL Database
- JDBC Driver for MySQL

## Installation

1. Clone or download the repository.  
2. Update the database connection details in DBCnnection.java.

## Database Setup

1. Create a MySQL database named `student`:
    ```sql
    CREATE DATABASE IF NOT EXISTS student;
    ```

2. Switch to the `student` database:
    ```sql
    USE student;
    ```

3. Create a table named `student_details` with the necessary columns:
    ```sql
    CREATE TABLE IF NOT EXISTS student_details (
        rollnum INT(11) PRIMARY KEY AUTO_INCREMENT,
        sname VARCHAR(100) NOT NULL,
        clgname VARCHAR(50),
        city VARCHAR(50),
        percentage DOUBLE(10,2)
    );
    ```

4. Verify that the table `student_details` is created:
    ```sql
    SHOW TABLES;
    ```

5. Optionally, you can check the structure of the `student_details` table by executing:
    ```sql
    DESCRIBE student_details;
    ```
    
## Usage

1. Start the application with `client.java`.
2. Follow the menu options to perform operations.
3. Exit the application when done.

## Contributing

I welcome contributions from the community to improve the Student Management System.
