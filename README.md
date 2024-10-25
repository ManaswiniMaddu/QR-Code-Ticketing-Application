# QR-Code-Ticketing-Application
This distributed application leverages MariaDB, XAMPP, and RESTful APIs to generate and manage over 100,000 distinct QR codes for event ticketing. It includes a comprehensive suite of features for event organization, seat reservation, pricing management, and the issuance of unique QR-coded tickets.

# Introduction
The QR Code Ticketing system utilizes MariaDB, an open-source relational database management system, along with RESTful services. This project includes an admin interface for scheduling events, reserving seats, setting prices, and generating tickets with unique QR codes. Data is pulled from the database and displayed using RESTful APIs on various pages including the dashboard, event page, and seat preference page.

# Tech Stack
Front-End: HTML, CSS, Bootstrap
Back-End: PHP
Database: MariaDB
Web Server: Apache (via XAMPP)
QR Code Generation: QRCode-Generator library for PHP

# Overview

1. Front-End: The front-end application serves as the user interface for customers to browse events, purchase tickets, and receive unique QR codes. It also includes an admin interface for event organizers to create and manage events, set seating arrangements, and control pricing. Built with HTML, CSS, and Bootstrap, the front-end ensures a responsive design and is hosted on an Apache web server provided by XAMPP.
2. Back-End: The back-end application operates as the server-side component, built using PHP. It processes requests from the front-end, generates QR codes, and manages data flow to and from the database. This component handles operations such as seat allocation and ticket generation, ensuring efficient communication with the front-end.
3. Database: Data persistence is achieved through MariaDB, which stores all critical information related to the ticketing system. This includes event details, seat inventories, ticket sales records, and generated QR codes. MariaDB ensures data integrity and allows for quick access to real-time information.
4. QR Code Generator Library: Utilizes QRCode-Generator for PHP to create unique codes for each ticket

# Features
1. Dashboard displaying number of events, seats, and tickets sold
2. Sold Tickets tracking
3. Event management (CRUD operations)
4. Seat preferences management (pricing, count, types)
5. QR code generation for tickets

# Working:
1. Event Management: The QR Code Ticketing System begins with administrators logging into a secure interface. From here, they can create new events by specifying details such as date, time, venue, and total seats available. They also have the ability to set different seat types and their corresponding prices. The dashboard provides real-time statistics on ticket sales and event performance.
2. Customer Interaction: Customers can browse available events through the user-friendly front-end interface. Once they select an event, they can choose their preferred seats. After confirming their selection, the system generates a unique QR code for each ticket purchased. This QR code contains encrypted information about the ticket, including event details and seat numbers.
3. Data Management: All interactions between the front-end and back-end are managed through RESTful APIs. When an admin creates or modifies event information, this data is stored in MariaDB, which serves as the application's database. As customers make purchases, the system updates the database to reflect current seat availability and ticket sales.
4. QR Code Generation: The QR code generation process is handled by the QRCode-Generator library for PHP. Each time a ticket is sold, the system retrieves or creates the corresponding QR code and displays it to the customer. This unique code not only serves as a digital ticket but also enhances security by preventing fraud during entry at events.

# Steps to Create

1. Set up the database: Create a new MariaDB database in XAMPP. Import the provided SQL schema
2. Create the front-end: Develop HTML pages for main, events, and booking. Style with CSS and Bootstrap. Place in XAMPP's htdocs folder
3. Implement the back-end: Create PHP files for database connection and functions. Implement API endpoints for events and bookings. Place in XAMPP's htdocs folder
4. Set up admin interface: Create PHP pages for admin dashboard, event management, and bookings. Place in 'admin' subfolder
5. Implement QR code generation: Install QRCode-Generator library. Create PHP script for QR code creation
6. Configure web server: Set up Apache in XAMPP. Configure for PHP processing
7. Testing and security: Test all features. Implement user authentication for admin area. Ensure proper error handling and data validation
   
# Helpful Links
1. https://www.apachefriends.org/download.html - To install XAMPP
2. https://www.php.net/manual/en/intro-whatis.php - For PHP programming
3. https://www.qr-code-generator.com/guides/how-to-create-a-qr-code/?gclid=CjwKCAjwit
ShBhA6EiwAq3RqAyYCJuE6E6UWzmV5qXSiv8ITcJ1yUt6TyC5MGNsE7mMKK0Wa
XWlsURoCtBYQAvD_BwE&campaignid=1900357600&adgroupid=69312969046&cpi
d=1699f9da-d663-4ebd-8e9e-a39a17699165&gclid=CjwKCAjwitShBhA6EiwAq3RqAy
YCJuE6E6UWzmV5qXSiv8ITcJ1

   

