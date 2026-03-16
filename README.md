# 🎓 Student Management System

![Java](https://img.shields.io/badge/Java-23-orange?logo=java&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?logo=mysql&logoColor=white)
![IDE](https://img.shields.io/badge/IDE-IntelliJ%20IDEA-purple?logo=intellij-idea&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A simple **Java + MySQL CLI project** that helps manage student records efficiently.  
This project demonstrates **JDBC connectivity, CRUD operations, and OOP concepts** in Java.

---

## ✨ Features
- ➕ Add new students with details (Name, Age, Email)  
- 📋 View all student records stored in the database  
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

## ⚙️ Setup & Installation

### 🔧 Prerequisites
- Install **[Java JDK 23](https://www.oracle.com/java/technologies/downloads/)**
- Install **[MySQL Server 8.0+](https://dev.mysql.com/downloads/mysql/)**
- Download **[MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/)** (JDBC driver JAR)

### 🗄️ Database Setup
Open MySQL shell or MySQL Workbench and run the following SQL:

```sql
CREATE DATABASE student_db;
USE student_db;

CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    email VARCHAR(100) NOT NULL
);
```

---

## 🚀 How to Run

### Step 1 — Clone the repository

```bash
git clone https://github.com/milindgajbhiye/studentmanagmentsystem.git
cd studentmanagmentsystem/JavaProject/Student\ Database\ Managment\ System/src
```

### Step 2 — Update database credentials

Open `StudentManagementSystem.java` and update the connection details to match your MySQL setup:

```java
static final String DB_URL = "jdbc:mysql://localhost:3306/student_db";
static final String USER   = "root";          // your MySQL username
static final String PASS   = "your_password"; // your MySQL password
```

### Step 3 — Compile the program

You must include the MySQL Connector/J JAR on the classpath when compiling and running.  
Replace `mysql-connector-j-8.x.x.jar` with the actual filename of the JAR you downloaded.

**On Linux / macOS:**
```bash
javac -cp .:mysql-connector-j-8.x.x.jar StudentManagementSystem.java
```

**On Windows:**
```cmd
javac -cp .;mysql-connector-j-8.x.x.jar StudentManagementSystem.java
```

### Step 4 — Run the program

**On Linux / macOS:**
```bash
java -cp .:mysql-connector-j-8.x.x.jar StudentManagementSystem
```

**On Windows:**
```cmd
java -cp .;mysql-connector-j-8.x.x.jar StudentManagementSystem
```

### 💡 Running with IntelliJ IDEA (alternative)

1. Open the project in **IntelliJ IDEA**.
2. Go to **File → Project Structure → Libraries** and add the `mysql-connector-j-8.x.x.jar`.
3. Update the database credentials inside `StudentManagementSystem.java`.
4. Right-click `StudentManagementSystem.java` → **Run 'StudentManagementSystem.main()'**.

---

## 🎮 Using the CLI Menu

Once the program starts and connects to the database, you will see:

```
Connected to database!

--- Student Management System ---
1. Add Student
2. Update Student
3. Delete Student
4. View All Students
5. Exit
Enter choice:
```

| Option | Description |
|--------|-------------|
| 1 | Prompts for student **Name**, **Age**, and **Email**, then inserts the record |
| 2 | Prompts for the student **ID** and new details, then updates the record |
| 3 | Prompts for the student **ID** and deletes that record |
| 4 | Displays all student records currently in the database |
| 5 | Exits the application |

---

## 🤝 Contributing  
Contributions, issues, and feature requests are welcome!  
Feel free to **fork this repo** and submit a **pull request**.  

---

## 📜 License  
This project is licensed under the **MIT License**.  
You are free to **use, modify, and distribute** this project with proper attribution.  

