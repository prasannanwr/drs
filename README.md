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

## 5.4 Daily Report Submission

### Description
Employees submit daily work reports.

Fields:

- Date
- Task Description
- Hours Worked
- Blockers / Issues
- Notes

---

## 5.6 Manager Review

Managers can review reports.

## 5.7 Report Dashboard

Dashboard shows:

Employee:

- Today’s report status
- Summary

Manager:

- Team activity

---

## 5.9 Notifications (optional)

Notifications for:

- Report submission 

Delivery methods:
- System notifications

---

## 6.2 Security

- Password encryption
- Secure authentication

---

# 7. Technology Stack

Backend:
- PHP / NodeJs

Frontend:
- HTML/CSS
- JavaScript

Database:
- MySQL

---

