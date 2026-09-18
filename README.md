# DVLD – Driving License Management System

A desktop-based Driving License Management System (DVLD) developed using C# and .NET.

This project was created as a practical software development project to gain hands-on experience in building a complete application using Object-Oriented Programming, multi-layer architecture, database design, SQL Server, data access, business logic, and Windows desktop application development.

---

## 📌 Project Overview

The **Driving License Management System** is designed to manage different processes related to driving licenses and license applications.

The system allows users to manage applicants, applications, driving licenses, tests, appointments, and different license-related services through an organized desktop application.

The project focuses on implementing a complete application workflow rather than only individual features.

---

## 🚀 Main Features

### 👤 People & Applicants

* Add new people
* Update applicant information
* Search for existing people
* Manage personal information
* Store applicant photos and contact information

### 🪪 Driving Licenses

* Issue new driving licenses
* Manage existing licenses
* Renew licenses
* Replace lost or damaged licenses
* Release suspended licenses
* Issue international driving licenses
* View license information and history

### 📝 License Applications

* Create new applications
* Manage application status
* Track application information
* Process different types of license applications
* Manage application fees

### 🧪 Tests & Appointments

* Manage driving test appointments
* Manage vision/medical tests
* Manage theoretical tests
* Manage practical driving tests
* Handle test results
* Schedule re-examinations

### 🔎 Search & Management

* Search for people and applicants
* Search for licenses
* View application details
* Display related records and information
* Update and delete records where appropriate

---

## 🛠️ Technologies Used

| Technology        | Usage                               |
| ----------------- | ----------------------------------- |
| **C#**            | Main programming language           |
| **.NET**          | Application framework               |
| **Windows Forms** | Desktop user interface              |
| **SQL Server**    | Database management                 |
| **ADO.NET**       | Database communication              |
| **Visual Studio** | Development environment             |
| **Git & GitHub**  | Version control and project hosting |

---

## 🏗️ Application Architecture

The project is organized using a **multi-layer architecture** to separate responsibilities and make the application easier to maintain.

### Presentation Layer

Responsible for:

* Windows Forms
* User interface
* User interaction
* Input validation
* Displaying information

### Business Layer

Responsible for:

* Business rules
* Application logic
* Validation
* Processing operations
* Communication between the presentation and data layers

### Data Access Layer

Responsible for:

* Database connections
* SQL queries
* CRUD operations
* Reading and writing data
* Communication with SQL Server

### ***Why This Architecture?***

Separating the application into different layers makes the project easier to maintain, debug, and extend.

Each layer has a specific responsibility, which helps reduce dependencies between different parts of the application. This makes it easier to add new features or modify existing functionality without affecting the entire system.

Another benefit of this approach is that the business logic and data access are separated from the user interface. This provides more flexibility if the presentation layer needs to be replaced in the future.

For example, the current Windows Forms interface could potentially be replaced with a web-based frontend such as Angular, while keeping much of the underlying business logic and database functionality. The architecture therefore provides a foundation that can be extended or adapted as the project grows.

---

## 📂 Project Structure

```text
DVLD
│
├── BusinessLayer
│   └── Business logic and application rules
│
├── DataLayer
│   └── Database access and SQL operations
│
├── PresentationLayer
│   └── Windows Forms and user interface
│
├── Database
│   └── Database backup and related files
│
├── DVLD
│   └── Main application
│
├── DVLDSelfPhotos
│   └── Applicant/license photo handling
│
└── img
    └── Project screenshots and images
```

---

# 🖥️ Application Screenshots

The following screenshots demonstrate different parts of the application and its user interface.

### Login Dashboard

<img width="1089" height="670" alt="image" src="https://github.com/user-attachments/assets/327e4127-5bfa-4d46-aaa4-6ec4a8f3b5c5" />

### Main Dashboard
<img width="1739" height="977" alt="image" src="https://github.com/user-attachments/assets/afd036a2-8d62-45b0-81ee-81ad2a39b835" />

### License Management

<img width="1720" height="917" alt="image" src="https://github.com/user-attachments/assets/57775226-c944-4cd4-9059-b36ab627bcae" />


---

# 🔄 Example Application Workflow

A typical driving license application can follow a workflow similar to:

```text
Applicant
    ↓
Create Application
    ↓
Medical / Vision Test
    ↓
Theoretical Test
    ↓
Practical Driving Test
    ↓
Application Approved
    ↓
Driving License Issued
```

The system keeps track of the related information throughout the process.

---

# 🎯 What I Practiced & Learned

This project was mainly built as a practical way to improve my software development skills.

During the development of this application, I worked with:

* Object-Oriented Programming (OOP)
* C# and .NET
* Windows Forms
* SQL Server
* Database design
* ADO.NET
* CRUD operations
* Multi-layer architecture
* Separation of concerns
* Business logic implementation
* Data validation
* Exception handling
* Working with relational data
* Reusable components
* Git and GitHub
* Debugging and troubleshooting
* Designing user interfaces for desktop applications

One of the main goals of the project was to understand how different parts of a real-world application work together, from the user interface to the business logic and finally to the database.

---

# 🗄️ Database

The application uses **Microsoft SQL Server** as its database management system.

A database backup is included in the `Database` folder so that the database structure and sample data can be restored and used with the application.

The database contains the required tables, relationships, constraints, and data needed to manage:

* People
* Applicants
* Applications
* Licenses
* License classes
* Tests
* Appointments
* Application types
* Test types
* Users and related records

### 🧩 Database Design

The database was one of the **most important parts of this project**. I started the development by designing the database and spent a significant amount of time working on its structure, relationships, and consistency before building the application on top of it.

The goal was to create a **clean and well-structured relational database** with clear relationships between the different entities. Since many parts of the application depend on the database, careful database design was important for keeping the application consistent and making it easier to maintain and extend.

### 🔐 Password Security

User passwords are **hashed before being stored in the database**. Plain-text passwords are not stored.

### 🖼️ Image Storage

The application also handles images related to driving licenses.

Instead of storing the image files directly inside the database, the images are stored on the **server/file system**, while the corresponding **file path is stored in the database**.

This approach keeps the database focused on structured application data while the actual image files are managed separately.

### 📊 Entity Relationship Diagram

The following ERD shows the database structure and the relationships between the main entities:

<img width="4251" height="2593" alt="image" src="https://github.com/user-attachments/assets/da093484-e67d-4832-8d4d-660b774ef753" />

---

## 📜 License

This project was created for educational and portfolio purposes.

---

## 👤 Author

**Mohamad Almokhallati**

GitHub:
https://github.com/MohamadAlmokhallati

---

⭐ If you find this project interesting, feel free to explore the source code and the different layers of the application.
