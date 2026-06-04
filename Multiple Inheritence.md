# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations: addition, subtraction, and division using three classes.

## 🎯 Aim

To write a Python program to calculate **addition, subtraction, and division** using **multiple inheritance**.

## 🧠 Algorithm

1. Define a class named `Calculation1`.
2. Inside it, define a method `Summation(a, b)` to return the sum of two numbers.
3. Define another class named `Calculation2`.
4. Inside it, define a method `Subtraction(a, b)` to return the difference of two numbers.
5. Define a class named `Derived` that inherits from both `Calculation1` and `Calculation2`.
6. Inside it, define a method `Division(a, b)` to return the division result.
7. Get two numbers from the user.
8. Create an object of the `Derived` class.
9. Call the `Summation`, `Subtraction`, and `Division` methods.
10. Display the results.

## 💻 Program

```python
class Calculation1:
    def Summation(self, a, b):
        return a + b


class Calculation2:
    def Subtraction(self, a, b):
        return a - b


class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        return a / b


a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

obj = Derived()

print("Addition:", obj.Summation(a, b))
print("Subtraction:", obj.Subtraction(a, b))
print("Division:", obj.Division(a, b))
```

## Output Example

```text
Enter first number: 10
Enter second number: 2
Addition: 12
Subtraction: 8
Division: 5.0
```

## Result

Thus, the Python program to perform arithmetic operations using multiple inheritance was executed successfully.
