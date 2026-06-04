=# Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student's name provided by the user.

## 🧠 Algorithm
1. Accept the student's name from the user.
2. Create a class named `Student`.
3. Define a default constructor `__init__`.
4. In the constructor, assign the user input to an instance variable `self.a`.
5. Define a method `show` to display the constructor message and welcome message.
6. Create an object of the `Student` class.
7. Call the `show` method.

## 🧾 Program

```python
class Student:
    def __init__(self):
        self.a = input("Enter student name: ")

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)

obj = Student()
obj.show()
```

## Output

```text
Enter student name: Nidhee
This is non-parameterized constructor
Welcome Nidhee
```

## Result

Thus, the Python program to display a welcome message using a default constructor was executed successfully.
