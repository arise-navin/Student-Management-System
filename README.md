# Student Management System

## Overview

This Java-based Student Management System is a console application designed to manage student records and their examination results. The system allows administrators to:

- Add new student profiles
- Record examination marks for multiple subjects
- View student details
- Generate examination reports with grades and percentages

## Features

### Student Management
- Store student information including:
  - Name
  - Roll Number
  - Date of Birth
  - Email
  - Student ID
  - Course

### Examination System
- Record marks for up to 5 subjects per student
- Automatic grade calculation (A+ to F)
- Percentage calculation for each subject
- Overall performance summary
- Grade conversion based on marks:
  - 90-100: A+
  - 80-89: A
  - 70-79: B+
  - 60-69: B
  - 50-59: C
  - 40-49: D
  - Below 40: F

## Technical Details

### Classes Structure
1. **Student**: Stores personal and academic information
2. **Subject**: Manages subject-specific data and grading
3. **Examination**: Handles multiple subjects and overall performance
4. **StudentManagementSystem**: Main class with user interface

### Data Storage
- Uses in-memory arrays (supports up to 100 students)
- Parallel arrays for students and their examinations

## How to Use

1. **Compile and Run**:
   ```
   javac StudentManagementSystem.java
   java StudentManagementSystem
   ```

2. **Menu Options**:
   - **Add New Student**: Create a student profile
   - **Add Examination Details**: Enter marks for 5 subjects
   - **View Student Details**: Display student information
   - **View Examination Results**: Show marks, grades, and percentages
   - **Exit**: Close the application

## Requirements

- Java JDK 8 or later
- Basic terminal/command prompt to run the application

## Limitations

- Data is not persisted between runs (in-memory storage only)
- Fixed maximum of 100 students
- Exactly 5 subjects required per student examination

## Future Enhancements

1. Implement database persistence
2. Add edit/delete functionality for student records
3. Support variable number of subjects
4. Add user authentication
5. Implement CSV import/export functionality
