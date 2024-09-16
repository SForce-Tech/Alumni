# Salesforce Academic Management System

## Project Overview

This project aims to develop a comprehensive academic management system using Salesforce, incorporating Experience Cloud and custom Lightning Web Components (LWC). The system is designed to manage student information, courses, grades, academic advising, and internal communications, providing a seamless and efficient experience for all users within the institution.

## Project Goals

- **Enhance User Experience:** Develop tailored portals for students, teachers, administrative staff, and the public to meet their specific needs.
- **Streamline Administrative Processes:** Centralize and automate academic workflows to reduce manual effort and errors.
- **Ensure Robust Data Management:** Leverage Salesforce's data management capabilities to securely handle all academic data, including student records, courses, grades, and advising details.
- **Automate Key Operations:** Utilize Salesforce automation tools (Apex, Flows) for notifications, enrollment processes, and other critical tasks.
- **Support Institutional Growth:** Create a scalable solution that can grow with the institution without needing complex external integrations.

## Key Features

1. **Custom Lightning Web Components (LWC):**

   - Student registration and management.
   - Course and grade management.
   - Academic advising and calendar modules.
   - Internal communications and resource management.

2. **Experience Cloud Sites:**

   - **Staff Portal:** Manage student data, courses, and generate reports.
   - **Teacher Portal:** Manage courses, grades, and communicate with students.
   - **Student Portal:** Enroll in courses, view grades, schedule advising sessions, and access learning resources.
   - **Public Site:** Provide information on academic offerings, news, and events.

3. **Automation and Business Logic:**

   - Apex Triggers and Classes for custom logic and data validations.
   - Salesforce Flows for automating critical processes like notifications and enrollments.
   - Apex REST Services for future integration opportunities.

4. **Security and Compliance:**

   - Configured user profiles, permissions, and validation rules to maintain data security and regulatory compliance.

5. **Analytics and Reporting:**
   - Custom reports and dashboards for monitoring key performance indicators (KPIs) such as enrollments, grades, and attendance.
   - Advanced analytics capabilities to support data-driven decision-making.

## Getting Started

### Prerequisites

- [Salesforce CLI](https://developer.salesforce.com/tools/sfdxcli) must be installed on your machine.

### Setup Instructions

1. **Clone the repository:**
   ```sh
   git clone git@github.com:SForce-Tech/Alumni.git
   cd Alumni
   ```
2. **Authenticate to your Salesforce Org:**
   ```sh
   sfdx force:auth:web:login -a <org-alias>
   ```
3. **Create a new scratch org:**
   ```sh
   sfdx force:org:create -s -f config/project-scratch-def.json -a <scratch-org-alias>
   ```
4. **Push source to the scratch org:**
   ```sh
   sfdx force:source:push
   ```
5. **Assign permission sets:**
   ```sh
   sfdx force:user:permset:assign -n <PermissionSetName>
   ```
6. **Open the scratch org:**
   ```sh
   sfdx force:org:open
   ```
7. **Run tests:**
   ```sh
   sfdx force:apex:test:run --resultformat human --codecoverage --testlevel RunLocalTests
   ```

## Ownership and Contact

This project is owned and maintained by [SForce Techies](https://www.sforce.tech). For inquiries or support, please contact [adrian@sforce.tech](mailto:adrian@sforce.tech).
