# CampusFix - Requirements Specification

## 1. Introduction
CampusFix is a web-based campus maintenance reporting system. It allows students to report facility problems and university staff to manage those reports.

## 2. User Types
The system has two main user types:

1. Student
2. University Staff

## 3. Functional Requirements

### FR-01: Submit Report
The system shall allow students to submit maintenance reports.

### FR-02: Select Location
Students shall be able to select the building and room where the problem occurred.

### FR-03: Select Issue Type
Students shall be able to select an issue category such as:
- Air Conditioner
- Light
- Fan
- Toilet
- Wi-Fi
- Other

### FR-04: Problem Description
Students shall be able to enter additional information about the problem.

### FR-05: Report Status
Each maintenance report shall have a status:
- Reported
- In Progress
- Fixed

### FR-06: Staff Dashboard
University staff shall be able to view submitted maintenance reports through a dashboard.

### FR-07: Update Status
University staff shall be able to update the status of a maintenance report.

### FR-08: Check Status
Students shall be able to check the current status of their submitted reports.

### FR-09: AI Chatbot
The system shall provide an AI chatbot to help users with reporting problems, checking status, and navigating CampusFix.

## 4. Non-Functional Requirements

### NFR-01: Usability
CampusFix should have a simple and easy-to-understand interface.

### NFR-02: Performance
Pages and reports should load quickly.

### NFR-03: Accessibility
CampusFix should work on computers and mobile devices.

### NFR-04: Security
Only authorized university staff should be able to change the status of maintenance reports.

### NFR-05: Reliability
Submitted reports should be stored correctly and remain available until they are resolved.