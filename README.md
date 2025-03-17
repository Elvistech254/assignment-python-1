# assignment-python-1
# Simple Calculator Program

# Ask the user to input two numbers
num1 =("Enter the first number")
num2 =("Enter the second number")

# Ask the user to choose an operation
operation = input("Enter the operation (+, -, *, /): ")

# Perform the operation based on the user's input
if operation == "+":
    result = num1 + num2
elif operation == "-":
    result = num1 - num2
elif operation == "*":
    result = num1 * num2
elif operation == "/":
    # Check if the user is trying to divide by zero
    if num2 != 0:
        result = num1 / num2
    else:
        result = "Error! Division by zero."
else:
    result = "Invalid operation!"

# Display the result
print(f"The result of {num1} {operation} {num2} is: {result}")
