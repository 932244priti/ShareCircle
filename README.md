# ShareCircle | Community Item Sharing Platform

**Share More. Waste Less. Build Stronger Communities.**

ShareCircle is a Java-based web application designed to make item sharing easier within apartments, hostels, and local communities. It provides a platform where users can explore items, submit booking requests, and manage their sharing activities through a simple, user-friendly interface.

The project aims to encourage resource reuse, reduce unnecessary purchases, and promote sustainable community living.

> **Project Status:** In Progress 🚧

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Application Modules](#application-modules)
- [Project Architecture](#project-architecture)
- [Database Management](#database-management)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## Overview

Many useful items remain unused in homes, hostels, and apartments. At the same time, other people may need those items temporarily.

ShareCircle aims to bridge this gap by providing a community-based item-sharing platform. Users can browse items across different categories, create accounts, and submit booking requests through the web application.

The application is being developed using Java and Spring Boot, with a MySQL database for persistent data storage.

## Key Features

- **User Management:** Registration and login pages.
- **Item Browsing:** Explore available items through a dedicated browsing interface.
- **Category-Based Navigation:** Browse items by categories such as books, electronics, sports, and others.
- **Booking Management:** Submit booking requests and view booking-related pages.
- **Payment Interface:** Mock checkout interface for demonstrating a payment workflow.
- **Responsive User Interface:** HTML and CSS-based pages designed for convenient navigation.
- **Database Integration:** Store application data using MySQL and Spring Data JPA.
- **Database Migrations:** Manage schema changes using Flyway.

## Technology Stack

| Technology | Purpose |
|---|---|
| Java | Backend programming |
| Spring Boot | Application framework |
| Spring MVC | Web request handling |
| Spring Data JPA / Hibernate | Database access and ORM |
| MySQL | Relational database |
| HTML5 | Page structure |
| CSS3 | Styling and layout |
| Thymeleaf | Server-side HTML templates |
| Maven | Dependency and build management |
| Flyway | Database schema migrations |
| Git & GitHub | Version control and source-code hosting |

## Application Modules

### 1. User Module
Handles the user registration and login interfaces.

### 2. Item Browsing Module
Displays items and provides category-based browsing.

### 3. Booking Module
Supports booking requests and booking-related pages.

### 4. Category Module
Organizes items into categories to make discovery easier.

### 5. Review Module
Provides the backend structure for item reviews.

### 6. Payment Interface
Includes a mock checkout page for demonstrating the payment flow. This is not a production payment gateway.

## Project Architecture

The application follows a layered structure to organize responsibilities and simplify future maintenance.

```text
User
 |
 v
Web Interface
(HTML, CSS, Thymeleaf)
 |
 v
Controllers
(Spring MVC)
 |
 v
Service Layer
(Business Logic)
 |
 v
Repositories
(Spring Data JPA)
 |
 v
MySQL Database
```

- **Controllers:** Handle incoming web requests.
- **Services:** Organize application operations and business logic.
- **Repositories:** Handle database access.
- **Entities:** Represent database-related objects.
- **DTOs:** Carry request data between the web layer and application logic.

## Database Management

ShareCircle uses MySQL for data storage and Flyway for database schema migrations.

The initial schema migration is maintained in:

`src/main/resources/db/migration/`

Database credentials should be configured locally and must not be committed to a public repository.

## Screenshots

The repository contains screenshots of the current application interface in the `Screenshots/` folder.

Examples include:

- Home Page
- Browse Items
- Category Pages
- Login Page
- Sign Up Page
- Booking Form
- Booking Submitted Page
- Payment Method Interface
- About Page

## Getting Started

### Prerequisites

Install the following software:

- Java Development Kit (JDK)
- MySQL Server
- Git
- IntelliJ IDEA or another Java IDE

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/932244priti/ShareCircle.git
cd ShareCircle
```

**2. Create the database**

Open MySQL and execute:

```sql
CREATE DATABASE sharecircle;
```

**3. Configure database credentials**

Configure the MySQL URL, username, and password in your local Spring Boot configuration. Do not publish real credentials.

**4. Run the application**

Open the project in IntelliJ IDEA, allow Maven dependencies to load, and run `SharecircleApplication.java`.

**5. Open the application**

If the application is configured for port 8081, open:

http://localhost:8081

> Note: The application configuration and database migration must be compatible with your local MySQL database before the application can run successfully.

## Future Enhancements

The following features are planned or may be considered for future development:

- Item listing and item-owner management
- Booking approval and return tracking
- Security deposit collection and refund workflow
- Integration with a real payment gateway
- Notifications for booking updates
- Ratings and reviews
- Improved authentication and role-based access control
- Deployment to a cloud platform

These enhancements will be implemented as the project evolves.

## Learning Outcomes

This project provides practical experience with:

- Java web application development
- Spring Boot application structure
- MVC architecture and layered design
- Relational database design
- ORM and repository patterns
- Database migrations
- Git and GitHub workflow

## Author

**Priti Bhagwan Gawai**

MCA (Data Science) Student

GitHub: [@932244priti](https://github.com/932244priti)

---

*ShareCircle is an academic project under active development. Features and implementation details may change as development continues.*
