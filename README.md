# A simple calculator program

# Get the first number from the user
num1 = float(input("Enter the first number: "))

# Get the second number from the user
num2 = float(input("Enter the second number: "))

# Get the mathematical operation from the user
operation = input("Enter a mathematical operation (+, -, *, /): ")

# Perform the calculation based on the user's input
if operation == '+':
    result = num1 + num2
elif operation == '-':
    result = num1 - num2
elif operation == '*':
    result = num1 * num2
elif operation == '/':
    # Check if the user is trying to divide by zero
    if num2 == 0:
        result = "Error! Division by zero is not allowed."
    else:
        result = num1 / num2
else:
    result = "Error! Invalid operation."

# Print the result
print(f"The result is: {result}")

