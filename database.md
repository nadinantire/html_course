# Database Fundamentals

## Course Overview

This course introduces the basic concepts of databases in a simple and practical way. By the end of this course, you will understand how data is stored, organized, and managed in a database. You will also learn how to use SQL to create, retrieve, update, and delete data.

---

# Learning Objectives

After completing this course, students will be able to:

- Explain what a database is.
- Differentiate between a database, table, row, and column.
- Understand the purpose of Primary Keys and Foreign Keys.
- Explain relationships between tables.
- Use SQL to insert, retrieve, update, and delete data.
- Search and filter data using SQL queries.
- Build a simple relational database using DB Browser for SQLite.

---

# 1. What is a Database?

A **database** is an organized collection of data that is stored electronically so it can be easily accessed, managed, and updated.

Think of a database as a digital filing cabinet where information is stored in an organized manner.

### Real-Life Examples

- School student records
- Hospital patient records
- Bank customer accounts
- Library book records
- Mobile phone contacts
- Online shopping websites

All these systems use databases to store and manage information.

---

# Why Do We Use Databases?

Imagine a school with 5,000 students.

If all student information were written on paper, finding one student's record would take a long time.

A database helps us:

- Store large amounts of information
- Find information quickly
- Update records easily
- Prevent duplicate information
- Keep data secure
- Share information between different users

---

# 2. What is a Table?

A **table** is a collection of related data.

Each table stores one type of information.

### Example

A school database may contain:

- Students Table
- Teachers Table
- Courses Table
- Departments Table

Example of a Students table:

| Student ID | Name | Age | Class |
|------------|------|-----|-------|
| 1 | Alice | 18 | S6 |
| 2 | John | 17 | S5 |
| 3 | Peter | 19 | S6 |

---

# 3. What is a Row?

A **row** (also called a **record**) represents one complete item of information.

Example:

| Student ID | Name | Age |
|------------|------|-----|
| 1 | Alice | 18 |

This entire line is **one row** because it contains all the information about one student.

---

# 4. What is a Column?

A **column** (also called a **field**) represents one type of information.

Example:

| Student ID | Name | Age |
|------------|------|-----|

The columns are:

- Student ID
- Name
- Age

Each column stores one specific type of data.

---

# Database Structure

```
Database
│
├── Students Table
│      ├── Student ID
│      ├── Name
│      ├── Age
│      └── Class
│
├── Teachers Table
│
└── Courses Table
```

---

# Example of a Students Table

| Student ID | Name | Age | Gender |
|------------|------|-----|--------|
| 1 | Alice | 18 | Female |
| 2 | John | 17 | Male |
| 3 | Peter | 19 | Male |
| 4 | Grace | 18 | Female |

---

# 5. Introduction to SQL

**SQL** stands for **Structured Query Language**.

It is the language used to communicate with a database.

SQL allows us to:

- Create databases
- Create tables
- Store data
- Retrieve data
- Update data
- Delete data

Think of SQL as the language you use to "talk" to a database.

---

# Basic SQL Commands

## SELECT

The **SELECT** statement retrieves data from a table.

Example:

```sql
SELECT * FROM students;
```

Output:

Returns all records from the Students table.

---

## INSERT

The **INSERT** statement adds new records into a table.

Example:

```sql
INSERT INTO students(name, age)
VALUES ('Alice', 18);
```

Result:

A new student is added to the table.

---

## UPDATE

The **UPDATE** statement changes existing information.

Example:

```sql
UPDATE students
SET age = 19
WHERE id = 1;
```

Result:

Alice's age becomes 19.

---

## DELETE

The **DELETE** statement removes records.

Example:

```sql
DELETE FROM students
WHERE id = 1;
```

Result:

Alice's record is removed.

---

# CRUD Operations

The four basic database operations are called **CRUD**.

| Operation | SQL Command | Meaning |
|-----------|-------------|---------|
| Create | INSERT | Add new data |
| Read | SELECT | View data |
| Update | UPDATE | Modify existing data |
| Delete | DELETE | Remove data |

