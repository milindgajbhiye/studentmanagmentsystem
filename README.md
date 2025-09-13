# 🎓 Student Management System

![Java](https://img.shields.io/badge/Java-23-orange?logo=java&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?logo=mysql&logoColor=white)
![IDE](https://img.shields.io/badge/IDE-IntelliJ%20IDEA-purple?logo=intellij-idea&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A simple **Java + MySQL CLI project** that helps manage student records efficiently.  
This project demonstrates **JDBC connectivity, CRUD operations, and OOP concepts** in Java.

---

## ✨ Features
- ➕ Add new students with details (Name, Age, Grade, etc.)  
- 📋 View all student records stored in the database  
- 🔍 Search students by ID or Name  
- ✏️ Update existing student details  
- ❌ Delete student records  
- 💾 Persistent storage using **MySQL**  
- 🖥️ Easy-to-use **menu-driven CLI interface**

---

## 🛠️ Tech Stack
| Component      | Technology |
|----------------|------------|
| Programming    | Java (JDK 23) |
| Database       | MySQL 8.0+ |
| Connectivity   | JDBC (MySQL Connector/J) |
| IDE            | IntelliJ IDEA Community Edition |

---

---

## ⚙️ Setup & Installation

### 🔧 Prerequisites
- Install **Java JDK 23**  
- Install **MySQL Server & Workbench**  
- Install **IntelliJ IDEA** (or any IDE of choice)  
- Download and add **MySQL Connector/J** (JDBC driver) to your project classpath  

### 🗄️ Database Setup
Run the following SQL in MySQL Workbench:
```sql
CREATE DATABASE student_db;
USE student_db;

CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    grade VARCHAR(10) NOT NULL
);
```
### Run the Program
----
## Clone the repository:
 - git clone https://github.com/your-username/StudentManagementSystem.git
 - cd StudentManagementSystem
## Update database credentials in StudentManagementSystem.java:
 - String url = "jdbc:mysql://localhost:3306/student_db";
 - String user = "root";
 - String password = "your_password";
## Compile and run:
 - javac StudentManagementSystem.java
 - java StudentManagementSystem

---

## 🤝 Contributing  
Contributions, issues, and feature requests are welcome!  
Feel free to **fork this repo** and submit a **pull request**.  

---

## 📜 License  
This project is licensed under the **MIT License**.  
You are free to **use, modify, and distribute** this project with proper attribution.  

