# Student Attendance Monitoring System

A logical design for a simple system that helps a teacher or class representative record and summarise student attendance. This is a design project (algorithm, pseudocode and flowcharts), so it contains no source code.

## Objectives
- Apply computational thinking to an attendance-recording challenge
- Design an algorithm, pseudocode and Flowgorithm flowcharts that match each other
- Demonstrate input, processing, output, decisions, loops, modules and functions
- Show how open source and Digital Public Goods ideas support SDG 4: Quality Education

## How the System Works
1. Enter the number of students (valid range: 1 to 100).
2. For each student, enter the name and ID, then record P (Present) or A (Absent).
3. Invalid entries are rejected and the user is asked again.
4. The system counts present and absent students and calculates:
   Attendance Percentage = (Students Present / Total Students) x 100
5. A summary is displayed with a status against a 75% target.

## Repository Contents
| Folder / File | Description |
|---|---|
| `algorithm/` | Step-by-step algorithm |
| `pseudocode/` | Pseudocode for the whole system |
| `flowchart/` | Flowgorithm file and flowchart images |
| `screenshots/` | Test run screenshots |
| `report/` | Final assignment report |

## Modules
- `ValidateStudentCount()` checks the class size
- `RecordAttendance()` reads and validates P or A
- `CalculateAttendancePercentage()` applies the formula
- `GenerateAttendanceReport()` displays the summary

## SDG and Open Source
Supports **SDG 4: Quality Education**. Intended as open-source software and a possible Digital Public Good. It is not an officially recognised Digital Public Good.
