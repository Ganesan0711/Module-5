
# Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a `Student` class with a default constructor and a method to display a welcome message along with the student's name provided by the user.

## 🧠 Algorithm
1. Get the student's name from the user.
2. Define a class named `Student`.
3. Create a default constructor using `__init__()`.
4. Store the student's name in the instance variable `self.a`.
5. Define a method named `show()` to display the constructor message and welcome message.
6. Create an object of the `Student` class.
7. Call the `show()` method to display the output.

## 🧾 Program

```python id="q7m2vn"
class Student:

    def __init__(self):
        self.a = input("Enter student name: ")

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)


obj = Student()
obj.show()
```

## 💻 Output

```text id="u8j5kp"
Enter student name: Ganesh
This is non-parameterized constructor
Welcome Ganesh
```

## ✅ Result
Thus, the Python program to create a Student class using a default constructor and display a welcome message with the student's name was executed successfully.
