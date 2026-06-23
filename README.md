# AttendanceChimp: QR-Code Based Attendance Tracking for Instructors
**Tech Stack:** Python · Django · SQLite

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

Collaborators: _Keegan Ballantyne_ & _Yourou Li_

AttendanceChimp is a web application that is designed to help college instructors keep track of attendance in their classes. The application uses a unique method to track attendance, which involves the use of a random QR code projected on a screen at the start of each class.

The instructor simply logs into the AttendanceChimp web application and generates a unique QR code for each class session. This code is then projected onto the classroom screen at the start of the class. As students arrive, they take a picture of the QR code using their smartphones and upload it to a web form that is accessible through the AttendanceChimp application.

The AttendanceChimp application then automatically logs each student's attendance as they upload their QR code. The application maintains a real-time dashboard of attendance, which the instructor can access at any time to monitor attendance trends.

AttendanceChimp can potentially play a role in promoting positive mental health outcomes by encouraging regular attendance and reducing chronic absenteeism. By providing instructors with an easy and efficient way to track attendance, AttendanceChimp can help identify students who are struggling with attendance issues and allow instructors to provide support and resources as needed. This can help students feel more connected and engaged in their learning community, which can have a positive impact on their mental health.

## Overview - CMSC 13600 Course Project
We used a running quarter-long course project to reinforce the material taught in our course Introduction to Data Engineering. One of the hardest aspects of data engineering is understanding all of the software tooling and why it exists. In this project, we designed a working web-application from start to finish. Each week we built a different component. Our goal was to simulate the development practices one would see in the tech industry in terms of version control, unit testing, and documentation for software programs. 

### Design Requirement 1. Simple and Easy to Use
The main design requirement is to reduce the number of "clicks" needed for a student to log their attendance. AttendanceChimp should be a user-friendly, efficient, and cost-effective way for instructors to track attendance. The application eliminates the need for paper-based attendance sheets and helps instructors save time and effort. With AttendanceChimp, instructors can focus on teaching, while the application takes care of attendance tracking.

### Design Requirement 2. Advanced Attendance Analytics
The AttendanceChimp dashboard provides instructors with an overview of each class session, including the number of students present, absent, or tardy. The application also generates detailed reports that can be exported to Excel or other software for further analysis. The software should contain metrics to detect changes in typical student behavior and problematic trends.

### Design Requirement 3. Robust to Cheating
While AttendanceChimp provides an efficient way for instructors to track attendance, there are a few ways that students could potentially cheat the system. Here is one example:

Uploading a photo of someone else's QR code: If students have access to another student's QR code, they could potentially take a photo of it and upload it as their own, even if they are not present in the class. This could be prevented by requiring students to take a selfie or use some form of biometric authentication to verify their identity.

AttendanceChimp should have tools to mitigate evasion through duplicate QR codes or other forms of cheating.

## Architecture
AttendanceChimp was built on `python-django` (https://www.djangoproject.com/). Django is a high-level Python web framework that encourages rapid development and clean, pragmatic design. It takes care of much of the hassle of web development, so we can focus on writing our app without needing to reinvent the wheel. Django can run a local web-server and can easily interface with a database backend. We used a SQLite databaase backend. SQLite is a database engine written in the C programming language. It is not a standalone app; rather, it is a library that software developers embed in their apps.
