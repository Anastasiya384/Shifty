# Technical Overview

## 1. Planned Technologies

The Shifty application is planned to be developed using the following technologies:

| Technology | Purpose |
|---|---|
| Flutter | Cross-platform application development |
| Dart | Main programming language |
| Firebase Authentication | User registration and authentication |
| Cloud Firestore | Cloud-based database for storing and synchronizing application data |
| Printing | Generating and printing PDF reports |

The application will use Firebase services to manage user accounts and store application data in the cloud.

## 2. System Architecture

Shifty will follow a client-cloud architecture.

The Flutter application will serve as the client-side application, providing the user interface for both administrators and employees.

Firebase will provide the backend services, including user authentication and cloud-based data storage.

The main architectural components will include:

- **Flutter Application:** Provides the user interface and application functionality for administrators and employees.
- **Firebase Authentication:** Handles user registration, login, and authentication.
- **Cloud Firestore:** Stores and synchronizes information about companies, users, work shifts, employee availability, absence requests, and working hours.
- **Printing Package:** Generates PDF reports containing employee working hours and monthly summaries.

The application will communicate with Firebase through the corresponding Firebase SDKs.

## 3. Data Model

The application will require several interconnected data entities to support its functionality.

The main planned entities include:

- **Company:** Stores information about registered businesses.
- **User:** Stores administrator and employee information.
- **Shift:** Represents individual work shifts.
- **ShiftSignup:** Stores employee registrations for specific shifts.
- **Availability:** Stores employees' availability information.
- **Absence:** Stores vacation and sick leave requests.
- **ShiftSwap:** Represents requests for exchanging work shifts.
- **TimeRecord:** Stores clock-in and clock-out records.
- **Announcement:** Stores announcements published by administrators.
- **Task:** Stores tasks assigned to individual employees.

The relationships between these entities will be defined as part of the database design.

An Entity-Relationship Diagram (ERD) will be used to visualize the conceptual data model.

Since Cloud Firestore is a NoSQL database, the final database structure will be adapted to its document-oriented data model.

## 4. Application Workflow

The application will support two main user roles: administrators and employees.

The administrator will first register an account and create a company profile. After configuring the company's working hours and shift requirements, the administrator will be able to invite employees to join the company through a QR code.

Employees will register their own accounts and request to join a company by scanning its QR code. Their membership will require administrator approval.

Once employees are connected to the company, they will be able to view the shared schedule, enter their availability, and sign up for available shifts.

The administrator will review employee registrations, make any necessary adjustments, and approve the final schedule.

The application will synchronize relevant changes through Firebase so that users can access up-to-date information.

## 5. Reports and Data Export

The application will use the Printing package to generate PDF reports.

Reports will be generated using working hours and other relevant records stored in the database.

Administrators will be able to export individual employee reports or monthly summaries covering all employees.

## 6. Security and Access Control

Firebase Authentication will be used to authenticate users.

The application will distinguish between administrators and employees, providing different functionality depending on the user's role.

Firebase security rules will be configured to restrict access to data according to user permissions and company membership.

Employees will only be allowed to access and manage information permitted by their role, while administrators will have additional permissions for managing their company and employees.
