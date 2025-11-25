# Python Attendance Tracker

## Project Overview
This project is a simple, command-line based attendance tracker implemented in Python. It allows users to mark student attendance as Present or Absent for given dates, using a date format of DD MM YY. Sundays are automatically detected and marked as holidays during which attendance cannot be marked.

## Features
- Interactive console interface to add attendance for multiple students per date.
- Date input strictly in DD MM YY format for consistency.
- Automated detection and marking of Sundays as holidays (no attendance entries).
- Options to mark each student as Present (P) or Absent (A).
- Attendance data is loaded from and saved to a CSV file (`attendance.csv`) ensuring persistence.
- View attendance records for all dates entered, including holiday markings.
- Input validation to minimize errors (date format, attendance status).
- Easy to extend and customize.

## Technologies Used
- Python 3.x
- Standard libraries: `csv`, `datetime`, `os`

## How to Use
1. Run the script in a Python environment.
2. From the menu, choose to mark attendance, view attendance records, or exit.
3. When marking attendance, enter the date in DD MM YY format or leave blank to use today’s date.
4. If the date is Sunday, the program automatically marks it as a holiday.
5. Enter student names and mark each as Present (P) or Absent (A). Type "done" to finish marking for the date.
6. Attendance is saved automatically to `attendance.csv`.
7. Use the view option to display all attendance records with holiday markings.

Example interaction:
Enter date (DD MM YY) or leave blank for today: 25 11 25
Mark attendance for 25 11 25:
Enter student name (or 'done' to finish): Rahul
Mark attendance - 'P' for Present, 'A' for Absent: P
Marked Rahul as Present.
Enter student name (or 'done' to finish): Aisha
Mark attendance - 'P' for Present, 'A' for Absent: A
Marked Aisha as Absent.
Enter student name (or 'done' to finish): done

Attendance saved.

text

## File Description
- `attendance.csv` - stores attendance data in CSV format with columns: Date, Student Name, Status.
- All attendance marked is persisted here and reloaded on program start.

## Extending the Project
- Add a graphical user interface (GUI) for convenience.
- Integrate unique student identifiers and automatic student list loading.
- Generate attendance summary reports (percentage attendance, absentees).
- Implement login for multiple teachers/admins.
- Add holiday list support beyond Sundays.

## Contribution
Contributions and feature requests are welcome via pull requests or issue reporting.

## License
This project is open source and free to use for educational and personal purposes.

## Author
Spoorthi

---

For questions or support, please contact Spoorthi via GitHub or email.
