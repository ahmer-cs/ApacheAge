# ApacheAge

# Arithmetic Expression Evaluation with Fibonacci Calculation

This program demonstrates arithmetic expression evaluation and Fibonacci calculation using a custom-defined expression tree. The program allows you to create arithmetic expressions using addition, subtraction, multiplication, division, absolute value, and Fibonacci function. It evaluates the expressions and provides the corresponding results.

## Features

- Supports addition, subtraction, multiplication, division, and absolute value operations.
- Calculates Fibonacci numbers using dynamic programming.
- Uses an expression tree data structure to represent the arithmetic expressions.
- Provides a function to calculate the value of a given expression tree.

## Requirements

- C compiler (supporting C99 standard)
- Standard C libraries: stdio.h, stdlib.h

## Usage

1. Clone the repository or download the source code files.

2. Compile the code using a C compiler:

    ```shell
    gcc arithmetic_expression.c -o arithmetic_expression
    ```

3. Run the compiled executable:

    ```shell
    ./arithmetic_expression
    ```

4. The program will output the evaluation results for the predefined arithmetic expressions.

## Code Explanation

- The `TypeTag` enum defines the types of nodes in the expression tree, including ADD, SUB, MUL, DIV, ABS, FIB, and LIT (literal).

- The `Node` struct represents a node in the expression tree. It contains the type of the node, a value (for LIT nodes), and pointers to the left and right child nodes.

- The `makeFunc` function creates a new node with the specified type and initializes its child pointers.

- The `makeValue` function creates a new literal node with the given value.

- The `fibonacci` function calculates the Fibonacci sequence using dynamic programming. It uses an array to store previously calculated Fibonacci numbers and avoids redundant calculations.

- The `calc` function recursively evaluates the expression tree and returns the result. It handles different node types and performs the corresponding operations.

- In the `main` function, predefined arithmetic expressions are created using the `makeFunc` and `makeValue` functions. The expressions are then evaluated using the `calc` function, and the results are printed to the console.

## Sample Output

add : 16
mul : 20
sub : -4
fibo : 2
