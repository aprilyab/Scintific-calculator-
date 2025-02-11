README for Advanced Calculator Program
This document provides detailed instructions on compiling, running, and using the 
Advanced Calculator Program. It also includes example inputs and expected outputs 
to help you understand how the program works.
Overview
The Advanced Calculator Program performs a variety of mathematical operations, 
including basic arithmetic (addition, subtraction, multiplication, division), advanced 
operations (exponents, square roots), and trigonometric and logarithmic calculations.
The menu-driven interface allows users to select their desired operations and input 
values easily.
Requirements
 To run the program, you need the following:
 C++ Compiler: Any C++ compiler (e.g., GCC, Clang, or MSVC).
 Operating System: Works on Linux, macOS, or Windows (ensure you have a 
terminal).
How to Compile the Program
1. Save the program code in a file named calculator.cpp.
2. Open your terminal or command prompt.
3. Navigate to the directory containing calculator.cpp.
4. Use the following command to compile the program:
 G++ calculator.cpp -o calculator
This command creates an executable file named calculator.
If you encounter errors during compilation, ensure your C++ compiler is correctly 
installed.
How to Run the Program
1. After successful compilation, execute the program with the following 
command:
 ./calculator
 On Windows, you may need to run calculator.exe instead.
2. Follow the instructions displayed on the screen to perform calculations.
Using the Program
When you run the program, you will see the following menu:
======================== Calculator Menu ======================== 
What type of operation do you want? Choose from the following options: 
1. Addition 2. Subtraction 3. Multiplication 4. Division 
5. Exponential 6. Square Root 7. Sine (sin) 8. Cosine (cos) 
9. Tangent (tan) 10. Cosecant (csc) 11. Secant (sec) 12. Cotangent (cot) 
13. arcsin 14. Arccos 15. Arctan 16. Arccsc 
17. arcsec 18. Arccot 19. Logarithm (log) 20. Natural Logarithm (ln) 
 0. Exit
Steps to Perform a Calculation
1. Enter the number corresponding to your desired operation.
2. Follow the prompts to input the required values.
3. The program will display the result.
4. To perform another operation, choose an option from the menu again.
5. Enter 0 to exit the program.
Examples of Inputs and Expected Outputs
Here are some examples to demonstrate how to use the program:
Menu Choices and Corresponding Inputs/Outputs:
1. Addition (Choose 1)
Input:
Enter two numbers: 10 5
Output:15
2. Subtraction (Choose 2)
Input:
Enter two numbers: 10 5
Output:5
3. Multiplication (Choose 3)
Input:
Enter two numbers: 10 5
Output:50
4. Division (Choose 4)
Input:
Enter dividend and divisor: 10 2
Output:5
If the divisor is zero:
Input: Enter dividend and divisor: 10 0
Output: Error: division by zero is not allowed.
5. Exponential (Choose 5)
Input:
Enter the base and the exponent: 2 3
Output:8
6. Square Root (Choose 6)
Input:
Enter a number: 16
Output:
4
If the number is negative:
Input: Enter a number: -16
Output: Invalid input: negative numbers cannot have square roots.
7. Sine (sin) (Choose 7)
Input:
Enter a value of angle in degree: 30
Output:
0.49999 (approximately 1/2)
8. Cosine (cos) (Choose 8)
Input:
Enter a value of angle in degree: 30
Output:
0.866 (approximately √3/2)
9. Tangent (tan) (Choose 9)
Input:
Enter a value of angle in degree: 45
Output:
1
10. Cosecant (csc) (Choose 10)
Input:
Enter a value of angle in degree: 30
Output:
2 (since csc(30°) = 1/sin(30°) = 2)
11. Secant (sec) (Choose 11)
Input:
Enter a value of angle in degree: 60
Output:
2 (since sec(60°) = 1/cos(60°) = 2)
12. Cotangent (cot) (Choose 12)
Input:
Enter a value of angle in degree: 45
Output:
1 (since cot(45°) = 1/tan(45°) = 1)
13. Arcsine (arcsin) (Choose 13)
Input:
Enter a value: 0.5
Output:
0.5236 (approximately 30°)
14. Arccosine (arccos) (Choose 14)
Input:
Enter a value: 0.5
Output:
1.0472 (approximately 60°)
15. Arctangent (arctan) (Choose 15)
Input:
Enter a value: 1
Output:
0.7854 (approximately 45°)
19. Logarithm (log) (Choose 19)
Input:
Enter the number and base of logarithm: 8 2
Output:
3 (since log(8) base 2 = 3)
20. Natural Logarithm (ln) (Choose 20)
Input:
Enter a number: 20
Output:
2.9957 (approximately ln(20))
Error Handling
The program handles invalid inputs as follows:
Error Handling Examples
1. Division by Zero:
Input:
Enter operation : 4
Enter first number: 5
Enter second number: 0
Output:
Error: Division by zero is not allowed.
2. Negative Input for Square Roots:
Input:
Enter first number: -4
Output:
Invalid input: Cannot compute the square root of a negative number.
3. Undefined Trigonometric Functions (Cosecant):
Input:
Enter operation :csc
Enter first number (angle in radians): 0
Output:
Error: Cosecant is undefined for this value.
4. Logarithm of a Negative Number:
Input:
Enter operation : log
Enter first number: -10
Enter second number (base): 10
Output:
Invalid input: Logarithm undefined for negative values.
5. Invalid Operation Code:
Input:
Enter operation : xyz
Output:
Error: Invalid operation. Please enter a valid operation.
6. Invalid Numeric Input:
Input:
Enter operation : +
Invalid input. Please enter valid numeric values.
Invalid Menu Option: If the user enters an invalid option (e.g., 25), the program 
prompts. the user to enter a valid choice.
Exit the Program
To exit the program, select the menu option 0. Example:
Input:
Enter the number corresponding to your choice (21 for menu): 0
Output:
Thank you for using the calculator! Goodbye!
Author
This program was created as part of a mathematical operations project to 
demonstrate the use of C++ programming.
For any questions or feedback, please contact Henok yoseph wubie at 
henokapril@gmail.com 
