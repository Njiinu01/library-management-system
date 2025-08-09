# library-management-system
The Library Management System is a relational database designed to efficiently manage the operations of a library.
It stores and organizes data related to books, members, authors, categories, loans, and librarians, while enforcing data integrity through primary keys, foreign keys, and other SQL constraints.

This project demonstrates:

Relational database design.

Use of Primary Key (PK), Foreign Key (FK), NOT NULL, UNIQUE, and other constraints.

Implementation of One-to-One, One-to-Many, and Many-to-Many relationships in SQL.

Use of SQL CREATE TABLE statements to define the schema.

Use Case
Libraries often need a reliable way to:

Store book information.

Track borrowing and returning of books.

Manage member records.

Keep track of librarian activities.

This database design provides a structured, scalable solution for these needs.

Key Features
Books Management – Stores details of books including title, author, category, and ISBN.

Members Management – Records library members’ personal and contact information.

Loans Tracking – Tracks borrowing and return dates for each book.

Authors & Categories – Organizes books by their authors and subject categories.

Librarians Table – Maintains librarian details for accountability and system administration.

Data Integrity – Uses foreign keys and constraints to maintain consistency.

Database Relationships
One-to-Many – A member can borrow many books, but each loan record belongs to one member.

Many-to-Many – A book can have multiple authors, and an author can write multiple books.

One-to-One – Some optional profile extensions could be linked uniquely to a member or book.

Technologies Used
MySQL – Database management system.

SQL – Data definition and manipulation.

Installation & Usage
Install MySQL on your system.

Import the provided library_db.sql file into your MySQL server:

bash
Copy code
mysql -u root -p library_db < library_db.sql
The database will be created with all required tables and constraints.

Possible Extensions
Adding stored procedures for automated book status updates.

Implementing triggers for overdue book notifications.

Creating views for frequently borrowed books.
