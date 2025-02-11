#pragma once // to ensure a file is only included once, preventing errors caused
             // by multiple inclusions

void displayMenu();
// Declaration of addition function
double addition(double a, double b);

// Declaration of difference function (subtraction)
double difference(double a, double b);

// Declaration of division function
double division(double a, double b);

// Declaration of multiplication function
double multiplication(double a, double b);

// Declaration of power function
double Exponential(double a, double b);

// Declaration of square root function
double square_root(double a);

// Declaration of sine function
double sine(double a);

// Declaration of cosine function
double cosine(double a);

// Declaration of tangent function
double tangent(double a);

// Declaration of cosecant function
double cosecant(double a);

// Declaration of secant function
double secant(double a);

// Declaration of cotangent function
double cotangent(double a);

// Declaration of arcsine function (inverse sine)
double arcsine(double a);

// Declaration of arccosine function (inverse cosine)
double arccosine(double a);

// Declaration of arctangent function (inverse tangent)
double arctangent(double a);

// Declaration of logarithmic function with a given base
double logarithmic(double a, double b);

// Declaration of natural logarithmic function (base e)
double natural_logarithmic(double a);
#include <cmath> // Include the cmath library for mathematical functions
#include <iostream>
#include <limits>
using namespace std;
#include "new.h" // Include the user-defined header file for additional functions

int main() {
  int type_of_operation; // Variable to store user's choice of operation

  // Display the calculator menu
  cout << "======================== Calculator Menu ========================"
       << endl;
  cout << "What type of operation do you want? Choose from the following "
          "options: "
       << endl;
  displayMenu();
  bool running = true;
  // Input the user's choice
  while (running) {
    cout << "Enter the number corresponding to your choice (21 for menu): ";
    cin >> type_of_operation;

    double a; // Variable to store input number
    double b; // Variable to store input number

    // Switch case to execute the operation based on user's choice
    switch (type_of_operation) {

    case 0:
      // Exit the program
      cout << "Thank you for using the calculator.\n";
      exit(0); // Exit the program

    case 1:
      // Addition operation
      cout << "enter two numbers :  ";
      cin >> a >> b;
      cout << addition(a, b) << endl; // Call the addition function
      break;

    case 2:
      // Subtraction operation
      cout << "enter two numbers:  ";
      cin >> a >> b;
      cout << difference(a, b) << endl; // Call the difference function
      break;

    case 3:
      // Multiplication operation
      cout << "enter two numbers:  ";
      cin >> a >> b;
      cout << multiplication(a, b) << endl; // Call the multiplication function
      break;

    case 4:
      // Division operation
      cout << "enter dividend and divisor:  ";
      cin >> a >> b;
      cout << division(a, b) << endl; // Call the division function
      break;

    case 5:
      // Exponential operation (a^b)
      cout << "enter the base and the exponent:  ";
      cin >> a >> b;
      cout << Exponential(a, b) << endl; // Call the power function
      break;

    case 6:
      // Square Root operation
      cout << "enter a number:  " << endl;
      cin >> a;
      cout << square_root(a) << endl; // Call the square root function
      break;

    case 7:
      // Sine operation (sin)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;            // Convert angle from degrees to radians
      cout << sine(a) << endl; // Call the sine function
      break;

    case 8:
      // Cosine operation (cos)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;              // Convert angle from degrees to radians
      cout << cosine(a) << endl; // Call the cosine function
      break;

    case 9:
      // Tangent operation (tan)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;               // Convert angle from degrees to radians
      cout << tangent(a) << endl; // Call the tangent function
      break;

    case 10:
      // Cosecant operation (csc)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;                // Convert angle from degrees to radians
      cout << cosecant(a) << endl; // Call the cosecant function
      break;

    case 11:
      // Secant operation (sec)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;              // Convert angle from degrees to radians
      cout << secant(a) << endl; // Call the secant function
      break;

    case 12:
      // Cotangent operation (cot)
      cout << "enter a value of angle in degree:  " << endl;
      cin >> a;
      a = a / 57.3;                 // Convert angle from degrees to radians
      cout << cotangent(a) << endl; // Call the cotangent function
      break;

    case 13:
      // Inverse Sine operation (arcsin)
      cout << "enter a value:  " << endl;
      cin >> a;
      cout << arcsine(a) << endl; // Call the arcsine function
      break;

    case 14:
      // Inverse Cosine operation (arccos)
      cout << "enter a value:  " << endl;
      cin >> a;
      cout << arccosine(a) << endl; // Call the arccosine function
      break;

    case 15:
      // Inverse Tangent operation (arctan)
      cout << "enter a value:  " << endl;
      cin >> a;
      cout << arctangent(a) << endl; // Call the arctangent function
      break;

    case 19:
      // Logarithm operation (log)
      cout << "enter the number and base of logarithm:  ";
      cin >> a >> b;
      cout << logarithmic(a, b) << endl; // Call the logarithmic function
      break;

    case 20:
      // Natural Logarithm operation (ln)
      cout << "enter a number:  ";
      cin >> a;
      cout << natural_logarithmic(a)
           << endl; // Call the natural logarithmic function
      break;
    case 21:
      displayMenu();
      break;
    default:
      // Invalid input handling
      cerr << "invalid input: your input do not match with any given options "
              "of operations  "
           << endl; // Error message if the input doesn't match any case
      cin.clear();
      cin.ignore(numeric_limits<int>::max(), '\n'); // clears the input stream
      break;
    }
  }

  return 0;
}
#include "new.h" // Include the user-defined header file for additional functions
#include <cmath> // Include the cmath library for mathematical functions
#include <iomanip>
#include <iostream>
using namespace std;

