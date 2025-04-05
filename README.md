# 🏥 Lilavati Hospital Management System (Python SQL Project)

A fully normalized MySQL database system designed to manage all major hospital operations — including patients, doctors, appointments, admissions, billing, departments, and prescriptions.

> 📌 Built with a clear ER model and real-world use cases for hospitals.

---

## 📷 Entity-Relationship Diagram

> ER Diagram for the Lilavati Hospital system:

![leelavati](https://github.com/user-attachments/assets/bd8fa746-dadf-4be2-94fd-e77694b4a0ae)




---

## 🗃️ Database Tables

| Table Name        | Description                                      |
|-------------------|--------------------------------------------------|
| `Patient`         | Stores information about registered patients     |
| `Docter`          | Maintains records of hospital doctors            |
| `Appointment`     | Tracks patient appointments with doctors         |
| `Department`      | Defines the hospital's departments               |
| `Admission`       | Handles patient admission records                |
| `Billing_Counter` | Records billing and payment transactions         |
| `Subscription`    | Medical prescriptions and reports linked to billing |

---

## 📐 Table Definitions (Schema Overview)

### 📌 `Patient`
```sql
CREATE TABLE Patient (
    patient_id VARCHAR(10) PRIMARY KEY,
    patient_name VARCHAR(100),
    gender VARCHAR(10),
    dob DATE,
    address TEXT,
    contact VARCHAR(15)
);
