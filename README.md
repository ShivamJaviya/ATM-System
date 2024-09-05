# 💳 ATM System

This **ATM System** project is built in Java, utilizing a **User Interface**, **MySQL Database**, **Multithreading**, and **Object-Oriented Programming** concepts. The system mimics basic ATM functionalities, including user sign-up, login, and transactions.

## 🗂 Features
- 🖥️ **User Interface**: Interactive UI for easy navigation.
- 🗄️ **Database Management**: Stores user details and transactions securely using MySQL.
- 🧵 **Multithreading**: Ensures smooth execution of simultaneous user operations.
- 🧑‍💻 **OOP Concepts**: Applied OOP principles for better system structure.

## 🏦 Database Structure

```sql
-- Create Database
CREATE DATABASE bankSystem;
USE bankSystem;

-- Table for user sign-up details
CREATE TABLE signup(
    form_no VARCHAR(30),
    name VARCHAR(30),
    father_name VARCHAR(30),
    DOB VARCHAR(30),
    gender VARCHAR(30),
    email VARCHAR(60),
    marital_status VARCHAR(30),
    address VARCHAR(60),
    city VARCHAR(60),
    pincode VARCHAR(60),
    state VARCHAR(60)
);
SELECT * FROM signup;

-- Table for additional user information
CREATE TABLE signuptwo(
    form_no VARCHAR(30),
    religion VARCHAR(30),
    category VARCHAR(30),
    income VARCHAR(30),
    education VARCHAR(30),
    occcupation VARCHAR(60),
    pan VARCHAR(30),
    aadhar VARCHAR(60),
    seniorcitizen VARCHAR(60),
    existing_account VARCHAR(60)
);
SELECT * FROM signuptwo;

-- Table for account and card details
CREATE TABLE signupthree(
    form_no VARCHAR(30),
    account_Type VARCHAR(30),
    card_number VARCHAR(30),
    pin VARCHAR(30),
    facility VARCHAR(300)
);
SELECT * FROM signupthree;

-- Table for login information
CREATE TABLE login(
    form_no VARCHAR(30),
    card_number VARCHAR(30),
    pin VARCHAR(30)
);
SELECT * FROM login;

-- Table for banking transactions
CREATE TABLE bank(
    pin VARCHAR(30),
    date VARCHAR(30),
    type VARCHAR(30),
    amount VARCHAR(30)
);
SELECT * FROM bank;
