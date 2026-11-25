
# Multilevel Inheritance Example in Python

## 🎯 Aim
To write a Python program using multilevel inheritance to get and display a person's name, age, and location.

## 🧠 Algorithm
1. Create a parent class named `Parent`.
2. Define a constructor `__init__()` to initialize the name.
3. Define a method `getName()` to return the name.
4. Create a child class named `Child` that inherits from `Parent`.
5. Use `super()` to initialize the name and add the age.
6. Define a method `getAge()` to return the age.
7. Create a grandchild class named `Grandchild` that inherits from `Child`.
8. Use `super()` to initialize the name and age and add the location.
9. Define a method `getLocation()` to return the location.
10. Get user input and display all details.

## 💻 Program

```python
class Parent:
    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name


class Child(Parent):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age


class Grandchild(Child):
    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def getLocation(self):
        return self.location


name = input("Enter name: ")
age = int(input("Enter age: "))
location = input("Enter location: ")

obj = Grandchild(name, age, location)

print("\nPerson Details")
print("Name:", obj.getName())
print("Age:", obj.getAge())
print("Location:", obj.getLocation())
```

## 🧪 Sample Output

```text
Enter name: Ganesh
Enter age: 21
Enter location: Chennai

Person Details
Name: Ganesh
Age: 21
Location: Chennai
```

## ✅ Result
Thus, the Python program to demonstrate multilevel inheritance using Parent, Child, and Grandchild classes was executed successfully.