---

# 6. Primary Key

A **Primary Key** is a column that uniquely identifies each row in a table.

Every table should have a Primary Key.

Example:

| Student ID | Name |
|------------|------|
| 1 | Alice |
| 2 | John |
| 3 | Peter |

Student ID is the Primary Key because:

- No two students have the same ID.
- IDs cannot be empty.
- IDs uniquely identify each student.

---

# Characteristics of a Primary Key

- Must be unique.
- Cannot contain NULL values.
- Each table should have only one Primary Key.

---

# 7. Foreign Key

A **Foreign Key** is a column that connects one table to another.

It references the Primary Key of another table.

Example:

Students Table

| Student ID | Name |
|------------|------|
| 1 | Alice |
| 2 | John |

Courses Table

| Course ID | Course Name |
|-----------|-------------|
| 1 | Mathematics |
| 2 | English |

Enrollment Table

| Student ID | Course ID |
|------------|-----------|
| 1 | 1 |
| 1 | 2 |
| 2 | 2 |

Student ID and Course ID in the Enrollment table are Foreign Keys because they refer to records in other tables.

---

# Why Do We Use Foreign Keys?

Foreign Keys help us:

- Connect related tables
- Avoid duplicate information
- Maintain data consistency
- Improve database organization

---

# 8. Database Relationships

A **relationship** is a connection between two or more tables.

Instead of storing everything in one large table, databases separate information into different tables and connect them using keys.

Example:

Students

| Student ID | Name |
|------------|------|
| 1 | Alice |
| 2 | John |

Courses

| Course ID | Course |
|-----------|---------|
| 1 | HTML |
| 2 | CSS |

Enrollment

| Student ID | Course ID |
|------------|-----------|
| 1 | 1 |
| 1 | 2 |
| 2 | 2 |

This shows:

- Alice studies HTML and CSS.
- John studies CSS.

---

# Types of Relationships

## One-to-One (1:1)

One record in Table A matches one record in Table B.

Example:

- Person → Passport

---

## One-to-Many (1:N)

One record in Table A matches many records in Table B.

Example:

- One teacher teaches many students.
- One department has many employees.

This is the most common relationship.

---

## Many-to-Many (M:N)

Many records in one table are related to many records in another table.

Example:

- Students enroll in many courses.
- Courses have many students.

This relationship requires a third table (called a junction table or bridge table), such as the Enrollment table.

---

# 9. Querying Data

Querying means asking the database to return specific information.

---

## View All Students

```sql
SELECT * FROM students;
```

---

## View Only Student Names

```sql
SELECT name FROM students;
```

---

## Find Students Who Are 18 Years Old

```sql
SELECT *
FROM students
WHERE age = 18;
```

---

## Find Female Students

```sql
SELECT *
FROM students
WHERE gender = 'Female';
```

---

## Sort Students by Name

```sql
SELECT *
FROM students
ORDER BY name;
```

---

## Count Students

```sql
SELECT COUNT(*)
FROM students;
```

---

# Summary

In this course, you learned:

- What a database is
- What a table is
- What rows and columns are
- How SQL is used to communicate with databases
- The four CRUD operations
- Primary Keys
- Foreign Keys
- Database relationships
- How to retrieve and filter information using SQL

These concepts form the foundation of relational databases and are essential before learning advanced SQL topics such as joins, grouping, indexing, and database design.

---

# Practical Exercises

1. Create a database called **SchoolDB**.
2. Create a **Students** table.
3. Insert at least five student records.
4. Display all student records.
5. Display only student names.
6. Update one student's age.
7. Delete one student record.
8. Create a **Courses** table.
9. Create an **Enrollment** table.
10. Connect the tables using Primary Keys and Foreign Keys.
11. Display students who are older than 18 years.
12. Sort students alphabetically by name.

Congratulations! You have completed the **Database Fundamentals** course.
