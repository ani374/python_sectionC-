PROJECT DESCRIPTION
The Gradebook Management System is a python-based application created and build to help schools to manage student's grade across many subjects.

The system lets the users to manage student records and perform different operations such as adding, removing, searching, sorting, and showing student details and grades.

The project is created and built very well, starting with the basic python concepts and continuing to more advanced programming concepts.

PURPOSE OF THE PROJECT
The purpose of this project is to create and build a user-friendly and a grading system that maanges grades much easily, quickly and accurately.

The system aims to make it easier to:
- Store student details
- Record student grades
- View student grades
- Search for students
- Add and remove students records
- Sort students records
- Generate useful grading details

  The project shows the use of important python programming concepts such as variables, loops, data structure, functions, classes.

  MAIN FEATURES
Features that will be provided by the gradebook management system:
- Add a new student
- Remove a student
- Search for a student
- View stdent recoreds
- View grades for a particular student for a particular subject
- Add or update student grades
- Sort student records
- Print student records
- Manage grades across multiple subjects
- Handle invalid input and errors

  TECHNOLOGIES USED
The project is created and built using the following:

- Pyhton
- python data structures such as dictionaries, tuples, list
- Python functions and loops
- Classes and objects
- Algorithms for searching and sorting

  HOW THE SYSTEM WORKS
  The system stores details about the students and their grades in python data structures.
For example a student may have infromation such as:

student = { 
    "name": "Aniah",
    "grades":{ 
          "Mathematics": 92,
          "English": 85,
          "Science": 88

  }
} 

The program can then use that information to show, search, update, or sort student records.

EXAMPLE OPERATIONS
1. Adding a student
The system allows the user to add a new student to the gradebook.

students ["Katlo"] = {"Math": 94, "English": 80, "Science": 82} 

2. Viewing student Records
    print(students)

This will show the student records stored in the gradebook system.

3. Viewing a subject grade
The system can also allow the user to view a student's grade for a particular subject.

math_grades = [info["Math"] for info in students.values()]
print("Math Grades:", math_grades) 


Below shows what was built from section A to C

SECTION A: Basic Student Grades
  FEATURES
  - Students and their grades stored in a **list of tuples**.
- Implemented:
  #Step 1: Number of students.
  #Step 2: Collect student names and grades.
  #Step 3: Calculate total grades and class average.
  #Step 4: Display each student’s grade compared to the class average.

 Example OUTPUT
  Class Summary:
Total Grades: 506
Class Average: 84.33

Aniah: 92 (Class Average: 84.33)
Mpho: 88 (Class Average: 84.33)
Leornad: 75 (Class Average: 84.33)
Phenyo: 83 (Class Average: 84.33)
Weno: 90 (Class Average: 84.33)
Mandisa: 78 (Class Average: 84.33) 

SECTION B: Multi-Subject Grades
    FEATURES
    - Extended to handle **three subjects**: Math, English, Science.
- Implemented:
  #Step 1: Number of students.
  #Step 2: Store student names with subject grades.
  #Step 3: Student summary table with averages.
  #Step 4: Highest and lowest grade per subject.

  Example OUTPUT
  Student Summary Table:
Name    Math    English    Science    Average
Aniah   92      85         88         88.33
Mpho    88      79         90         85.67
Leornad 75      80         70         75.00
Phenyo  83      77         85         81.67
Weno    90      89         91         90.00
Mandisa 78      82         76         78.67

Math: Highest = 92, Lowest = 75
English: Highest = 89, Lowest = 77
Science: Highest = 91, Lowest = 70

SECTION C: Dictionaries For Efficient Management
      FEATURES
- Transitioned from lists/tuples to **nested dictionaries**.
- Each student is a key, with subjects and grades stored in a nested dictionary.
- Implemented:
  - Add a new student.
  - Update an existing student’s grades.
  - Remove a student by name.
  - View all grades for a particular subject across all students.
  - Search for a student and calculate their average.
 
  EXAMPLE CODE OUTPUT FOR CREATING STUDENT DICTIONARY

  students = {
    "Aniah": {"Math": 92, "English": 85, "Science": 88},
    "Mpho": {"Math": 88, "English": 79, "Science": 90},
    "Leornad": {"Math": 75, "English": 80, "Science": 70},
    "Phenyo": {"Math": 83, "English": 77, "Science": 85},
    "Weno": {"Math": 90, "English": 89, "Science": 91},
    "Mandisa": {"Math": 78, "English": 82, "Science": 76}
}

EXAMPLE SEARCH

def get_student_info(name):
    if name in students:
        grades = students[name]
        avg = sum(grades.values()) / len(grades)
        print(f"{name}'s Grades: {grades}")
        print(f"{name}'s Average: {avg:.2f}")
    else:
        print(f"Student {name} not found.")

get_student_info("Aniah") 

OUTPUT
Aniah's Grades: {'Math': 92, 'English': 85, 'Science': 88}
Aniah's Average: 88.33


  

