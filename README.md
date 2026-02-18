# Smart Clinic Management System - Database

## Experiment Information
Course: Database Systems Lab (CIT 350L)  
Experiment: #9  
Title: Smart Clinic Management System (SCMS)

---

## Overview

This project presents the design and implementation of a Smart Clinic Management System database.

The system manages:

- Patients
- Doctors
- Appointments
- Medical Records
- Prescriptions
- Billing

The database design includes ER modeling, relational schema conversion, normalization (3NF / BCNF), and SQL implementation.

---

## System Entities

1. PATIENT
2. DOCTOR
3. APPOINTMENT
4. MEDICAL_RECORD
5. PRESCRIPTION
6. BILL

---

## Relationships

- One Patient can have many Appointments (1:M)
- One Doctor can have many Appointments (1:M)
- One Appointment generates at most one Medical Record (1:1)
- One Medical Record can have many Prescriptions (1:M)
- Each Appointment has exactly one Bill (1:1)

---

## Project Structure

Smart-Clinic-Management-System-Database
│
├── README.md
├── ERD.png
├── schema/
│   └── create_tables.sql
│
├── data/
│   └── insert_sample_data.sql
│
├── queries/
│   ├── select_queries.sql
│   ├── update_delete.sql
│
└── docs/
    └── normalization_and_fd.md

---

## Database Design

The database was designed using ER modeling and converted into a relational schema.

All tables include:

- Primary Keys
- Foreign Keys
- Proper cardinalities
- Business rules constraints

---

## Normalization

All relations satisfy:

- Third Normal Form (3NF)
- Boyce-Codd Normal Form (BCNF)

There are no partial or transitive dependencies.

---

## SQL Implementation

The project includes:

- DDL (CREATE TABLE statements)
- DML (INSERT sample data)
- SELECT queries (joins, subqueries, aggregation)
- UPDATE and DELETE commands

---
