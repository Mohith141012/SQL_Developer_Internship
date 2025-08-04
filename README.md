# SQL_Developer_Internship_Task_1

# 📚 Library Management System - Database Schema

##  Objective

This project sets up a relational database schema for a **Library Management System** using SQL. The goal is to define entities, relationships, and constraints that allow for managing books, members, authors, borrowing, and staff activities.

---

## 🛠️ Tool Used

- MySQL Workbench

---

## 🧱 Schema Overview

### Entities & Fields:

1. **Authors**
   - `author_id` (PK)
   - `name`
   - `country`

2. **Books**
   - `book_id` (PK)
   - `title`
   - `genre`
   - `publication_year`

3. **Members**
   - `member_id` (PK)
   - `name`
   - `email`
   - `membership_date`

4. **Staff**
   - `staff_id` (PK)
   - `name`
   - `role`

5. **Borrow**
   - `borrow_id` (PK)
   - `member_id` (FK)
   - `book_id` (FK)
   - `staff_id` (FK)
   - `borrow_date`
   - `return_date`

6. **BookAuthor**
   - `book_id` (FK)
   - `author_id` (FK)
   - Composite Primary Key (`book_id`, `author_id`)

---

## 🔗 Relationships

- A **book** can have multiple **authors**, and an **author** can write multiple **books** → Many-to-Many (`BookAuthor`)
- A **member** can borrow multiple **books**, and each **borrow** record is handled by **staff**.
- Borrowing activity is tracked in the **Borrow** table, capturing issue and return dates.

---

## 📌 Notes

- All foreign keys are properly defined.
- Composite key used in the `BookAuthor` table to manage many-to-many relationships.
- You can insert sample data for testing borrow records, book-author mapping, etc.


*This project is part of a database schema design task focused on practical ER modeling and SQL implementation.*
