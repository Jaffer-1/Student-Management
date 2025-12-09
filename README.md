# UniTrack: University Student Management ERP System

## Project Overview

UniTrack is a comprehensive ERP system designed to digitalize various administrative and academic workflows within a university. It provides separate interfaces for Administrators, Faculty, and Students, implemented using a Role-Based Access Control (RBAC) model.

The project is available in two versions:

1. Web GUI: A modern dashboard built with HTML, CSS, and JavaScript, using LocalStorage for data persistence.  
2. C++ Backend: A console-based version using file handling for storing and managing student records.

---

## Features

### 1. Admin Portal

- Dashboard with statistics on student enrollment, hostel usage, and fee collection  
- Analysis tools for financial, academic, and logistical insights  
- Fee configuration for departments and facilities, including fines and adjustments  
- Management of student and faculty accounts  
- Viewable audit logs and downloadable JSON data backups  

### 2. Faculty Portal

- Access limited to students from the assigned department  
- Gradebook for searching, sorting, and updating student CGPA  
- Automatic class analysis including class average and top performers  
- Appeals system to review and process student academic requests  

### 3. Student Portal

- View personal profile, academic information, and fees  
- Pay academic and logistics fees (partial or full) through a simulated payment interface  
- Submit academic appeals and track their status  
- Receive administrative alerts related to dues or announcements  

---

## Technology Stack

| Component          | Technology               | Description                                    |
|--------------------|--------------------------|------------------------------------------------|
| Frontend GUI       | HTML, CSS, JavaScript    | Web interface with dynamic layouts             |
| Data Persistence   | LocalStorage / File I/O  | Browser storage for GUI; text files for C++   |
| Backend Logic      | C++ (STL)                | Classes for Admin, Faculty, and Student roles |
| Design             | Inter Font, SVG Icons    | Minimal and clean user interface               |

---

## How to Run

### Running the Web Dashboard
Open the file `index.html` in any modern browser.  
No setup is required. The version includes sample data for testing.

### Running the C++ Application
Open the `.cpp` file in a C++ IDE such as VS Code.  
Compile and run the program. It automatically creates the required text files (such as `unitrack_students.txt`) for data storage.

---

## Default Login Credentials

| Role       | Username     | Password   |
|------------|--------------|------------|
| Admin      | admin        | admin123   |
| Faculty    | prof_cse     | 123        |
| Student    | 21CSE101     | 123        |

---

## System Architecture

### Role-Based Access Control (RBAC)

- Admin: Full access to all financial, academic, and logistical data  
- Faculty: Access restricted to students from the assigned department; no financial access  
- Student: Access to their own profile, academic details, and appeals  

### Data Logic

- Searching and sorting implemented using efficient algorithms (linear search, bubble sort or quick sort logic)  
- Fee calculations based on base department fee plus logistics charges  
- Payments update the total due in real time  

---

## Usage Guide

- Login with the appropriate role  
- Admin can configure fee structures, add users, and view analytical reports  
- Faculty can update grades and address student appeals  
- Students can check their fee status, make payments, and submit appeals  

---

## Credits

Developer: Shaik Jaffer  
Course: Coding Skills - I (B.Tech, 3rd Semester)  
Submission Date: November 9, 2025
