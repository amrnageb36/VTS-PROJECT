# Vacation Tracking System (VTS)

## 🌟 Project Vision

The **Vacation Tracking System (VTS)** empowers employees to manage their own vacation time, sick leave, and personal time off with ease—without needing to be experts in company or facility-specific leave policies. The system provides a user-friendly, automated solution to streamline and modernize the vacation request process.

---

## 🏢 Domain Overview

Traditionally, vacation approvals involved multiple layers of manual work—manager approvals followed by HR clerks processing requests, often taking days to complete. This project automates and accelerates that workflow with a flexible, rules-based system that minimizes manual intervention, saving both time and cost for the HR department.

---

## ✅ Functional Requirements

- 🔄 **Rules-Based Validation System:** Validates and verifies leave requests using configurable business rules.
- 👤 **Manager Approval:** Optional workflow for immediate manager approval, depending on employee role.
- 📅 **Time Flexibility:** Allows access to past requests from the previous calendar year and supports requests up to 18 months into the future.
- 📧 **Email Notifications:** Notifies managers and employees of status changes and approval requests via email.
- 🛠 **Override Capability:** HR and system admins can override system rules with all actions logged.
- 🎁 **Manager Privileges:** Managers can directly award personal leave time within pre-defined system limits.
- 📓 **Activity Logs:** All transactions are recorded for auditing and transparency.

---

## 📈 Non-Functional Requirements

- 🖥 **Reuse Existing Infrastructure:** Built on top of the existing intranet portal, using the same hardware and middleware.
- 🔐 **Single Sign-On:** Authenticates users using the portal’s existing single-sign-on (SSO) mechanism.
- 🔄 **Web Service API:** Exposes vacation summaries for integration with other internal systems.
- 🔗 **HR System Integration:** Interfaces with legacy HR systems to retrieve and update employee data.
- 🧾 **Comprehensive Logging:** Logs all activities for traceability and system monitoring.

---

## ⚙️ System Constraints

- Must be implemented as an **extension of the intranet portal**.
- Must **reuse the existing hardware and middleware infrastructure**.
- Must **leverage the portal's single-sign-on (SSO)** for authentication.

---

## 👥 Project Actors

- **Employee:** Uses the system to manage personal leave, vacation, and sick time.
- **Manager:** Has all employee functionalities plus the ability to approve requests and award comp time (within limits).
- **HR Clerk:** Responsible for data accuracy and maintenance; can add/remove records; may use a separate login for HR tasks.
- **System Admin:** Ensures technical operation of the system, including server/database management and log archiving.

---

## Sequence diagram for Manage time use case

![Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/images/sequenceDiagram.png?raw=true)
 

