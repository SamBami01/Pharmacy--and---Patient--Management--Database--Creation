# Pharmacy-Patient-Management-Database

## Overview
This project is a relational database system for managing pharmacy operations, patient records, prescriptions, and medication inventory.

## Technologies Used
- MySQL Workbench
- SQL

## Features
- Patient and Doctor management.
- Prescription history tracking.
- Medication inventory system.

## ER Diagram
![ER DIAGRAM](https://github.com/user-attachments/assets/9c8d59f8-5969-490d-8a93-73f53e0256a6)

## Defining Relationships
#### Drugstore to Drug
A drugstore sells several drugs. A drug can be sold at multiple drugstores.

Relationship: Sells (Many-to-Many)

#### Patient to Doctor
Every patient has a primary doctor, and every doctor has at least one patient.

Relationship: Has (One-to-Many)

#### Doctor to Prescription
Doctors prescribe drugs for patients. A doctor can prescribe multiple drugs for multiple patients.

Relationship: Prescribes (Many-to-Many)

#### Patient to Prescription
A patient can have prescriptions from multiple doctors.

Relationship: Obtains (One-to-Many)

#### Drugstore to Pharmaceutical Company
Pharmaceutical companies have contracts with drugstores. A company can contract with multiple drugstores and vice versa.

Relationship: Contracts (Many-to-Many)

#### Contract to Supervisor
Each contract has a supervisor. The supervisor can change over time.

Relationship: Managed By (One-to-Many)
