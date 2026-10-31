# School Management System

Course project for CSE 311 (Database Systems).

A web-based school management system built with Flask and MySQL. Teachers and students have separate logins and dashboards.

## Team

- [konokuzzaman](https://github.com/konokuzzaman)
- [wahiPP](https://github.com/wahiPP)

## Features

**Teacher**
- Manage students, teachers, classes, sections and subjects
- Enroll students and assign subjects to teachers
- Create exams and enter marks
- Take attendance
- Download marks and attendance as CSV

**Student**
- View their own dashboard with marks and attendance
- Change password

## Tech Stack

- Python, Flask
- MySQL
- HTML, CSS, JavaScript (Jinja templates)

## Database

The schema is in `schema.sql` and includes tables for teachers, students, accounts, classes, sections, enrollments, subjects, subject assignments, exams, marks and attendance.

## How to Run

1. Install the dependencies:
   ```
   pip install -r requirements.txt
   ```
2. Create the database in MySQL and load the schema:
   ```
   mysql -u root -p < schema.sql
   ```
3. Set your database login (or edit `DB_CONFIG` in `app.py`):
   ```
   set DB_USER=your_mysql_user
   set DB_PASSWORD=your_mysql_password
   set DB_NAME=school_db
   ```
4. Start the app:
   ```
   python app.py
   ```
5. Open http://127.0.0.1:5000 in your browser.

New students and teachers are created with the default password `123456`, which can be changed after logging in.
