👤 Personal Details Management (JDBC CRUD)

A simple Java JDBC console application to manage personal details using CRUD operations (Create, Read, Update, Delete).
This project connects to a MySQL database and allows users to store and manage personal information.

🚀 Features

✅ Add new person details
✅ View all records
✅ Update existing details
✅ Delete records
✅ MySQL database connectivity using JDBC
✅ Console-based menu system

🛠️ Tech Stack

Language: Java

Database: MySQL

Connectivity: JDBC

IDE (recommended): Eclipse / IntelliJ IDEA

Driver: MySQL Connector/J

📂 Project Structure
personaldetials/
│
├── src/main/java/crud/
│   └── person.java
│
├── src/main/webapp/
│   └── WEB-INF/
│       └── lib/
│           └── mysql-connector-j-9.6.0.jar
│
└── build/

⚙️ Setup Instructions
1️⃣ Create Database

Open MySQL and run:

CREATE DATABASE person_det;

2️⃣ Create Table
CREATE TABLE detials (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    email VARCHAR(100),
    phoneno BIGINT,
    address VARCHAR(255)
);

3️⃣ Update DB Credentials

In person.java, update if needed:

static final String URL ="jdbc:mysql://localhost:3306/person_det";
static final String username = "root";
static final String password = "YOUR_PASSWORD";

4️⃣ Add JDBC Driver

Make sure:

mysql-connector-j-9.6.0.jar


is added to your project libraries.

5️⃣ Run Program

Run person.java as a Java application.

▶️ How It Works

When the program runs, a menu appears:

1. Add
2. View
3. Update
4. Delete
5. Exit


User selects an option and enters details accordingly.

📌 Example Usage

Add Record

Name: Vijay
Email: vijay@gmail.com
Phone: 9876543210
Address: Chennai


View Records

Vijay | vijay@gmail.com | 9876543210 | Chennai

⚠️ Notes

Ensure MySQL server is running

Table name in code is detials (typo kept as-is)

Phone number stored as integer in code
