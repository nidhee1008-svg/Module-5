# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person's name, age, and location.

## 🧠 Algorithm

1. Create a parent class named `Parent`.
2. In the parent class, initialize the `name` attribute.
3. Define a method `getName()` to return the name.
4. Create a child class named `Child` that inherits from `Parent`.
5. In the child class, initialize the `age` attribute.
6. Define a method `getAge()` to return the age.
7. Create a grandchild class named `Grandchild` that inherits from `Child`.
8. In the grandchild class, initialize the `location` attribute.
9. Define a method `getLocation()` to return the location.
10. Create an object of `Grandchild`.
11. Print the name, age, and location using class methods.

## Program

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

print("Name:", obj.getName())
print("Age:", obj.getAge())
print("Location:", obj.getLocation())
```

## Sample Output

```text
Enter name: Nidhee
Enter age: 20
Enter location: Chennai
Name: Nidhee
Age: 20
Location: Chennai
```

## Result

Thus, the Python program to demonstrate multilevel inheritance was executed successfully.
