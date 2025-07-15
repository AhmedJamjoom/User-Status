# User-Status

# 💻 PHP MySQL User Status Manager

A simple web-based application that enables users to submit their name and age, which is then stored in a MySQL database. Each user record includes a toggleable status (Active/Inactive), which can be updated directly from the interface.

---

## 🎯 Project Objectives

This project helps you learn how to:

- Build HTML forms for collecting user input  
- Store and manage data in a MySQL database using PHP  
- Display user records in a responsive table  
- Implement status toggling (Active/Inactive) with PHP  
- Perform basic CRUD operations (Insert, Update, Fetch)  

---

## 🧱 Project Overview

We developed a dynamic web interface using PHP connected to a MySQL database. The core functionalities include:

- Submitting a user's name and age  
- Viewing all submitted users in a table  
- Changing each user's status between Active and Inactive with a button  

The database schema was created using **phpMyAdmin**, and the structure is included in the `users_db.sql` file.

The project is built and tested using **XAMPP** as the local development environment.

---

## 📦 Included Files

- `index.php` → Main application file (form submission + data table)  
- `users_db.sql` → SQL script to set up the database structure  
- `README.md` → Project documentation  

---

## 🛠️ Tools & Technologies Used

- 🧠 PHP (Backend logic)  
- 🗃️ MySQL (Database)  
- 🖥️ HTML & CSS (Frontend)  
- ⚙️ XAMPP (Local server environment)  
- 🧑‍💻 Visual Studio Code (Code editor)  

---

## 🧪 How It Works

1. The user submits their name and age via a form.  
2. PHP script inserts this data into the `users` table.  
3. The table displays all users, including their current status.  
4. Status can be toggled between Active and Inactive with a button.  
5. Status is stored as:
   - `0` → Inactive  
   - `1` → Active  

---

## 🗃️ Database Schema (users_db.sql)

```sql
CREATE TABLE `users` (
  `ID` int NOT NULL AUTO_INCREMENT,
  `Name` varchar(100),
  `Age` int,
  `Status` tinyint DEFAULT 0,
  PRIMARY KEY (`ID`)
);
```

---

## 🚀 How to Run the Project Locally

1. Install [XAMPP](https://www.apachefriends.org/)  
2. Start **Apache** and **MySQL**  
3. Open **phpMyAdmin** and:
   - Create a database named `users_db`  
   - Import the `users_db.sql` file  
4. Copy the project folder into:  
   `C:\xampp\htdocs\users`  
5. Open your browser and go to:  
   `http://localhost/users/index.php`

---

## 👤 Author

Developed by: **Ahmed Jamjoom**  
Date: **15 July 2025**
