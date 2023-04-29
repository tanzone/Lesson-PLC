In this lesson 8, we will continue our exploration of Structured Text (ST) programming for Omron PLCs.

Another important concept in ST programming is the use of functions and function blocks. Functions are pre-written blocks of code that perform a specific task and can be called from within a program. Function blocks are similar to functions, but are designed to work with input and output variables.

Here is an example program that uses a function block to calculate the average of three numbers:
```c
FUNCTION_BLOCK CalcAverage
VAR_INPUT
    Num1 : REAL;
    Num2 : REAL;
    Num3 : REAL;
END_VAR

VAR_OUTPUT
    Avg : REAL;
END_VAR

BEGIN
    Avg := (Num1 + Num2 + Num3) / 3;
END_FUNCTION_BLOCK
```
In this example, we have defined a function block called "CalcAverage". This function block takes three input variables, "Num1", "Num2", and "Num3", and calculates their average. The result is then stored in the output variable "Avg".

Here is an example program that uses a function to calculate the square of a number:
```c
FUNCTION Square : REAL
VAR_INPUT
    Num : REAL;
END_VAR

VAR_OUTPUT
    Result : REAL;
END_VAR

BEGIN
    Result := Num * Num;
END_FUNCTION
```
In this example, we have defined a function called "Square". This function takes one input variable, "Num", and calculates its square. The result is then stored in the output variable "Result".

In conclusion, in this lesson 8, we have explored the use of functions and function blocks in ST programming for Omron PLCs. Functions and function blocks allow us to create reusable code that can be used in multiple programs, increasing code efficiency and reducing errors. In the next lessons, we will continue to explore more advanced concepts in ST programming.