void displayMenu() {
  cout << left;
  cout << "======================== Calculator Menu ========================"
       << endl;
  cout << "What type of operation do you want? Choose from the following "
          "options: "
       << endl;
  cout << setw(20) << "1.  Addition" << setw(20) << "2.  Subtraction"
       << setw(20) << "3.  Multiplication" << setw(20) << "4.  Division"
       << endl;
  cout << setw(20) << "5.  Exponential" << setw(20) << "6.  Square Root"
       << setw(20) << "7.  Sine (sin)" << setw(20) << "8.  Cosine (cos)"
       << endl;
  cout << setw(20) << "9.  Tangent (tan)" << setw(20) << "10. Cosecant (csc)"
       << setw(20) << "11. Secant (sec)" << setw(20) << "12. Cotangent (cot)"
       << endl;
  cout << setw(20) << "13. arcsin" << setw(20) << "14. arccos" << setw(20)
       << "15. arctan" << setw(20) << "16. arccsc" << endl;
  cout << setw(20) << "17. arcsec" << setw(20) << "18. arccot" << setw(20)
       << "19. Logarithm (log)" << setw(20) << "20. Natural Logarithm (ln)"
       << endl;
  cout << right << setw(40) << "0. Exit" << endl;
}
// Function for addition of two numbers
double addition(double a, double b) { return a + b; }

// Function for subtraction of two numbers
double difference(double a, double b) { return a - b; }

// Function for multiplication of two numbers
double multiplication(double a, double b) { return a * b; }

// Function for division of two numbers, includes error handling for division by
// zero
double division(double a, double b) {
  try {
    if (b == 0) {
      throw runtime_error("division by zero");
    }
    return a / b;
  } catch (const runtime_error &e) {
    cout << "Error: division by zero is not allowed." << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating the power of a number
double Exponential(double a, double b) { return pow(a, b); }

// Function for calculating the square root of a number
double square_root(double a) {
  if (a >= 0) {
    return sqrt(a);
  } else {
    cout << "Invalid input: negative numbers cannot have square roots." << endl;
  }
  return 1; // Return 1 as a fallback value for invalid input
}

// Function for calculating sine of an angle (in radians)
double sine(double a) { return sin(a); }

// Function for calculating cosine of an angle (in radians)
double cosine(double a) { return cos(a); }

// Function for calculating tangent of an angle (in radians)
double tangent(double a) { return tan(a); }

// Function for calculating cosecant of an angle (in radians)
double cosecant(double a) {
  if (sin(a) != 0) {
    return 1 / sin(a);
  } else {
    cout << "Invalid input: Cosecant is undefined for this value." << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating secant of an angle (in radians)
double secant(double a) {
  if (cos(a) != 0) {
    return 1 / cos(a);
  } else {
    cout << "Invalid input: Secant is undefined for this value." << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating cotangent of an angle (in radians)
double cotangent(double a) {
  if (tan(a) != 0) {
    return 1 / tan(a);
  } else {
    cout << "Invalid input: Cotangent is undefined for this value." << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating the logarithm of a number with a given base
double logarithmic(double a, double b) {
  if (a > 0 && b > 0 && b != 1) {
    return log(a) / log(b);
  } else {
    cout << "Invalid inputs: The values must be positive and the base cannot "
            "be 1."
         << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating the natural logarithm of a number (base e)
double natural_logarithmic(double a) {
  double e = 2.71828;
  if (a > 0) {
    return log(a) / log(e);
  } else {
    cout << "Invalid input: The value must be positive." << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating arcsine (inverse sine) of a value
double arcsine(double a) {
  if (a <= 1 && a >= -1) {
    return 57.3 * asin(a); // Convert from radians to degrees
  } else {
    cout << "Invalid input: arcsine is defined only for values in the range "
            "[-1, 1]."
         << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating arccosine (inverse cosine) of a value
double arccosine(double a) {
  if (a <= 1 && a >= -1) {
    return 57.3 * acos(a); // Convert from radians to degrees
  } else {
    cout << "Invalid input: arccosine is defined only for values in the range "
            "[-1, 1]."
         << endl;
  }
  return 1; // Return 1 as a fallback value
}

// Function for calculating arctangent (inverse tangent) of a value
double arctangent(double a) {
  return 57.3 * atan(a); // Convert from radians to degrees
}

