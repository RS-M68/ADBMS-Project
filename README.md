# University Management Application

A role-based University Management System built as part of my Advanced Database Management Systems (ADBMS) master’s project. The system manages core university workflows such as student onboarding, course enrollment, and admin operations with secure authentication and database-backed business rules.

## Why this project exists

Universities deal with highly relational data (students ↔ courses ↔ departments ↔ enrollments ↔ grades). This project demonstrates:
1.Designing a normalized schema
2.Implementing transactional workflows (enrollment, updates, deletes)
3.Enforcing data integrity with database constraints
4.Building a usable app layer on top of an ADBMS-designed backend

## Features
Admin
Create/update/delete students
Manage courses and departments
View enrollments and student records

Student
View available courses
Enroll / drop courses
View profile / academic details

## Database Design
This project was designed with core ADBMS principles:
Normalization: Schema normalized up to [3NF/BCNF]
Relationships: One-to-many and many-to-many using junction tables (example: Enrollments)
Integrity Rules: Primary keys, foreign keys, NOT NULL, UNIQUE constraints
Transactions: Enrollment operations handled atomically to prevent partial writes
Indexing: Indexes added on frequently queried columns (e.g., email, courseId, studentId)
Queries/Reports: example: student course history, admin analytics, department-wise enrollments


# Getting Started
Installation
npm install
npm run dev

## Credentials

### Admin

- Email: manager@ucmo.edu
- Password: password

### Student

- Email: student@ucmo.edu
- Password: password

## Project Structure
/src
  /components
  /pages
  /services
/server (if applicable)
  /routes
  /controllers
  /models
/db
  schema.sql
  seed.sql
/docs
  ERD.png
  assumptions.md



