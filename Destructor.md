
# Destructor in Python

## 🚀 Overview
This program demonstrates how to implement a destructor in Python using a simple class.

## 🎯 Aim
To write a Python program to demonstrate the working of a destructor using the `__del__()` method.

## 🧠 Algorithm
1. Define a class named `Demo`.
2. Create a constructor named `__init__()`.
3. Initialize an instance variable `status` with the value `"Alive"`.
4. Print the value of `status`.
5. Define a destructor named `__del__()`.
6. Print a message when the object is destroyed.
7. Create an object of the `Demo` class.
8. Delete the object using the `del` keyword.

## 💻 Program

```python id="m7x2qa"
class Demo:

    def __init__(self):
        self.status = "Alive"
        print("Object Status:", self.status)

    def __del__(self):
        print("Destructor called. Object is destroyed.")


obj = Demo()

del obj
```

## 🧪 Output

```text id="j9k3wp"
Object Status: Alive
Destructor called. Object is destroyed.
```

## ✅ Result
Thus, the Python program to demonstrate the destructor using the `__del__()` method was executed successfully.
