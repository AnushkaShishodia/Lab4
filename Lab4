class Employee:
    def __init__(self, emp_id, name, age, salary):
        self.emp_id = emp_id
        self.name = name
        self.age = age
        self.salary = salary

class EmployeeDatabase:
    def __init__(self):
        self.employees = []

    def add_employee(self, employee):
        self.employees.append(employee)

    def print_employees(self):
        for employee in self.employees:
            print(f"Employee ID: {employee.emp_id}, Name: {employee.name}, Age: {employee.age}, Salary: {employee.salary}")

    def sort_employees(self, key):
        if key == 1:
            self.employees.sort(key=lambda x: x.age)
        elif key == 2:
            self.employees.sort(key=lambda x: x.name)
        elif key == 3:
            self.employees.sort(key=lambda x: x.salary)
        else:
            print("Invalid sorting parameter")

if __name__ == "__main__":
    database = EmployeeDatabase()

    employee_data = [
        ("161E90", "Raman", 41, 56000),
        ("161F91", "Himadri", 38, 67500),
        ("161F99", "Jaya", 51, 82100),
        ("171E20", "Tejas", 30, 55000),
        ("171G30", "Ajay", 45, 44000),
    ]

    for emp_id, name, age, salary in employee_data:
        employee = Employee(emp_id, name, age, salary)
        database.add_employee(employee)

    print("Employee Data:")
    database.print_employees()

    while True:
        print("\nSelect sorting parameter:")
        print("1. Age")
        print("2. Name")
        print("3. Salary")
        print("4. Quit")
        choice = int(input("Enter your choice: "))

        if choice == 4:
            break

        database.sort_employees(choice)
        print("\nSorted Employee Data:")
        database.print_employees()
# Lab4