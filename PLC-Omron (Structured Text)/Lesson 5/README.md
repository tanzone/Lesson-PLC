In this lesson 5, we will continue our exploration of Structured Text (ST) programming for Omron PLCs.

Another important concept in ST programming is the use of functions. A function is a block of code that performs a specific task and returns a value to the calling program. We can declare our own functions or use built-in functions provided by the PLC manufacturer.

Here is an example program that demonstrates the use of a built-in function:
```c
VAR
    Num : INT := 5;
    Sqrt : REAL;
END_VAR

Sqrt := SQRT(Num);
```
In this example, we have declared an integer variable "Num" and initialized it with the value 5. We also declared a real variable "Sqrt". We then use the built-in "SQRT" function to calculate the square root of "Num" and assign the result to "Sqrt".

We can also declare our own functions using the "FUNCTION" and "END_FUNCTION" keywords. Here is an example program that declares a function to calculate the average of two numbers:
```c
FUNCTION Calc_Avg : REAL
VAR_INPUT
    Num1 : REAL;
    Num2 : REAL;
END_VAR
VAR_OUTPUT
    Result : REAL;
END_VAR

Result := (Num1 + Num2) / 2;

END_FUNCTION
```
In this example, we have declared a function called "Calc_Avg" that takes two real numbers as input and returns the average as a real number. We declare the input variables using the "VAR_INPUT" keyword and the output variable using the "VAR_OUTPUT" keyword. Inside the function, we calculate the average using the formula "(Num1 + Num2) / 2" and assign the result to "Result".

We can then call this function from other parts of our program, like this:
```c
VAR
    Num1 : REAL := 5.5;
    Num2 : REAL := 7.8;
    Avg : REAL;
END_VAR

Avg := Calc_Avg(Num1, Num2);
```
In this example, we have declared two real variables "Num1" and "Num2" and initialized them with the values 5.5 and 7.8, respectively. We also declare a real variable "Avg". We then call the "Calc_Avg" function with the arguments "Num1" and "Num2" and assign the result to "Avg".

In conclusion, in this lesson 5, we have explored the concept of functions in ST programming for Omron PLCs. Functions allow us to create reusable blocks of code that perform specific tasks, making our programs more efficient and easier to maintain. In the next lessons, we will continue to explore more advanced concepts in ST programming.
