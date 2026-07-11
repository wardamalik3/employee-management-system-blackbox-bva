# Employee Management System | Black-box testing, Boundary Value Analysis, functional testing, manual testing

## Overview

This project is a desktop-based Employee Management System developed using JavaFX, Maven, and MySQL. The system is designed to manage employee records, leave requests, task assignments, performance tracking, and payroll-related operations through a structured JavaFX user interface connected to a relational database backend.

The project follows a controller-based JavaFX architecture where FXML views are mapped to dedicated Java controllers. The application uses JDBC and prepared statements for database interaction and JavaFX observable models/properties for displaying and updating employee, leave, and task data in table-based UI components.

## Core Functional Modules

- Employee record management including add, update, delete, profile view, and employee listing.
- Leave management workflow including employee leave request submission, manager approval, rejection, and leave status tracking.
- Task management workflow including task assignment, task update, task deletion, and task completion status handling.
- Performance management using performance factors and employee rating updates.
- Payroll-related functionality including salary calculation, payroll view, leave-based deductions, and report generation.
- Dashboard/report features for employee performance, department productivity, leave analysis, task completion, and monthly payroll review.

## Technical Stack

- Java 17
- JavaFX 17
- Maven
- MySQL
- JDBC
- FXML
- ControlsFX
- JUnit 5
- Jira for test case and bug tracking

## Database Design

The application uses a MySQL database named `EmployeeManagement`. The main entities include:

- `employees` for employee profile, department, position, salary, bonus, and performance factor data.
- `leave_requests` for employee leave request records and approval/rejection status.
- `tasks` for employee task assignment and completion status tracking.

## Testing

As part of the SQE assignment, the project was tested using black-box testing and boundary value analysis. Test cases were designed around critical business functions such as employee creation, employee update validation, leave request processing, task assignment, task update, payroll view, and report generation.

The testing work included:

- Creating and documenting functional test cases.
- Mapping expected results against actual results.
- Tracking pass/fail execution status.
- Identifying high-priority failed test cases.
- Logging critical bugs in Jira.
- Creating test dashboards for pass/fail ratio and high-priority failure tracking.
- Preparing Boundary Value Analysis documentation for controller-level input validation and error-handling scenarios.

## Key QA Findings

The testing process identified validation and workflow issues, including missing error handling when employee fields were left empty, update operations with incomplete input, and task update behavior not matching the expected result. These issues were documented as bugs and mapped against related failed test cases.

## Documentation

The repository includes supporting SQE documentation:

- SQE Assignment Report
- Boundary Value Analysis Test Cases
- Jira Test Case Export

## How to Run

### Prerequisites

- Java JDK 17 or above
- Maven
- MySQL Server
- JavaFX-supported environment

### Setup

1. Clone the repository.
2. Create the MySQL database using `database/schema.sql`.
3. Configure the following environment variables:

```bash
DB_URL=jdbc:mysql://localhost:3306/EmployeeManagement
DB_USER=root
DB_PASSWORD=your_password
```
