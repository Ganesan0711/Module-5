
# Hierarchical Inheritance in Python

## 🎯 Aim
To write a Python program using hierarchical inheritance to input and display Employee and Patient details.

## 📘 Description
- **Base Class:** `Details`
  - Stores common attributes: `name` and `age`.
  - Provides methods: `getName()` and `getAge()`.
- **Derived Class 1:** `Employee`
  - Inherits from `Details`.
  - Adds `employee_id` and `department`.
  - Method: `getEmployeeDetails()`.
- **Derived Class 2:** `Patient`
  - Inherits from `Details`.
  - Adds `patient_id` and `disease`.
  - Method: `getPatientDetails()`.

## 🧠 Algorithm
1. Create a base class named `Details`.
2. Define common attributes such as name and age.
3. Create the `Employee` class inheriting from `Details`.
4. Create the `Patient` class inheriting from `Details`.
5. Get employee and patient details from the user.
6. Display the employee details.
7. Display the patient details.

## 💻 Program

```python
class Details:
    def getName(self):
        self.name = input("Enter name: ")

    def getAge(self):
        self.age = int(input("Enter age: "))


class Employee(Details):
    def getEmployeeDetails(self):
        self.getName()
        self.getAge()
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")

    def display(self):
        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def getPatientDetails(self):
        self.getName()
        self.getAge()
        self.patient_id = input("Enter patient ID: ")
        self.disease = input("Enter disease: ")

    def display(self):
        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


emp = Employee()
emp.getEmployeeDetails()
emp.display()

pat = Patient()
pat.getPatientDetails()
pat.display()
```

## 🧪 Sample Output

```text
Enter name: Ganesh
Enter age: 21
Enter employee ID: E101
Enter department: Mechanical

Employee Details
Name: Ganesh
Age: 21
Employee ID: E101
Department: Mechanical

Enter name: Kumar
Enter age: 40
Enter patient ID: P101
Enter disease: Fever

Patient Details
Name: Kumar
Age: 40
Patient ID: P101
Disease: Fever
```

## ✅ Result
Thus, the Python program to demonstrate hierarchical inheritance using a base class `Details` and derived classes `Employee` and `Patient` was executed successfully.
