# students-report-system
python 
The program allows you to:

Add Student Data: Input student names and their marks for specific subjects.
View All Students: Display a basic list of all entered students.
Generate Reports: Print a detailed report for all students, including individual subject grades, average marks, overall grades, and identify the top-performing student.
Key Global Variable
subject = ["Maths", "English", "Science"]: This list defines the subjects for which student marks are recorded. It's accessible throughout the program.
Core Functions
get_valid_marks(subject_name):

Prompts the user to enter marks for a given subject_name.
Includes input validation to ensure that the entered mark is a valid number (float). It keeps asking until a valid number is provided.
get_students_input():

Collects data for multiple students until the user types 'done' for the student name.
For each student, it prompts for their name.
Then, it iterates through the subject list to get marks for each subject using get_valid_marks().
Stores each student's data as a dictionary { 'name': '...', 'marks': { 'Subject1': mark1, ... } } and adds it to a list of students.
get_grade(mark):

Takes a numerical mark as input.
Returns a letter grade ('A', 'B', 'C', 'D', 'F') based on predefined ranges (e.g., 80+ is 'A', 65+ is 'B').
calculate_average(student):

Takes a student dictionary (which includes their marks) as input.
Calculates the average mark across all subjects defined in the global subject list.
Ensures marks are treated as floats during calculation and rounds the average to two decimal places.
get_student_report(student):

Generates a comprehensive report dictionary for a single student.
It includes the student's name, a detailed breakdown of marks and grades for each subject, their overall average mark, and an overall letter grade based on that average.
get_all_results(students):

Takes a list of students and returns a list of individual student reports by calling get_student_report() for each student.
get_top_student(students):

Identifies the student with the highest average mark from the list of students.
Uses calculate_average as the key for comparison.
Returns the full student dictionary of the top student or None if no students are present.
view_all_students(students):

Prints the name and raw marks for each student in a simple list format.
print_report(students):

Formats and prints the detailed results report to the console.
It includes a header, a table showing each student's name, marks and grades per subject, average, and overall grade.
It also highlights the top student and provides a grade scale legend.
show_menu():

Displays the main menu options to the user (Add Student, View All Students, Print Report, Exit).
get_menu_choice():

Prompts the user to enter their choice from the menu.
Validates the input to ensure it's a number between 1 and 4.
main():

This is the main function that orchestrates the entire program.
It initializes an empty list students.
It enters a continuous loop, displaying the menu, getting the user's choice, and then calling the appropriate function based on that choice (add students, view students, print report, or exit).
Program Execution (if __name__ == "__main__":)
This standard Python construct ensures that the main() function is called only when the script is executed directly (not when imported as a module).
What's Happening in Your Output
Your output perfectly demonstrates the flow:

Welcome Message & Menu: The main() function starts, prints the welcome message, and displays the menu.
Invalid Choice: You entered '5', and the system correctly responded with "Invalid choice."
Adding Students: You then chose '1' (Add Student) and provided data for six students (wangechi, John, Amina, Angel, John, Ben), then typed 'done' to finish adding.
View All Students: You chose '2' (View All Students), and the program listed the names and raw marks for all the students you just entered.
Print Report: You chose '3' (Print Report), and the system generated the well-formatted table, calculated averages and grades, and correctly identified 'wangechi' as the top student.
Exiting: Finally, you chose '4' (Exit), and the program printed "Exiting the system. Goodbye!" and terminated.
This code provides a complete, interactive system for managing student results from data entry to detailed reporting.
