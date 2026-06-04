# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create a base class `Details` with common attributes `name` and `age`.
2. Create an `Employee` class that inherits from `Details`.
3. Add employee-specific details such as employee ID and department.
4. Create a `Patient` class that inherits from `Details`.
5. Add patient-specific details such as patient ID and disease.
6. Get user input for employee and patient details.
7. Display the collected information using class methods.

## Program

```python
class Details:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def getName(self):
        return self.name

    def getAge(self):
        return self.age


class Employee(Details):
    def __init__(self, name, age, employee_id, department):
        super().__init__(name, age)
        self.employee_id = employee_id
        self.department = department

    def getEmployeeDetails(self):
        print("Employee Name:", self.getName())
        print("Employee Age:", self.getAge())
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def __init__(self, name, age, patient_id, disease):
        super().__init__(name, age)
        self.patient_id = patient_id
        self.disease = disease

    def getPatientDetails(self):
        print("Patient Name:", self.getName())
        print("Patient Age:", self.getAge())
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


employee = Employee("Ravi", 30, "E101", "CSE")
patient = Patient("Anu", 25, "P101", "Fever")

employee.getEmployeeDetails()
print()
patient.getPatientDetails()
```

## Sample Output

```text
Employee Name: Ravi
Employee Age: 30
Employee ID: E101
Department: CSE

Patient Name: Anu
Patient Age: 25
Patient ID: P101
Disease: Fever
```

## Result

Thus, the Python program to demonstrate hierarchical inheritance was executed successfully.
