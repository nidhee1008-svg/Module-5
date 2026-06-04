# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method.
3. Initialize an instance variable `status` with the value `"Alive"`.
4. Print the value of `status`.
5. Define the `__del__` method.
6. Print a message indicating that the object is being destroyed.
7. Create an object of the `Demo` class.
8. Delete the object using the `del` keyword.

## Program

```python
class Demo:
    def __init__(self):
        self.status = "Alive"
        print(self.status)

    def __del__(self):
        print("Object destroyed")

obj = Demo()
del obj
```

## 🧪 Output

```text
Alive
Object destroyed
```

## Result

Thus, the Python program to demonstrate a destructor was executed successfully.
