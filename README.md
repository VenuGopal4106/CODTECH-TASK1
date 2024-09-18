Name: BOORLA VENU GOPAL
Company: CODTECH IT SOLUTIONS
ID: CT08DS7413
Domain: PYTHON PROGRAMMING
Duration: AUGUST to SEPTEMBER 2024

OVERVIEW OF THE PROJECT

Project Report: Basic Calculator Program

![Screenshot (147)](https://github.com/user-attachments/assets/84eba3bf-74af-4377-b3c9-b69ae4846dbf)



1. Introduction:
The Basic Calculator Program is a Python-based console application that allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, and division. The program is designed to prompt the user for two numerical inputs and an operation choice. Based on the user’s choice, it performs the appropriate operation and displays the result.

2. Objective:
The primary goal of this project is to develop a simple and functional calculator that:
- Prompts the user to select one of four arithmetic operations (addition, subtraction, multiplication, and division).
- Accepts two numerical inputs from the user.
- Performs the operation on the inputs and returns the result.
- Handles division by zero and provides an error message when the second number is zero in division.

3. Features:
- Basic Arithmetic Operations: Addition, subtraction, multiplication, and division.
- User Input: The program prompts users to input two numbers and an operation choice.
- Error Handling: The program checks for division by zero and returns an appropriate error message.
- Output: The result of the operation is displayed in the console.

4. Program Overview
4.1. Flow of the Program
1. The program begins by displaying a menu with four options for the user to select an operation.
2. The user selects an option (1 for addition, 2 for subtraction, 3 for multiplication, or 4 for division).
3. The user is prompted to enter two numbers, which will be used in the operation.
4. The program performs the chosen operation and displays the result.

4.2. Program Code

def calculator(num1, num2, n):
    match n:
        case 1:
            return num1 + num2
        case 2:
            return num1 - num2
        case 3:
            return float(num1 * num2)
        case 4:
            if num2 != 0:
                return float(num1 / num2)
            else:
                return "Error: Division by zero is not allowed."

#Displaying the operation menu
print("Select operation:")
print(" 1. Addition \n 2. Subtraction \n 3. Multiplication \n 4. Division")

# Taking user inputs
n = int(input("Enter choice (1/2/3/4): "))
num1 = float(input("Enter the number1: "))
num2 = float(input("Enter the number2: "))

# Displaying the result
print(calculator(num1, num2, n))

4.3. Explanation of Code
- Function Definition: The function `calculator` takes three parameters: `num1` (the first number), `num2` (the second number), and `n` (the operation choice).
- Match Statement: This structure is used to evaluate the user's choice of operation. It executes the corresponding arithmetic operation based on the value of `n`.
- Division by Zero Handling: A check is included to ensure that division by zero does not occur. If `num2` is zero and division is selected, an error message is returned instead of performing the operation.
- User Interface: The program interacts with the user through the console to gather inputs and display results.

Example Interaction:

Select operation:
 1. Addition 
 2. Subtraction 
 3. Multiplication 
 4. Division
Enter choice (1/2/3/4): 1
Enter the number1: 10
Enter the number2: 5
15.0

5. Limitations:
- Input Validation: The current version does not validate non-integer inputs for the operation choice or non-numeric inputs for the numbers.
- Floating-point Precision: As with many calculators, floating-point operations may result in minor precision errors.
  
6. Future Improvements
Potential future enhancements include:
- Adding input validation to ensure the user enters valid data.
- Allowing the calculator to perform operations on more than two numbers.
- Expanding the functionality to include more advanced operations such as exponentiation, square root, etc.
- Implementing a GUI (Graphical User Interface) for a more user-friendly experience.

. Conclusion:
This project successfully implements a basic calculator in Python that can perform addition, subtraction, multiplication, and division. It demonstrates key programming concepts such as user input handling, arithmetic operations, and basic error checking. Through this project, a foundational understanding of how calculators operate and how to implement them using Python has been gained.

