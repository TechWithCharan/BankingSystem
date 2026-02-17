# 🏦 Banking System (Java + MySQL)

## 📌 Project Overview

The Banking System is a simple **console-based application** developed using **Java** and **MySQL** that simulates basic real-world banking operations.
Users can securely **register, log in, create bank accounts, and perform transactions** such as deposit, withdrawal, and balance inquiry.
The project demonstrates how Java applications connect to databases using **JDBC** for reliable and permanent data storage.

---

## ✨ Key Features

* Secure user registration and login
* Bank account creation with unique account number
* Deposit and withdrawal functionality
* Balance checking system
* Persistent data storage using MySQL
* Menu-driven console interface

---

## 🛠️ Technologies Used

* **Java** – Core programming and OOP concepts
* **MySQL** – Relational database management
* **JDBC** – Java database connectivity
* **CLI (Command Line Interface)** – User interaction

---

## 🗄️ Database Schema

### User Table

Stores login credentials of registered users.

```sql
CREATE TABLE user(
    full_name VARCHAR(255),
    email VARCHAR(255) PRIMARY KEY,
    password VARCHAR(255)
);
```

### Accounts Table

Stores bank account details and balance information.

```sql
CREATE TABLE accounts(
    account_number BIGINT PRIMARY KEY,
    full_name VARCHAR(255),
    email VARCHAR(255) UNIQUE,
    balance DECIMAL(10,2),
    security_pin CHAR(4)
);
```

---

## 📂 Project Structure

```
BankingSystem/
│── BankingApp.java
│── AccountManager.java
│── Accounts.java
│── User.java
│── README.md
```

---

## 🎯 Learning Outcomes

This project helps in understanding:

* Java **Object-Oriented Programming (OOP)** concepts
* **JDBC integration** with MySQL database
* Writing and executing **SQL queries**
* Designing a **menu-driven console application**
* Basic structure of real-world banking software

---

## 👨‍💻 Author

**Charan Sai**

---

## 📖 Academic Purpose

This project is created as a **beginner-level mini project** for learning Java-MySQL integration and demonstrating practical database-driven application development.
