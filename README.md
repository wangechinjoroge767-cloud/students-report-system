# Student Results Management System Using Python

## Project Overview

The Student Results Management System is a simple, menu-driven Python application developed to manage student academic results. It allows users to enter student names and marks, calculate grades and average scores, generate performance reports, and identify the top-performing student.

This project demonstrates the practical application of Python programming concepts in managing and processing student academic data.

## Project Objectives

- Record student names and academic marks.
- Validate user input to ensure marks are within the permitted range.
- Calculate grades for individual subjects and overall performance.
- Calculate and display each student's average marks.
- Generate a report showing student performance.
- Identify the student with the highest average score.

## Key Features

### 1. Add Student Data
Users can enter student names and marks for Maths, English, and Science. Multiple students can be added during a session.

### 2. Input Validation
The application checks that marks are numerical values between 0 and 100. It also prevents empty student names and invalid menu selections.

### 3. Grade Calculation
The system automatically assigns letter grades according to the following grading scale:

| Marks | Grade |
|---|---|
| 80–100 | A |
| 65–79.99 | B |
| 50–64.99 | C |
| 40–49.99 | D |
| Below 40 | F |

### 4. Student Records
Users can view the names of all students entered and their recorded subject marks.

### 5. Performance Reports
The system generates a formatted report displaying each student's subject marks, individual subject grades, average score, and overall grade.

### 6. Top Student Identification
The application calculates student averages and identifies the student with the highest average mark.

### 7. Interactive Menu
Users can choose between adding students, viewing student records, generating reports, and exiting the application.

## Technologies Used

- **Programming Language:** Python
- **Data Structures:** Lists and dictionaries
- **Core Concepts:** Functions, loops, conditional statements, input validation, iteration, and calculations

## How to Run the Project

### Prerequisites
Install Python 3 on your computer.

### Instructions

1. Clone or download this repository.
2. Open the project folder in your terminal or code editor.
3. Run the following command:

```bash
python student_results_system.py
```

4. Follow the on-screen menu instructions to use the application.

On some systems, you may need to use `python3` instead of `python`.

## Example Usage

The application displays a menu with four options:

1. Add Student
2. View All Students
3. Print Report
4. Exit

After adding student records, users can view the entered data or generate a report containing grades, average scores, and the top-performing student.

## Learning Outcomes

Through this project, I applied Python programming concepts to a practical data management scenario. The project strengthened my understanding of:

- Organizing information using lists and dictionaries.
- Writing reusable functions.
- Validating user input.
- Performing calculations and applying conditional logic.
- Processing multiple records.
- Presenting results in a structured report.

## Limitations

The current application stores student records in memory while it is running. Records are not automatically saved to a permanent file or database, so they are lost when the program terminates.

The application is designed as a command-line program and does not currently include a graphical user interface or database integration.

## Conclusion

The Student Results Management System demonstrates how Python can be used to automate basic academic record management, calculate student performance, and generate structured reports. It serves as a practical foundation for developing more advanced data management applications.
