# Relational Database Design: Student & Employee Records

## Overview
This project involved designing a normalized relational database schema for managing student and employee records, as part of Columbia University's COMS W4111 (Introduction to Databases) course. The focus was on applying core relational database principles, including normalization, atomicity, and update anomalies, while building stored procedures to handle common data operations safely and reliably.

## Schema Design
- Designed separate, normalized tables for student and employee records, avoiding data redundancy and ensuring each piece of information is stored in exactly one place
- Applied principles of atomicity (ensuring fields hold single, indivisible values) and addressed update anomalies that arise when data is duplicated across rows or improperly structured
- Considered which views over the schema would be theoretically updatable versus not, based on relational database theory (Codd's rules)

## Stored Procedures
- Built stored procedures (`create_student`, `update_student`, `create_employee`, `update_employee`) to handle record creation and updates directly within the database
- Enforced data constraints to prevent duplicate entries (e.g., unique ID generation) and invalid inputs (e.g., rejecting invalid employee type values)
- Tested each procedure against edge cases, including attempts to insert invalid or duplicate data, to confirm constraints behaved as intended

## Key Concepts Applied
- Relational schema normalization
- Atomicity and non-atomic data problems (e.g., composite identifier strings)
- Update anomalies and theoretically updatable views
- Stored procedures vs. database functions vs. triggers
- Data integrity constraints and validation

## Tools
SQL, MySQL

## Files
- `Employees-Analysis.ipynb` — full assignment notebook, including written theory questions, schema design, and tested stored procedures
