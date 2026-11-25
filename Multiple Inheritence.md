
# Arithmetic Operations Using Multiple Inheritance in Python

## 🎯 Aim
To write a Python program to perform Addition, Subtraction, and Division using Multiple Inheritance.

## 🧠 Algorithm
1. Define a class named `Calculation1`.
2. Create a method `Summation(a, b)` to calculate the sum of two numbers.
3. Define another class named `Calculation2`.
4. Create a method `Subtraction(a, b)` to calculate the difference between two numbers.
5. Define a class named `Derived` that inherits from both `Calculation1` and `Calculation2`.
6. Create a method `Division(a, b)` to calculate the division of two numbers.
7. Get two numbers from the user.
8. Create an object of the `Derived` class.
9. Call all three methods and display the results.

## 💻 Program

```python id="v8n2kx"
class Calculation1:
    def Summation(self, a, b):
        return a + b


class Calculation2:
    def Subtraction(self, a, b):
        return a - b


class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero is not possible"


a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

obj = Derived()

print("Addition:", obj.Summation(a, b))
print("Subtraction:", obj.Subtraction(a, b))
print("Division:", obj.Division(a, b))
```

## 📤 Output Example

```text id="m4q7wp"
Enter first number: 20
Enter second number: 5
Addition: 25.0
Subtraction: 15.0
Division: 4.0
```

## ✅ Result
Thus, the Python program to perform Addition, Subtraction, and Division using Multiple Inheritance was executed successfully.
