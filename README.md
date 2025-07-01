# 🏥 ASHA Worker Health Record Management System

> *Database Management System Project — Principles of Database Management (DBMS)*

This project is a *database-driven solution* designed to help *ASHA (Accredited Social Health Activist) workers* efficiently manage healthcare records in rural India. The system digitizes crucial health data including vaccination records, pregnancies, chronic illnesses, and medicine distribution, replacing traditional handwritten records.

> ✅ This project was developed as part of our DBMS coursework.

---

## 📚 About the Project

- 🌍 *Purpose:* To create a structured, normalized database for managing community health records.
- 🩺 *Goal:* Empower ASHA workers with an efficient tool for tracking:
  - Immunizations
  - Pregnancy and newborn records
  - Chronic diseases
  - Medicine distribution
  - Mortality data
- 🔗 Supports better decision-making and health service delivery at the village level.

---

## ⚙ Features

- 👨‍👩‍👧‍👦 Manage households and family members
- 📅 Track village visits by ASHA workers
- 🤰 Monitor pregnancies and newborn health
- 💉 Immunization tracking based on age eligibility
- 💊 Medicine distribution recording
- ❤ Chronic disease management
- ⚰ Mortality tracking
- 🔗 Fully normalized relational database schema

---

## 🗂 Database Entities

- Village
- Asha
- Family
- Person
- VillageVisitRecord
- PregnancyRecord
- NewBornRecord
- DeathRecord
- Disease
- ChronicDiseaseRecord
- Vaccine
- ImmunizationRecord
- Tablet
- MedicineDistributionRecord

---

## 🔗 Entity Relationship (ER) Highlights

- *One-to-One:* Asha ↔ Village, Asha ↔ Person
- *One-to-Many:* Village ↔ Family, Family ↔ Person
- *Parent-Child Links:* Person ↔ Person (FatherID, MotherID)
- *Health Records:* Person ↔ Immunization, Chronic Diseases, Medicine Distribution, and Death Records
- *Pregnancy to Newborn Relationship:* PregnancyRecord ↔ NewBornRecord ↔ Person

---

## 🛠 Technologies Used

- *Database:* MySQL  
- *Query Language:* SQL (DDL, DML)  
- *Design Tools:* dbdiagram.io (Relation Schema) , draw.io (ER Diagram)
- *Environment:* MySQL Workbench, XAMPP (optional)  

---

## 🏗 Functionalities Implemented

- ✅ Table creation with primary keys and foreign key constraints  
- ✅ Insertions with sample data  
- ✅ Triggers:  
  - For automatic creation of Person entries when a NewBornRecord is added  
  - For updating IsDeceased in Person upon a death entry  
- ✅ Normalization (up to 3NF)  
- ✅ Functional dependencies identified for all tables  

---

## 🗺 Entity-Relationship Diagram

(Add ER diagram image if available — Recommended)  
Or view the live ER diagram at: [dbdiagram.io](https://dbdiagram.io) (if link is published)

---

## 🚀 How to Run

1. Install MySQL Server / XAMPP / WAMP.
2. Create a new database (e.g., asha_health_db).
3. Run the provided SQL script (schema.sql or create_tables.sql) to create tables.
4. Insert sample data using insert_data.sql.
5. Run queries for reports or insights.

---

## 👨‍💻 Authors

- *Rishith Thommandru* — [LinkedIn](https://www.linkedin.com/in/rishith-thommandru-10a364355)  
- *Vyshnav Reddy Pinreddy* - [LinkedIn](www.linkedin.com/in/pinreddy-vyshnav-reddy-084277310)

---

## 📜 License

This project is for *educational purposes only* as part of the *Database Management Systems (DBMS) course.*  
© 2024 Rishith Thommandru & Vyshnav Reddy Pinreddy. All rights reserved.

---
