# AcademiCore – Django + SQLite3

## Project Overview
This is **AcademiCore**, a **Student Management System** built using **Python**, **Django**, and **SQLite3**.  
It allows staff to efficiently manage students, courses, attendance, topics, batches, tests, and placements.

## Tech Stack
- Python 3.x  
- Django Framework  
- SQLite3 Database  
- HTML (for templates)  

## Features
- Student & Staff Management: Create, update, and manage student and staff records.  
- Course & Topic Management: Assign students to courses and track progress on topics.  
- Attendance Tracking: Record attendance for students and staff.  
- Batch Management: Create and assign students to batches.  
- Test & Placement Tracking: Record test scores, mock assessments, and placement outcomes.  
- Database Integrity: Relationships and constraints like `unique_together` to prevent duplicate entries.  

## SQL / Database Work
- Designed relational tables using Django ORM (SQLite3 backend).  
- Implemented One-to-One, One-to-Many, and Many-to-Many relationships.  
- Performed CRUD operations using Django ORM.  
- Used filters, joins, and aggregate functions for data retrieval and manipulation.  
- Enforced primary keys, foreign keys, and unique constraints for data integrity.  

## Folder Structure



TesDBRegister-main/
│
├── db.sqlite3
├── manage.py
├── requirements.txt
├── <app_name>/
│ ├── migrations/
│ ├── templates/
│ ├── admin.py
│ ├── models.py
│ ├── views.py
│ └── ...
└── templates/

## How to Run AcademiCore

1. Open Command Prompt or PowerShell and navigate to the project directory:
   C:\Users\Admin\Desktop\DjangoProject\TESDBREGISTER_Project\TesDBRegister-main

2. (Optional) Create a virtual environment to keep dependencies isolated:
   python -m venv venv
   venv\Scripts\activate

3. Install project dependencies:
   pip install --upgrade pip
   pip install django
   pip install -r requirements.txt   # if a requirements file is available

4. Apply database migrations to create tables:
   python manage.py makemigrations
   python manage.py migrate

5. Create a superuser to access the Django admin panel:
   python manage.py createsuperuser
   # Follow prompts to set username, email, and password

6. Start the development server:
   python manage.py runserver

7. Access the project:
   - Main site: http://127.0.0.1:8000/
   - Admin panel: http://127.0.0.1:8000/admin

Notes:
- Make sure Python 3.x is installed on your system.
- Virtual environment is recommended but optional.
- All database tables are handled automatically via Django ORM.

## Usage
- Add students, staff, courses, and batches through the admin panel.  
- Track attendance, topics, tests, and placements.  
- Ensure unique entries using the enforced database constraints.

## Notes
- Developed using Django ORM with SQLite3.  
- Relationships handled in models using `ForeignKey`, `ManyToManyField`, and `OneToOneField`.  
- Ensure Python 3.x and Django are installed before running.

