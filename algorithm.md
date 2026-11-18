# Algorithm - Student Attendance Monitoring System

## Steps
1. Start the system and display the welcome message.
2. Initialise: declare the variables (totalStudents, studentsCount, presentCount, absentCount, studentName, studentID, attendanceStatus, attendancePercentage) and assign the fixed values (minStudents = 1, maxStudents = 100, attendanceTarget = 75, presentCode = "P", absentCode = "A").
3. Enter the total number of students: display a prompt and read totalStudents.
4. Validate the number: while totalStudents is less than minStudents or greater than maxStudents, display an error message and read totalStudents again.
5. Initialise counters: set presentCount = 0 and absentCount = 0.
6. Start the student loop: set studentsCount = 1.
7. Loop test: if studentsCount is greater than totalStudents, go to step 14; otherwise continue.
8. Enter student information: read studentName and studentID.
9. Record attendance: read attendanceStatus.
10. Validate attendance status: while attendanceStatus is not "P" and not "A", display an error message and read attendanceStatus again.
11. Update counters: if attendanceStatus = "P", add 1 to presentCount and display "marked PRESENT"; otherwise add 1 to absentCount and display "marked ABSENT".
12. Move to the next student: add 1 to studentsCount.
13. Repeat: return to step 7.
14. Calculate attendance percentage: attendancePercentage = (presentCount x 100) / totalStudents.
15. Display the attendance summary: totalStudents, presentCount, absentCount and attendancePercentage. If the percentage is at least attendanceTarget, display "Attendance target met"; otherwise display "Below target - follow-up recommended". Then display a thank-you message.
16. End the system.

## Correctness Checks
- **Termination:** the class-size loop ends when a valid number is entered; the student loop runs exactly totalStudents times; each status loop ends when P or A is entered.
- **No division by zero:** validation guarantees totalStudents is at least 1.
- **Counter check:** after every student, presentCount + absentCount equals the number of students processed.
- **Range:** the percentage is always between 0 and 100.
