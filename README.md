# 🌐 Language Options:
**English** | [Bahasa Indonesia](README-id.md)

---

# GRAD-System (Graduation Data Management System)

A centralized graduation and yudisium administration management platform built on top of the **Laravel Framework**. This system bridges, automates, and accelerates the validation workflow of graduation prerequisites in *real-time* between graduating students, the BAAK division, and multi-departmental verifiers.

## Overview

GRAD-System replaces conventional, time-consuming university graduation bureaucraices with a modern unified digital solution. 

The application implements a strict *Multi-role Access Control (RBAC)* mechanism, tailoring dedicated operational workspaces for 6 distinct roles:
* **BAAK (Academic Administration & Student Affairs):** Acts as the Super Admin overseeing the entire graduation pipeline.
* **Students:** Submit necessary documentation and track validation progress in real-time.
* **Library Staff, Finance Staff, CSDL Staff, and Faculty Staff:** Act as specialized internal departmental verifiers.

Each role operates within an isolated workspace, guaranteeing a faster, highly structured, transparent, and secure document verification workflow.

---

# Main Features

## Multi-Role Authentication & Route Authorization
* Automated provisioning of unique dashboard modules customized for 6 different user privileges.
* Route protection enforced via strict role-based *Laravel Middleware*.
* **Automated Account Provisioning:** Student login credentials are automatically generated in batches by the system when BAAK imports student rosters.

## 📊 Roster & Data Management (BAAK Group)
* Instantly import or export graduating student datasets via spreadsheet formats.
* Integrated with *Email Automation* to dynamically dispatch login credentials (*username* & *password*) directly to individual student emails upon a successful roster import.

## 🎓 Graduation Registration & Yudisium Pipeline
Students can register for graduation and upload necessary prerequisite documents independently through their portal.
* **Real-Time Tracking Engine:** Enables BAAK to monitor graduation metrics, document completion rates, and cross-departmental approval workflows through live data feeds.
* **Isolated Verification Workspaces:** Verifiers from the Library, Finance, CSDL, and Faculty offices can directly validate requirements or attach revision notes if a submission is incomplete.
* Technical isolation ensures verifiers can only interact with their respective department's fields, while BAAK retains master administrative oversight.

## 🔔 Instant Notification Subsystem
Students receive immediate, actionable notifications directly on their dashboard regarding graduation schedule releases, requirement validation updates, and specific revision notes from checking staff.

## 📄 SKPI (Diploma Supplement) Document Management
* Students can input accomplishments and upload digital evidence for their SKPI portfolio directly into the system.
* Provides BAAK with comprehensive review dashboards, record-editing capabilities, data-cleaning tools, and an instant print engine for verified SKPI forms.

## 📦 Gown Distribution Logistical Tracker (Toga Tracker)
A digital logistics module to track graduation gown collections. The system locks and enforces toga eligibility, ensuring collection is only unlocked for students who have successfully cleared all institutional checkboxes and SKPI validations.

## 📣 Information Broadcast & Announcement Panel
Empowers BAAK to publish official yudisium notices, export visual metrics charts on graduation cohorts, and push critical circulars to the student network.

## ❓ Interactive Q&A Support Module
A built-in *Frequently Asked Questions* (FAQ) manager allowing BAAK to handle recurrent queries inside the app, minimizing repetitive inquiries sent to administrative staff.

## 📝 Testimonial Moderation Workflow
Graduates can submit feedback and reflections on their academic journey. Submissions are piped to a secure BAAK moderation queue for approval before publishing publicly.

## Student Hub Dashboard
An intuitive, self-service dashboard for students to register for yudisium, submit SKPI records, view public notices, update profile fields, track live verification timelines, and access direct communication shortcuts to BAAK via WhatsApp or Email.

---

# Technologies Used

* **Backend Architecture:** Laravel (PHP)
* **Database Management:** MySQL
* **Frontend Ecosystem:** Blade Template Engine, Bootstrap, JavaScript, HTML5 & CSS3

---

# System Roles & Privileges

| User Role | Technical Scope & Responsibilities |
| --------- | ------------------------------------------------------------------------- |
| BAAK      | Comprehensive lifecycle control, cross-departmental monitoring, data moderation |
| Student   | Yudisium registration, document uploads, portfolio & SKPI data management |
| Library   | Validates library clearance and thesis/dissertation final deposits |
| Finance   | Validates tuition settlement, institutional clearance, and graduation fees|
| CSDL      | Validates tracer study submissions and career-center records |
| Faculty   | Validates academic evaluation requirements and faculty-level paperwork |

---

# Key Highlights

* Engineered a sophisticated, deeply integrated multi-role dashboard architecture.
* Introduced a centralized, frictionless document verification workflow.
* Seamless distribution of auto-generated credentials utilizing automated email pipelines.
* Live tracking engine monitoring cross-departmental document approval states.
* Highly structured, relational file and data management system.
* Fully responsive web-layout scaling fluidly across modern screen resolutions.

---

# Screenshots

## Authentication Gateway
![Login Page](screenshots/login-page.png)

## Master BAAK Administration Console
![Admin Dashboard](screenshots/admin-dashboard.png)

## Interactive Student Dashboard
![Student Dashboard](screenshots/student-dashboard.png)

---

# Engineering Team Contribution

- **Liana Syifa Fauzia:** Lead Full-Stack Engineer (Architected backend layers, designed relational databases, programmed core system logic, built email automation pipelines, and led internal dashboard frontend engineering).
- **Ni'mas Subang Asih:** Development Support Specialist.
- **Hani Ayu Fadila:** Software Quality Assurance (QA) Analyst — managed system behavior testing and technical feedback cycles.
- **Ririn Dwi Ariyanti:** Software Quality Assurance (QA) Analyst & User Acceptance Testing (UAT) Support.
- **Wulan Saputri:** System Deployment Tester & Compliance Documentation Lead.
