# Credit-Card-Validator

A Credit Card Validator in C++ is a software program that uses the Luhn Algorithm, a simple checksum formula, to validate the integrity of a variety of identification numbers, especially credit card numbers. Our program asks for a credit card number as input and validates the number based on its length, the identity of the issuer (like Visa, MasterCard, or American Express), and the results of the Luhn Algorithm.

Introduction

The Credit Card Validator in C++ is particularly useful to prevent typos or simple input errors when a user is asked to enter their credit card number in a software system. Please note that while this program can confirm whether a credit card number is theoretically valid, it doesn’t check if the card number is actually issued or in use, which would require access to the issuer’s database.

Objective

We are developing the Credit Card Validator in C++ project to achieve the following objectives:
1. To check if the credit card number is valid or not.
2. To check for the type of credit card being used.
   
Requirements

1. Knowledge of C++ Programming. In particular, an understanding of the standard library functions used in this program (such as cin, cout, strcpy, etc.) is required.
2. C++ Compiler: The GCC (GNU Compiler Collection) is a common compiler used for C++ and is available on most platforms. For Windows, the MinGW compiler is widely used. For macOS, Xcode’s Command Line Tools include a suitable compiler.
3. Integrated Development Environment (IDE): We have used Visual Studio Code. You can use other IDEs like Code::Blocks, Eclipse, Visual Studio Code, and CLion.
4. Understanding of the Luhn Algorithm: This program uses the Luhn algorithm to validate credit card numbers. A basic understanding of this algorithm is necessary to understand and modify this code.

   Explanation of Code
   
1. Firstly we have included the C++ Standard Libraries needed for the program #include<bits/stdc++.h>, #include <stdio.h>, #include <iostream>, #include <string>, and #include<string>. These libraries provide functionality such as input/output operations, string manipulation, etc.
2. using namespace std: This line allows for using objects and variables in the standard namespace without having to prefix “std” before every use.
3. After that, the main function begins in which we declare variables
creditnum – to store the credit card number
sum – the sum of digits according to the Luhn algorithm
count1 – count of digits in the number
divisor – to find the first and first two digits of the card, and
types – the type of the card
4. A do-while loop prompts the user to enter a credit card number until a positive number is entered.
5. Two while loops apply the Luhn algorithm to the card number, storing the result in sum. Another while loop counts the number of digits in the card number.
6. A for loop calculates the divisor needed to find the first and first two digits of the card number.
7. If the sum is a multiple of 10 (as per Luhn’s algorithm), nested if statements check the first digit or first two digits and the length of the card number to determine the card type.
8. If the sum is not a multiple of 10, the card is deemed invalid.
9. The type of the card or “INVALID” is printed, depending on the validity of the card number.
10. The main function ends successfully with return 0.

Conclusion

Hence we have successfully developed a Credit Card Validator in C++ project that identifies whether the credit card number is valid or not and the credit card type. In our project, we worked with the Luhn algorithm to satisfy the conditions. This project helps to prevent the fraudulent activities raised in the Cyber site. You can use other algorithms to meet your requirements.
