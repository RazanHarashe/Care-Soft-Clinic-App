# CareSoft Clinic Management System

## Overview
CareSoft is a clinic management system designed to streamline healthcare operations while ensuring compliance with the Healthcare Insurance Portability and Accountability Act (HIPAA). This project includes the implementation of specific interfaces to enforce security and access protocols for healthcare professionals and administrative users.

## Project Structure
The project is structured using the reverse domain name convention. The main package for the application is `com.caresoft.clinicapp.demo`.

### Packages and Classes
- **Package**: `com.caresoft.clinicapp.demo`
  - **Interfaces**:
    - `HIPAACompliantUser`: Ensures that users comply with HIPAA requirements.
    - `HIPAACompliantAdmin`: Ensures that admins comply with HIPAA requirements and can report security incidents.
  - **Classes**:
    - `User`: A base class for all users in the system.
    - `Physician`: Extends `User` and implements `HIPAACompliantUser`.
    - `AdminUser`: Extends `User` and implements `HIPAACompliantUser` and `HIPAACompliantAdmin`.
  - **Test**:
    - `Test`: Contains test cases to verify the implementations of the classes and interfaces.
