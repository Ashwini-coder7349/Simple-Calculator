COMANY:MICRO IIT

NAME:ASHWINI NAIK

DOMAIN: PYTHON PROGRAMMING

DURATION:1 MONTH

MENTOR:MR. VIJAY KUMAR

*** # Simple-Calculator
Here's a detailed explanation of a simple calculator application, along with a Python program to implement it:

Simple Calculator Application
A simple calculator application is designed to perform basic arithmetic operations, such as:

- Addition
- Subtraction
- Multiplication
- Division

The application typically features a user-friendly interface, where users can:

- Input numbers
- Select operations
- View results in real-time

***Python Program: Simple Calculator
Here's a Python program that implements a simple calculator application:


# Define a function for each arithmetic operation
def add(x, y):
    """Return the sum of x and y"""
    return x + y

def subtract(x, y):
    """Return the difference of x and y"""
    return x - y

def multiply(x, y):
    """Return the product of x and y"""
    return x * y

def divide(x, y):
    """Return the quotient of x and y"""
    if y == 0:
        raise ValueError("Cannot divide by zero!")
    return x / y

# Define a main function to handle user input and operations
def calculator():
    print("Simple Calculator")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    choice = input("Enter your choice (1/2/3/4): ")

    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            try:
                print(num1, "/", num2, "=", divide(num1, num2))
            except ValueError as e:
                print(e)
    else:
        print("Invalid choice")
# Call the calculator function
calculator()


***How the Program Works
1. The program defines four functions: add, subtract, multiply, and divide, each taking two arguments, x and y.
2. The calculator function serves as the main entry point, displaying a menu with options for the four arithmetic operations.
3. The user is prompted to enter their choice of operation.
4. Based on the user's choice, the program asks for two numbers, num1 and num2, which are used as arguments for the corresponding arithmetic function.
5. The result of the operation is then printed to the console.
6. If the user chooses division and attempts to divide by zero, a ValueError is raised with a message indicating that division by zero is not allowed.

***Example Use Cases
- Run the program and select option 1 (Addition). Enter two numbers, say 5 and 7, and the program will display the result: 5 + 7 = 12.
- Run the program and select option 4 (Division). Enter two numbers, say 10 and 2, and the program will display the result: 10 / 2 = 5.0.
- Run the program and select option 4 (Division). Enter two numbers, say 10 and 0, and the program will display an error message: Cannot divide by zero!.
