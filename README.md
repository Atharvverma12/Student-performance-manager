# 🎓 Student Performance Management System

A **Java-based Command-Line Application** designed to manage student academic information, including student details, marks, attendance, and overall performance.

The system uses **Object-Oriented Programming (OOP)** concepts and **file handling** to store and retrieve student data for future use.

---

## 📌 Project Overview

The **Student Performance Management System** provides a simple and efficient way to manage academic records.

It allows users to:

* 👨‍🎓 Manage student information
* 📚 Store subject-wise marks
* 📊 Calculate total marks and percentage
* 🏆 Calculate grades
* 📅 Manage attendance records
* 📈 Analyze overall student performance
* 📄 Generate detailed student reports
* 💾 Store data using text files
* ✅ Validate user input

---

## ✨ Features

### 👨‍🎓 Student Management

The system provides options to:

* ➕ Add a student
* 👀 View all students
* 🔍 Search for a student
* ✏️ Update student details
* 🗑️ Delete a student

### 📚 Marks Management

Users can:

* Add marks for:

  * Mathematics
  * Java
  * Operating Systems
* View all marks
* Search marks using Student ID
* Calculate total marks
* Calculate percentage
* Automatically calculate grades

### 📅 Attendance Management

The system can:

* Add attendance records
* View attendance records
* Search attendance using Student ID
* Calculate attendance percentage
* Check whether a student meets the **75% attendance requirement**

### 📈 Performance Analysis

The system evaluates both **marks and attendance** to determine the student's overall performance.

Performance categories include:

| Marks        | Attendance   | Performance          |
| ------------ | ------------ | -------------------- |
| 80% or above | 75% or above | 🟢 Excellent         |
| 60% or above | 75% or above | 🔵 Good              |
| 50% or above | 60% or above | 🟡 Average           |
| Otherwise    | —            | 🔴 Needs Improvement |

The system also displays warnings when marks or attendance are below the required level.

---

## 📄 Student Performance Report

A complete performance report can be generated for an individual student.

The report contains:

* Student ID
* Student Name
* Course
* Mathematics Marks
* Java Marks
* Operating Systems Marks
* Total Marks
* Percentage
* Grade
* Attendance
* Attendance Status
* Overall Performance

Example:

```text
========================================
       STUDENT PERFORMANCE REPORT
========================================

Student ID      : 101
Student Name    : Rahul Sharma
Course          : CSE

------------- MARKS -------------------
Mathematics     : 85
Java            : 78
Operating Sys.  : 82

Total Marks     : 245
Percentage      : 81.67%
Grade           : A

------------- ATTENDANCE ---------------
Attendance      : 82%
Status          : Eligible

------------- PERFORMANCE -------------
Overall         : Excellent

========================================
```

---

## 🏆 Grading System

| Percentage | Grade  |
| ---------- | ------ |
| 90–100     | **A+** |
| 80–89      | **A**  |
| 70–79      | **B**  |
| 60–69      | **C**  |
| 50–59      | **D**  |
| Below 50   | **F**  |

---

## ✅ Input Validation

The application validates user input before storing or processing data.

Some validation rules include:

* Student ID must be greater than `0`
* Student name cannot be empty
* Course name cannot be empty
* Marks must be between `0` and `100`
* Total classes must be greater than `0`
* Attended classes cannot be greater than total classes
* A student must exist before marks or attendance can be added

This helps prevent incorrect or invalid data from being stored.

---

## 💾 Data Storage

The project uses **text files** for storing data.

The data is stored inside the:

```text
data/
```

folder.

This allows information to remain available even after the application is closed and restarted.

Example project structure:

```text
Student-Performance-Management-System/
│
├── data/
│   ├── students.txt
│   ├── marks.txt
│   └── attendance.txt
│
├── src/
│   └── ...
│
├── tests/
│   └── StudentTest.java
│
├── README.md
└── ...
```

---

## ⚙️ How the System Works

```text
             ┌──────────────────┐
             │   Start Program  │
             └────────┬─────────┘
                      ↓
             ┌──────────────────┐
             │   Display Menu   │
             └────────┬─────────┘
                      ↓
          ┌──────────────────────────┐
          │ Select Required Operation│
          └────────────┬─────────────┘
                       ↓
       ┌───────────────┼────────────────┐
       ↓               ↓                ↓
   Students          Marks          Attendance
       │               │                │
       └───────────────┼────────────────┘
                       ↓
              ┌─────────────────┐
              │ Input Validation│
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │ Save Data to    │
              │ Text Files      │
              └────────┬────────┘
                       ↓
              ┌─────────────────┐
              │ Generate Report │
              └─────────────────┘
```

---

## 🛠️ Technologies Used

* ☕ **Java**
* 🧩 **Object-Oriented Programming**
* 📁 **File Handling**
* 🧪 **Java Testing**
* 🌿 **Git & GitHub**
* 📄 **Text File Storage**

---

## 🧠 Java Concepts Used

This project demonstrates several fundamental Java concepts:

* Classes and Objects
* Encapsulation
* Constructors
* Methods
* ArrayLists / Collections
* Conditional Statements
* Loops
* Exception Handling
* File Handling
* BufferedReader
* BufferedWriter
* Input Validation
* Basic Unit Testing

---

## 🧪 Testing

A basic test program is included in:

```text
tests/StudentTest.java
```

The test verifies:

* Basic student information
* Student creation
* Student storage
* Searching for a student through the Student Manager

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Student-Performance-Management-System.git
```

### 2. Navigate to the Project

```bash
cd Student-Performance-Management-System
```

### 3. Compile the Project

Compile the Java source files using your preferred Java IDE or terminal.

Example:

```bash
javac src/*.java
```

### 4. Run the Program

```bash
java src.Main
```

> **Note:** The exact compile/run command may vary depending on your package structure and main class name.

---

## 📋 Main Menu

The application provides a menu-driven interface similar to:

```text
========================================
   STUDENT PERFORMANCE MANAGEMENT
========================================

1. Add Student
2. View All Students
3. Search Student
4. Update Student
5. Delete Student
6. Add Marks
7. View Marks
8. Search Marks
9. Add Attendance
10. View Attendance
11. Search Attendance
12. Performance Analysis
13. Generate Student Report
14. Exit

Enter your choice:
```

---

## 🎯 Objectives

The main objectives of this project are:

1. To manage student academic information efficiently.
2. To maintain marks and attendance records.
3. To automatically calculate percentage and grades.
4. To analyze student performance.
5. To generate individual performance reports.
6. To implement input validation.
7. To practice Java OOP concepts.
8. To understand Java file handling.
9. To store information permanently using text files.

---

## 🔮 Future Improvements

The project can be further improved by adding:

* 🖥️ Graphical User Interface (GUI)
* 🗄️ MySQL / database integration
* 🔐 User login and authentication
* 📊 Performance charts and graphs
* 📤 Export reports to PDF
* 📧 Email performance reports
* 👨‍🏫 Teacher/Admin accounts
* 🔎 Advanced student filtering and sorting

---

## 👨‍💻 Author

**Atharv Verma**

Java | OOP | File Handling | Git

---

## ⭐ Support

If you found this project useful, consider giving the repository a ⭐ on GitHub!

---

### 📌 Project Status

**Completed — Academic Project**

Made with ☕ Java and lots of debugging 😄

