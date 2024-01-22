# CreditCardValidator
Basic C++ code to validate a Credit Card Number.

A credit card validator is an application or a software that verifies the authenticity and validity of credit card numbers. This software uses a mathematical algorithm, known as the Luhn algorithm, to determine whether a credit card number is valid or not.
A credit card validator can be used for several purposes, including fraud prevention, chargeback reduction, and proper billing. Credit card validators are used by merchants and financial institutions to protect themselves against fraudulent transactions and to verify that they only accept authentic credit card payments. We will be creating a credit card validator using C++ programming language.

How does the Luhn Algorithm work?
The Luhn algorithm works by checking the sum of the digits of a credit card number against a predefined formula. The Luhn algorithm, also known as the "Modulus 10 Algorithm", is a mathematical formula that determines if an identification number is accurate. If the sum of the digits meets the formula requirements, then the number is considered valid. However, if the sum of the digits does not meet the formula requirements, then the number is considered invalid.

Overview of the UI:
This program uses the Luhn Algorithm to validate a CC number.
You can enter ‘exit’ anytime to quit.
Please enter a CC number to validate:
The user will enter a Credit card number. If according to the Luhn algorithm, the CC number is valid, then the program will display ‘valid’ else ‘invalid’.


The Luhn Algorithm works as follows:

Step 1 is to double every second digit, starting from the right. If it results in a two-digit number, add both digits to obtain a single-digit number. Finally, sum all the answers to obtain ‘doubleEvenSum’.
For this step we will create a for loop and implement the Luhn algorithm by looping over the credit card number’s digits, starting from the rightmost digit. The loop doubles every second digit and adds the result to a variable called ‘doubleEvenSum’.

Step 2 is to add every oddly placed digit from the right to the value ‘doubleEvenSum’.
We will create another for loop. This loop will add all the odd-placed digits to ‘doubleEvenSum’. It will check if ‘doubleEvenSum’ is a multiple of 10 and outputs the result (either “Valid!” or “Invalid!”).
