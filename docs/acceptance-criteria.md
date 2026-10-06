# CampusFix - Acceptance Criteria

## AC-01: Submit Maintenance Report

Given a student is on the CampusFix report page,
When the student selects a location and issue type and submits the report,
Then the system should create a new maintenance report.

## AC-02: Select Issue Type

Given a student is creating a maintenance report,
When the student opens the issue type section,
Then the system should display the available issue categories:
- Air Conditioner
- Light
- Fan
- Toilet
- Wi-Fi
- Other

## AC-03: Select Location

Given a student is creating a maintenance report,
When the student selects a location,
Then the system should allow the student to select the building and room where the problem occurred.

## AC-04: Staff View Reports

Given maintenance reports have been submitted,
When university staff open the staff dashboard,
Then the submitted reports should be displayed.

## AC-05: Update Report Status

Given a staff member is viewing a maintenance report,
When the staff member changes the report status,
Then the new status should be saved and displayed.

The available statuses are:
- Reported
- In Progress
- Fixed

## AC-06: Fixed Problem

Given a maintenance problem has been solved,
When university staff change its status to "Fixed",
Then the system should display the report as Fixed.

## AC-07: Student Status Check

Given a student has submitted a maintenance report,
When the student checks the report,
Then the system should display its current status.

## AC-08: AI Chatbot

Given a user needs help using CampusFix,
When the user opens the AI chatbot,
Then the chatbot should provide guidance about reporting problems, checking report status, or navigating the website.