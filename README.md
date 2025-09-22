# Basic-Calculator-internship
import math

print("----- Basic Calculator -----")
print("Operations: +  -  *  /  %  ^")

# take inputs
num1 = float(input("Enter first number: "))
operator = input("Enter operator (+, -, *, /, %, ^): ")
num2 = float(input("Enter second number: "))

# calculate
result = None
if operator == "+":
    result = num1 + num2
elif operator == "-":
    result = num1 - num2
elif operator == "*":
    result = num1 * num2
elif operator == "/":
    if num2 != 0:
        result = num1 / num2
    else:
        print("Error! Division by zero.")
elif operator == "%":
    result = num1 % num2
elif operator == "^":
    result = math.pow(num1, num2)
else:
    print("Invalid operator!")

# show result
if result is not None:
    print("Result:", result)