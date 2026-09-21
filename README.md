# 📚 Library Management System

<p align="center">
  <img src="https://img.shields.io/badge/Project-Library%20Management%20System-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Database-SQL-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

<p align="center">
  <b>📖 A simple and efficient database system for managing books, students, issues, returns and fines.</b>
</p>

---

## 🌟 About The Project

Managing a library manually can be time-consuming.

This project provides a **database-driven Library Management System** that helps organize library records and makes common operations faster and easier.

> 🎯 **Goal:** Build a practical SQL project while learning database design, queries and CRUD operations.

---

## ✨ Features

| Feature                  | Description                          |
| ------------------------ | ------------------------------------ |
| 📚 Book Management       | Add, update, search and delete books |
| 👨‍🎓 Student Management | Store and manage student information |
| 📤 Issue Books           | Record issued books                  |
| 📥 Return Books          | Track returned books                 |
| 💰 Fine Management       | Manage overdue fines                 |
| 🔎 Search                | Quickly find books and records       |
| 🗃️ Database             | Organized relational database        |

---

## 🛠️ Tech Stack

<p align="center">

<img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Database-Management-6C63FF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/CRUD-Operations-00A67E?style=for-the-badge"/>

</p>

---

## 🗄️ Database Structure

```text
                 📚 LIBRARY DATABASE
                        │
        ┌───────────────┼───────────────┐
        │               │               │
     📖 Books        👨‍🎓 Students    📤 Issue_Return
        │               │               │
        └───────────────┼───────────────┘
                        │
                    💰 Fines
```

### 📖 Books

```text
Book_ID
Book_Name
Author
Category
Quantity
```

### 👨‍🎓 Students

```text
Student_ID
Student_Name
Phone
```

### 📤 Issue & Return

```text
Issue_ID
Book_ID
Student_ID
Issue_Date
Return_Date
```

---

## 💻 SQL Examples

### 🔍 Search Books

```sql
SELECT *
FROM Books
WHERE Book_Name LIKE '%Java%';
```

### 📚 Available Books

```sql
SELECT Book_Name, Quantity
FROM Books
WHERE Quantity > 0;
```

### ➕ Add a New Book

```sql
INSERT INTO Books
(Book_ID, Book_Name, Author, Category, Quantity)
VALUES
(101, 'Java Programming', 'James Gosling', 'Programming', 5);
```

### ✏️ Update Quantity

```sql
UPDATE Books
SET Quantity = Quantity + 1
WHERE Book_ID = 101;
```

---

## 📊 What I Learned

Through this project, I practiced:

* 🧠 Database design
* 🔗 Relationships between tables
* 🔍 SQL queries
* ➕ INSERT operations
* 📖 SELECT operations
* ✏️ UPDATE operations
* 🗑️ DELETE operations
* 🔄 CRUD operations
* 🗃️ Data organization

---

## 🚀 Future Improvements

🔹 Add a login system
🔹 Add a graphical interface
🔹 Automatic fine calculation
🔹 Advanced search & filtering
🔹 Dashboard with library statistics
🔹 User authentication

---

## 👩‍💻 Author

### **Lovepreet Kaur**

🎓 BCA Graduate
💻 Aspiring Software Developer
📍 India

<p align="center">

<a href="https://github.com/YOUR_USERNAME">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</p>

---

<p align="center">

### ⭐ Thanks for visiting this project!

**Made with 💻 + ☕ + SQL**

</p>
