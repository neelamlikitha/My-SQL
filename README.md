# 🗄️ Python MySQL DBMS Project – School Database

This project demonstrates how to build and manage a **relational database system** using **Python** and **MySQL**. It covers database creation, table management, CRUD operations, and SQL joins through a structured Python program.

---

## 📌 Project Overview

The application manages a simple **School Database (SchoolDB)** with two related tables:

- **Students**
- **Classes**

It showcases:
- Database connection handling
- Table creation with foreign key constraints
- Inserting sample data
- Displaying records using JOIN queries
- Updating and deleting records safely

---

## 🛠️ Technologies Used

- **Python 3**
- **MySQL**
- **mysql-connector-python**

---

## 📂 Database Schema

### 🧑‍🎓 Students Table
| Column | Type |
|------|------|
| id | INT (Primary Key, Auto Increment) |
| name | VARCHAR(100) |
| age | INT |
| grade | VARCHAR(10) |

---

### 📚 Classes Table
| Column | Type |
|------|------|
| class_id | INT (Primary Key, Auto Increment) |
| student_id | INT (Foreign Key → Students.id) |
| subject | VARCHAR(50) |
| score | INT |

---

## ⚙️ Features Implemented

- ✅ MySQL server connection with error handling
- ✅ Automatic database creation (`SchoolDB`)
- ✅ Table creation with constraints
- ✅ Data insertion using `executemany()`
- ✅ JOIN queries for relational data
- ✅ Safe update and delete operations
- ✅ Auto-increment reset using TRUNCATE
- ✅ Clean console output for clarity

---

## ▶️ How to Run the Project

### 1️⃣ Install Dependencies
```bash
pip install mysql-connector-python
2️⃣ Configure Database Credentials
Update the following lines in the script:

python
Copy code
create_connection("localhost", "root", "YOUR_PASSWORD")
3️⃣ Run the Script
bash
Copy code
python main.py
📊 Sample Output
Displays all students

Displays student scores using JOIN

Updates a student grade

Deletes a student and related class records

Shows updated database state

🔐 Database Operations Covered
CREATE DATABASE

CREATE TABLE

INSERT

SELECT

JOIN

UPDATE

DELETE

FOREIGN KEY handling

🚀 Use Cases
DBMS academic projects

Python–MySQL integration learning

CRUD operation demonstrations

Backend database logic practice

📌 Future Improvements
Add exception handling for SQL queries

Implement user input instead of hardcoded data

Add logging instead of print statements

Convert to OOP-based architecture

🤝 Contributing
Feel free to fork this repository and submit pull requests for improvements or enhancements.

📄 License
This project is licensed under the MIT License.

🙌 Author
NARALA GURULOHITHA
Python Developer | Database Enthusiast

📧 Email: naralagurulohitha@gmail.com
🔗 GitHub: https://github.com/gurulohithanarala
