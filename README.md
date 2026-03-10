# Functional Requirements Document (FRD)
## Daily Report System

## 1. Document Information

| Version | Date | Author | Description |
|-------|------|------|-------------|
| 1.0 | 2026-03-10 | Prasanna | Initial FRD for Daily Report System |

---

# 2. Introduction

## 2.1 Purpose
The purpose of this document is to describe the functional requirements for the **Daily Report System**, a web-based platform that allows employees to submit daily work reports and managers to review and monitor productivity.

## 2.2 Scope
The Daily Report System will allow:

- Employees to submit daily reports
- Managers to review reports
- Track work progress and activities

The system will be accessible via web browsers.

## 2.3 Definitions

| Term | Description |
|-----|-------------|
| User | Employee who submits daily reports |
| Manager | Person who reviews reports |
| Admin | System administrator |

---

# 3. System Overview

The Daily Report System is designed to help organizations track employee daily work activities.

---

# 4. User Roles

## 4.1 Admin
Responsibilities:

- Manage users
- View all reports

## 4.2 Manager

Responsibilities:

- View reports from team members

## 4.3 Employee

Responsibilities:

- Submit daily reports

---

# 5. Functional Requirements

## 5.1 User Authentication

### Description
Users must log in to access the system.

### Requirements

- User login using email and password
- Password reset functionality
- Logout option

---

## 5.2 User Management

### Description
Admin can manage users.

### Requirements

Admin should be able to:

- Create users
- Edit users
- Delete users
  
User fields:
- Name
- Email
- Status

---

## 5.3 Project Management

### Description
Admin can manage projects.

### Requirements

Admin should be able to:

- Create projects
- Assign employees to projects
- Edit projects
- Deactivate projects

Project fields:

- Project Name
- Project Description
- Start Date
- End Date
- Status

---

## 5.4 Daily Report Submission

### Description
Employees submit daily work reports.

### Requirements

User should be able to:

- Create a report
- Select project
- Add work description
- Add hours worked
- Submit report

Fields:

- Date
- Project
- Task Description
- Hours Worked
- Blockers / Issues
- Notes

Validation:

- Only one report per day per user
- Required fields must be completed

---

## 5.5 Edit Report

Users may edit reports only within the same day.

Restrictions:

- Cannot edit reports from previous days
- Manager can request corrections

---

## 5.6 Manager Review

Managers can review reports.

Capabilities:

- View team reports
- Add comments
- Mark reports as reviewed
- Filter reports by date/user/project

---

## 5.7 Report Dashboard

Dashboard shows:

Employee:

- Today’s report status
- Total reports submitted
- Weekly summary

Manager:

- Team activity
- Missing reports
- Productivity metrics

Admin:

- System overview
- User activity
- Report statistics

---

## 5.8 Report History

Users can view report history.

Filters:

- Date range
- Project
- Status

Export options:

- CSV
- PDF

---

## 5.9 Notifications

Notifications for:

- Missing reports
- Manager comments
- Report approval

Delivery methods:

- Email
- System notifications

---

# 6. Non-Functional Requirements

## 6.1 Performance

- System should support at least 500 concurrent users
- Page load time should be under 3 seconds

## 6.2 Security

- Password encryption
- Role-based access control
- Secure authentication

## 6.3 Availability

- System availability: 99%

## 6.4 Backup

- Daily database backup
- Restore capability

---

# 7. Database Entities

Main entities:

- Users
- Projects
- Reports
- Comments
- Roles

---

# 8. Suggested Technology Stack

Example:

Backend:
- PHP / Laravel

Frontend:
- HTML
- CSS
- JavaScript
- Bootstrap / Vue

Database:
- MySQL

Authentication:
- JWT / Session based

---

# 9. Future Enhancements

Possible future features:

- Mobile application
- Timesheet integration
- Slack / Teams notifications
- Performance analytics
- AI-based productivity insights

---

# 10. Approval

| Role | Name | Signature | Date |
|----|----|----|----|
| Project Manager |  |  |  |
| Technical Lead |  |  |  |
| Stakeholder |  |  |  |
