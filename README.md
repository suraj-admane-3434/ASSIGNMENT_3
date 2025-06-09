# ASSIGNMENT_3

import math

# Task 1: Factorial using a function
def factorial(n):
    if n < 0:
        return "Factorial is not defined for negative numbers."
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

# Calling the factorial function with a sample number
sample_number = 5
print(f"Factorial of {sample_number} is: {factorial(sample_number)}")

# Task 2: Using math module for calculations
try:
    user_input = float(input("\nEnter a number for math calculations: "))
    if user_input < 0:
        print("Square root and logarithm are not defined for negative numbers.")
    else:
        print(f"Square root of {user_input} is: {math.sqrt(user_input)}")
        print(f"Natural logarithm (log base e) of {user_input} is: {math.log(user_input)}")
    print(f"Sine of {user_input} radians is: {math.sin(user_input)}")
except ValueError:
    print("Invalid input. Please enter a valid number.")
######################################################################################################################################################################
