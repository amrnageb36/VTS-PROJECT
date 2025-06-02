# 🌴 Vacation Tracking System (VTS)

## 🌟 Project Vision

The **Vacation Tracking System (VTS)** enables employees to effortlessly manage their vacation, sick leave, and personal time off. Designed with usability and flexibility in mind, VTS streamlines the time-off request process by automating validations and approvals—eliminating the need for manual HR intervention or policy expertise.

---

## 🏢 Domain Overview

Traditionally, vacation requests required multiple layers of manual approvals—often taking days to process. VTS automates this workflow through a rules-based engine that minimizes manual input, reducing processing time and improving operational efficiency for HR teams.

---

## ✅ Functional Requirements

- 🔄 **Rules-Based Validation System**  
  Validates and verifies leave requests based on configurable business rules.

- 👤 **Manager Approval Workflow**  
  Supports optional manager approval depending on the employee's role.

- 📅 **Time Flexibility**  
  Allows employees to view and submit requests for:
  - Past leave (previous calendar year)
  - Future leave (up to 18 months ahead)

- 📧 **Email Notifications**  
  Automatically notifies managers and employees of request status changes and approval actions.

- 🛠 **Override Capabilities**  
  HR staff and system admins can override validation rules—with all overrides logged for audit purposes.

- 🎁 **Manager Privileges**  
  Managers can directly grant personal leave within pre-defined limits.

- 📓 **Activity Logs**  
  All user and system activities are recorded for transparency and auditing.

---

## 📈 Non-Functional Requirements

- 🖥 **Infrastructure Reuse**  
  Leverages the existing intranet portal’s hardware and middleware stack.

- 🔐 **Single Sign-On (SSO)**  
  Authenticates users via the portal’s existing SSO mechanism.

- 🔄 **Web Service API**  
  Provides vacation summary data for integration with other internal systems.

- 🔗 **HR System Integration**  
  Syncs with legacy HR systems for employee data updates and lookups.

- 🧾 **Comprehensive Logging**  
  Tracks and stores all system activity for traceability and monitoring.

---

## ⚙️ System Constraints

- Must be developed as an **extension of the existing intranet portal**.
- Must **reuse the current infrastructure** (hardware/middleware).
- Must **utilize the portal’s Single Sign-On (SSO)** for authentication.

---

## 👥 Project Actors

- **Employee**  
  Submits and manages personal leave, vacation, and sick requests.

- **Manager**  
  Has employee-level access, plus approval authority and the ability to grant comp time.

- **HR Clerk**  
  Oversees data integrity, manages records, and may access a dedicated HR interface.

- **System Administrator**  
  Manages server, database, and system-level operations including log maintenance.

---

## 📊 Diagrams & Documentation

### 🧠 Entity Relationship Diagram (ERD)

- [View ERD](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/ERD_diagram.png)

### 🔄 State Machine Diagram for Request Object

- [State Machine Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/state_machine_diagram_for_request.png)

---

## 📌 Use Cases

### 📅 Manage Time

- [Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/manageTime/sequenceDiagram.png)  
- [Flowchart Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/manageTime/flowchart.png)

---

### ❌ Cancel Request

- [Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/cancelRequest/cancel_request%20_seq.png)  
- [Flowchart Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/cancelRequest/cancel_request%20flow_chart.png)

---

### 🔙 Withdraw Request

- [Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/withdraw/withdraw_request%20seq.png)  
- [Flowchart Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/withdraw/withdraw_flowchart.png)

---

### ✏️ Edit Request

- [Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/edit/editSeq.png)  
- [Flowchart Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/diagrams/edit/editFlowChart.png)

---

## 🧰 Contributing

Contributions, issues, and suggestions are welcome! Please feel free to open a pull request or issue.

---
