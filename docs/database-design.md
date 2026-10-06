# CampusFix - Database Design

## 1. Database Overview

The CampusFix database stores information about users, campus locations, maintenance reports, and report status updates.

## 2. Users Table

| Field | Type | Description |
|---|---|---|
| user_id | Integer | Primary key |
| name | Varchar | User's name |
| email | Varchar | User's email |
| password | Varchar | User's password |
| role | Varchar | Student or Staff |

## 3. Locations Table

| Field | Type | Description |
|---|---|---|
| location_id | Integer | Primary key |
| building_name | Varchar | Campus building name |
| room_number | Varchar | Room number |

## 4. Reports Table

| Field | Type | Description |
|---|---|---|
| report_id | Integer | Primary key |
| user_id | Integer | Student who submitted the report |
| location_id | Integer | Location of the problem |
| issue_type | Varchar | Type of maintenance problem |
| description | Text | Description of the problem |
| status | Varchar | Reported, In Progress, or Fixed |
| created_at | DateTime | Date and time report was created |
| updated_at | DateTime | Date and time report was last updated |

## 5. Status History Table

| Field | Type | Description |
|---|---|---|
| history_id | Integer | Primary key |
| report_id | Integer | Related maintenance report |
| status | Varchar | Updated report status |
| updated_by | Integer | Staff member who updated the report |
| updated_at | DateTime | Date and time of the update |

## 6. Database Relationships

- One User can create many Reports.
- One Location can have many Reports.
- One Report can have many Status History records.

## 7. Simple Database Relationship Diagram

Users
  |
  | 1
  |
  | Many
Reports
  |
  | Many
  |
  | 1
Locations

Reports
  |
  | 1
  |
  | Many
Status_History

## 8. Database Purpose

This database allows CampusFix to store maintenance reports, identify where each problem occurred, connect reports to students, and keep track of changes to the status of each problem.