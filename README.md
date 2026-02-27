# 💇 Salon Appointment Scheduler

A command-line salon booking system built using **Bash** and **PostgreSQL** as part of the freeCodeCamp Relational Database certification.

The application allows users to select salon services, register as customers, and schedule appointments — all through a terminal interface.

---

## 🚀 Features

* Service selection menu
* Customer lookup using phone number
* Automatic new customer registration
* Appointment scheduling
* Relational database design with foreign keys
* Input validation and retry flow

---

## 🧱 Tech Stack

* Bash scripting
* PostgreSQL
* psql CLI
* Relational database design

---

## 🗄️ Database Schema

### Customers

* customer_id (PK)
* name
* phone (unique)

### Services

* service_id (PK)
* name

### Appointments

* appointment_id (PK)
* customer_id (FK)
* service_id (FK)
* time

---

## ⚙️ How to Run

### 1. Clone the repo

```bash
git clone <repo-url>
cd salon-appointment-scheduler
```

### 2. Create database

```bash
psql --username=freecodecamp --dbname=postgres
CREATE DATABASE salon;
\c salon
```

Run the schema SQL (or recreate tables manually).

---

### 3. Make script executable

```bash
chmod +x salon.sh
```

### 4. Run

```bash
./salon.sh
```

---

## 🧠 Learning Outcomes

* Bash scripting for real applications
* Database normalization and relationships
* Using psql inside scripts
* Handling user input and validation
* Building CLI products end-to-end

---

## 📌 Example Flow

* User selects a service
* System checks customer by phone
* Registers customer if new
* Books appointment
* Confirms booking

---

## 📜 License

This project is for educational and portfolio purposes.
