# student-management-system
Python mini project for managing student details
students = []

def add_student():
    name = input("Enter student name: ")
    roll = input("Enter roll number: ")
    marks = input("Enter marks: ")

    student = {
        "Name": name,
        "Roll No": roll,
        "Marks": marks
    }

    students.append(student)
    print("Student Added Successfully!")

def view_students():
    for student in students:
        print(student)

while True:
    print("\n1. Add Student")
    print("2. View Students")
    print("3. Exit")

    choice = input("Enter choice: ")

    if choice == "1":
        add_student()
    elif choice == "2":
        view_students()
    elif choice == "3":
        print("Project Ended")
        break
    else:
        print("Invalid Choice")
