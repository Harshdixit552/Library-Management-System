 Library Management System
A desktop-based Library Management System built with Java Swing for the GUI, NetBeans as the IDE, and MySQL for the backend database. This application streamlines library operations such as managing books, members, and issuing/returning books.

🚀 Features
User Authentication: Secure login system for administrators.

Book Management: Add, update, delete, and search for books.

Member Management: Manage library members, including students and staff.

Issue & Return Books: Handle the issuance and return of books with due date tracking.

Fine Calculation: Automatically calculate fines for overdue books.

Search Functionality: Search books by title, author, or category.

Reports: Generate reports on issued books, returned books, and overdue items.

🛠️ Technologies Used
Programming Language: Java

GUI Framework: Java Swing

Database: MySQL

IDE: NetBeans

Database Connector: MySQL Connector/J
GitHub

📂 Project Structure
pgsql
Copy
Edit

LibraryManagementSystem/
├── src/
│   └── library/
│       ├── Main.java
│       ├── Login.java
│       ├── Dashboard.java
│       ├── BookManagement.java
│       ├── MemberManagement.java
│       ├── IssueReturn.java
│       └── DBConnection.java
├── lib/
│   └── mysql-connector-java-8.0.xx.jar
├── database/
│   └── library.sql
├── README.md
└── LICENSE
⚙️ Setup Instructions
Clone the Repository

bash
Copy
Edit
git clone https://github.com/Harshdixit552/Library-Management-System
Import Project into NetBeans

Open NetBeans.

Click on File > Open Project.

Navigate to the cloned repository and open it.

Set Up the Database

Open MySQL Workbench or any MySQL client.

Create a new database:

sql
Copy
Edit
CREATE DATABASE library;
Import the library.sql file located in the database/ directory to set up the necessary tables.

Configure Database Connection

Open the DBConnection.java file.

Update the database URL, username, and password as per your MySQL configuration.

java
Copy
Edit
private static final String URL = "jdbc:mysql://localhost:3306/library";
private static final String USER = "yourusername";
private static final String PASSWORD = "yourpassword";
Add MySQL Connector/J to the Project

Download the MySQL Connector/J from the official website.

Place the mysql-connector-java-8.0.xx.jar file into the lib/ directory.

In NetBeans:

Right-click on the project > Properties.

Go to Libraries > Add JAR/Folder.

Navigate to the lib/ directory and select the JAR file.

Build and Run the Project

Press F6 or click on Run > Run Project.
