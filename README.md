# Timetable-Generator
A desktop application built using **Python**, **Tkinter**, and **SQLite** that automates the creation of class timetables for educational institutions. It allows admins to manage students, faculties, and subjects, and generates personalized schedules for both students and faculty based on input constraints.

---

## Key Features
- **Automated Scheduling**: Generates optimized timetables with minimal manual effort.
- **Conflict Resolution**: Handles constraints like availability, precedence, and room capacities.
- **Modular System**: Clean folder structure with separate modules for students, faculty, and scheduling.
- **Database-Driven**: Uses SQLite to store all user and schedule data.
- **User Roles**: Separate login-based views for Admins, Faculty, and Students.
- **Editable Data**: Admin can add/update/delete faculty, students, and subjects.
- **Report-Ready**: Timetables can be viewed per user and are ready for printing or exporting.

---

## System Overview
The application uses a centralized flow controlled by the `admin_screen.py` module:
- **Admin** manages all core data (students, faculty, subjects).
- **Scheduler** generates timetables based on inputs and constraints.
- Generated timetables are saved and accessed by:
  - Students (`timetable_stud.py`)
  - Faculty (`timetable_fac.py`)

All data is stored in `timetable.db`, which includes:
- `FACULTY` table
- `STUDENT` table
- `SUBJECTS` table
- `SCHEDULE` table

---

## Technologies Used
- **Python 3**
- **Tkinter** – GUI interface
- **SQLite** – Lightweight local database
- **OS & Sys Libraries** – File system and system control
- **VS Code** – Development environment

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Akira2206/Timetable-Generator.git
   cd Timetable-Generator
2.Run the application: 
   ```python main.py
