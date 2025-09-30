Library Management System

This project is a Java Project with MySQL as database. 
It handles all the basic functions required for an admin to run an library management system.

## Features
- Basic Login Page for admin to enter
- Dashboard has few button options to check functions
- Can see Book details, Add or Remove Books
- Can see Student details, Add or Remove Students also
- Can edit or see admin details with extra step authentication
- the MySQL has only 3 tables to maintain all the database

## Technologies Used
- Java (Swing, JDBC)
- NetBeans IDE (Platform)
- MySQL (Database)

## Setup Instructions
### 1. Clone this repository
```bash
git clone https://github.com/your-username/library-admin-panel.git
cd library-admin-panel
```
### 2. Database Setup
- Create a database named `library` in MySQL.
- Run the following SQL to create the `admin` table:
```sql
CREATE DATABASE library;
USE library;

CREATE TABLE admin (
    admin_id INT PRIMARY KEY,
    aname VARCHAR(50),
    pno VARCHAR(15),
    pass VARCHAR(50)
);

-- Insert a sample admin
INSERT INTO admin (admin_id, aname, pno, pass)
VALUES (1, 'Admin User', '9876543210', 'admin123');
```
- Can also create sample tables for books and students respectively also.
  
### 3. Configure Database Connection
In `Edit_Admin.java`, update these lines with your MySQL username and password:
```java
String url = "jdbc:mysql://localhost:3306/library?useSSL=false";
String mysqlUser = "root";
String mysqlPass = "your_mysql_password";
```

### 4. Run the Project
* Open the project in **NetBeans**
* Clean and Build the project
* Run codes.

## 📄 License

This project is licensed under the **MIT License** – free to use and modify.
Copyrights still belong to me.

---
