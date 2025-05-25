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

## Manage time use-case

 Use case name: Manage Time
 Actor: Employee
 Goal: The employee wishes to submit a new request for vacation time.
 Preconditions: The employee is authenticated by the portal framework and 
identified as an employee of the company with privileges to manage his or her 
own vacation time. 
Main flow:
 1. The employee begins by selecting a link from the intranet portal to the 
VTS.
 2. The VTS uses the employee’s credentials to look up the current status 
of all the employee’s vacation time requests and outstanding balances. 
Information is displayed for the previous 6 months and up to 18 months 
in the future.
 3. The employee wants to create a new request. The employee selects 
one of the categories of vacation time with a positive balance to use.
 4. The VTS prompts the employee for the date(s) and time for which to 
request vacation time. The employee should have access to a visual 
calendar to help select and compare chosen dates.
CHAPTER 12 WEB APPLICATION: VACATION TRACKING SYSTEM
 503
 5. The employee selects the desired dates and hours per date (e.g., four 
hours might indicate a half-day vacation time request). The employee 
enters a short title and description (no more than a paragraph in length) 
so that the manager will have more information with which to approve 
this request. When all the information is entered, the employee submits 
the request.
 6. If the submitted information is incomplete or incorrect or does not pass 
validation, the Web page is redisplayed, with the errors highlighted and 
documented.
 7. The employee has an opportunity to change the information or cancel 
the request. 
8. If the information is complete and passes validation, the employee is 
returned to the main VTS home page. If the employee’s vacation time 
requests require manager approval, an e-mail is immediately sent to 
the manager(s) authorized to approve the employee’s requests. 
9. The vacation time request is placed in a state of pending approval.
 10. The manager responds to the e-mail by clicking on a link embedded in 
the e-mail or by explicitly logging into the intranet portal and navigating 
to the main VTS home page. 
11. The manager may be required to supply necessary authentication cre
dentials to gain access to the portal and VTS application.
 12. The VTS home page lists the manager’s own vacation time requests 
and outstanding balances but also has a separate section listing 
requests pending approval by subordinate employees. The manager 
selects each of these one at a time to individually approve or deny.
 13. The VTS displays the details of the requested time and prompts the 
manager to approve or disapprove the request. If the request is disap
proved, the manager is required to enter an explanation. Once the man
ager submits the result, the internal state of the request is changed to 
approved or rejected.
 14. Whether a request is approved or rejected, an e-mail notification is 
immediately sent to the employee who made the request. The man
ager’s screen returns to the main VTS home page, and the manager 
may approve other outstanding requests, make a request for him- or 
herself, or simply leave the VTS application

## Sequence diagram for Manage time use case

![Sequence Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/images/sequenceDiagram.png?raw=true)
 
## ERD diagram for Manage time use case

![ERD Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/images/ERD_diagram.png?raw=true)

## flow chart for Manage time use case

![ERD Diagram](https://github.com/amrnageb36/VTS-PROJECT/blob/main/images/flowchart.png?raw=true)
 
