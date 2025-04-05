# 🏥 Lilavati Hospital Management System (Python SQL Project)

A fully normalized MySQL database system designed to manage all major hospital operations — including patients, doctors, appointments, admissions, billing, departments, and prescriptions.
---

> 📌 Built with a clear ER model and real-world use cases for hospitals.
---

## 📷 Entity-Relationship Diagram

> ER Diagram for the Lilavati Hospital system:

![leelavati](https://github.com/user-attachments/assets/bd8fa746-dadf-4be2-94fd-e77694b4a0ae)



## 🚀 Features

- **Realistic Data Generation**: Uses logic + Python's `random` and `datetime` libraries to generate authentic Indian names, phone numbers, DOBs, and addresses.
- **Relational Structure**: Implements foreign key relationships between tables like doctor, department, and billing.
- **SQL-Ready Scripts**: Automatically writes data to `.sql` files that can be directly imported into MySQL or MariaDB.
- **Extensible Design**: Modular code allows for adding more entities or updating schema easily.
- **Privacy-Safe Simulation**: Dummy data is purely fictional and does not resemble real individuals.

---

## 🧩 Entity Overview

| Entity         | Description                                       |
|----------------|---------------------------------------------------|
| `Patient`      | Includes name, gender, contact, DOB, address      |
| `Doctor`       | Specializations, contact info                     |
| `Nurse`        | Cute, Indian-themed fictional names               |
| `Department`   | Linked with billing and doctors                   |
| `Room`         | Patient room assignment info                      |
| `Billing`      | Tracks total, payment status, and date            |
| `Appointment`  | Arrival times, department, diagnosis              |
| `Subscription` | Medicine, report, doctor-bill relation            |

---

## 🛠️ How It Works

1. **Each generator script** produces SQL insert scripts for its corresponding entity.
2. Scripts can be run independently or chained together.
3. All `.sql` files are stored in `sql_scripts/` and ready for import.

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


## 💽 Requirements

- Python 3.7+
- MySQL / MariaDB
- (Optional) `faker` library for enhanced realism

To install dependencies:

```bash
pip install -r requirements.txt

git clone https://github.com/yourusername/lilavati-hospital-db.git
cd lilavati-hospital-db

python data_generators/patient_generator.py

SOURCE ./sql_scripts/lilavati_patient.sql;

Bhupesh

Software Developer @ Be10x

💼 Skilled in Python, React, SQL,Core Java

🧠 Prompt Engineer | Python Developer |

❤️ Support This Project
If this saved you time or helped you prepare for interviews or internships:

⭐ Star this repository

👥 Share with friends

👥


---

## ❤️ Need Full Code or Help?

You can **contact me** if you need the **complete codebase**, help in customizing it for your use case, or if you're looking to integrate it into a real project or academic assignment.

📧 **Email**: bhupesh.coding@gmail.com  
🐙 **GitHub**: [@bhupeshcoding](https://github.com/bhupeshcoding)  
💬 **LinkedIn**: [https://www.linkedin.com/in/bhupesh-joshi-/](https://www.linkedin.com/in/bhupesh-joshi-/)
🍕 Buy me a coffee (link if applicable)

> 💡 *Happy to help with full implementation, setup, or extending this project further!*

---



