# Calculator Project

## Overview
This project is a simple command-line calculator that can evaluate mathematical expressions using basic arithmetic operations. It supports addition, subtraction, multiplication, division, modulus, and exponentiation. The calculator uses the shunting yard algorithm to convert infix expressions (like `3 + 4 * 2`) to postfix notation (Reverse Polish Notation, RPN) and then evaluates the result.

## Features
- **Basic Operations**: Addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), modulus (`%`), and exponentiation (`^`).
- **Operator Precedence**: Correctly handles operator precedence and associativity.
- **Parentheses Support**: Allows the use of parentheses to group expressions.

## How It Works
1. **Shunting Yard Algorithm**: Converts the input expression from infix to postfix notation.
2. **RPN Evaluation**: The postfix expression is evaluated using a stack to compute the final result.

## Files
- **calculator.c**: Contains the implementation of the stack, queue, shunting yard algorithm, and RPN evaluation.
- **calculator.h**: Declares the data structures and functions used in `calculator.c`.
- **main.c**: The entry point of the program. It handles user input and utilizes the functions from `calculator.c` to process and evaluate the expression.

## How to Compile and Run
1. **Compilation**:
   ```bash
   gcc -o calculator main.c calculator.c
   ```
2. **Run the Program**:
   ```bash
   ./calculator
   ```

## Example Usage
- Input: `3 + 4 * 2 / ( 1 - 5 ) ^ 2 ^ 3`
- Output: The program will process this expression and display the result.

## License
This project is licensed under the MIT License.
