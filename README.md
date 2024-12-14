PG Management System
Table of Contents
Introduction
Features
Installation
Configuration
Usage
Technologies Used
Testing
Conclusion
1. Introduction
The Virtual PG Management System is a web-based application designed to streamline the management of Paying Guest accommodations. The system provides features for both PG owners and tenants, facilitating efficient communication, booking management, payment processing, and more.

2. Features
User Authentication and Profile Management: Secure login for PG owners and tenants, profile management.
Property Management: PG owners can list, update, and remove properties.
Booking Management: Handles booking requests, approvals, rejections, and provides a calendar view for property availability.
Payment Management: Integrates with payment gateways for online transactions and manages reminders and failures.
Messaging System: Facilitates communication between PG owners and tenants.
Review and Rating System: Allows tenants to share feedback.
Admin Dashboard: Provides control over users, properties, bookings, payments, and access to analytics.
3. Installation
To run this project on your local machine using XAMPP, follow these steps:

Prerequisites
XAMPP installed on your machine.
A web browser.
Steps
Download and Install XAMPP: If you haven't already, download and install XAMPP from here.
Clone the Repository: Download or clone the project repository to your local machine.
Move Project to XAMPP's htdocs Directory:
Copy the project folder.
Paste it into the htdocs directory of your XAMPP installation. (e.g., C:\xampp\htdocs\PG_Management_System).
4. Configuration
Database Setup
Start XAMPP: Open the XAMPP control panel and start Apache and MySQL.
Create a Database:
Open a web browser and go to http://localhost/phpmyadmin.
Create a new database named pg_management.
Import Database:
Select the pg_management database.
Click on the Import tab.
Choose the SQL file provided in the database directory of the project and import it.
Update Database Configuration
Database Configuration:
Open the project folder and navigate to the config directory.
Edit the config.php file with your database credentials.
php
Copy code
<?php
define('DB_SERVER', 'localhost');
define('DB_USERNAME', 'root');
define('DB_PASSWORD', '');
define('DB_DATABASE', 'pg_management');
$db = mysqli_connect(DB_SERVER, DB_USERNAME, DB_PASSWORD, DB_DATABASE);
?>
5. Usage
Accessing the Application
Open a Web Browser: Go to http://localhost/PG_Management_System.
Login/Register: Use the login page to log in as a PG owner or tenant. New users can register.
Admin Dashboard
Manage Properties: Add, update, or delete property listings.
Manage Bookings: View and manage booking requests.
Payments: Monitor and manage payment transactions.
User Communication: Use the messaging system for communication between users.
6. Technologies Used
Frontend:
HTML, CSS, JavaScript
Backend:
PHP
Database:
MySQL
Tools:
XAMPP
7. Testing
Unit Testing
Verify individual components such as user authentication, database connections, and form submissions.
Integration Testing
Ensure different modules work together seamlessly, such as booking management and payment processing.
User Interface Testing
Test the responsiveness and usability of the interface across different devices and browsers.
8. Conclusion
The Virtual PG Management System simplifies the management of PG accommodations by providing a comprehensive platform with robust features. It enhances operational efficiency, improves communication, and ensures secure transactions, making it an invaluable tool for PG owners and tenants.

For any further assistance or queries, please refer to the project's documentation or contact the development team.
