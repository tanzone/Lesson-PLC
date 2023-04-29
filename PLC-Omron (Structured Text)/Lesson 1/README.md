In ST, we can use control structures such as "IF...THEN...ELSE" and "FOR...TO...DO" to create more complex programs. These structures allow us to control the flow of the program and execute specific actions based on certain conditions.

For example, the following ST program checks if variable "x" is greater than variable "y". If it is, it assigns the value of "x" to variable "z". Otherwise, it assigns the value of "y" to variable "z":
```c
VAR
    x : INT := 10;
    y : INT := 5;
    z : INT;
END_VAR

IF x > y THEN
    z := x;
ELSE
    z := y;
END_IF
```
In this example, we have used the "IF...THEN...ELSE" structure to check the condition "x > y". If this condition is true, we assign the value of "x" to "z". Otherwise, we assign the value of "y" to "z".

Another useful control structure in ST is the "FOR...TO...DO" loop. This loop allows us to execute a specific set of instructions multiple times, with a variable taking on different values each time.

For example, the following ST program uses a "FOR...TO...DO" loop to calculate the sum of the first 10 integers and store the result in variable "sum":
```c
VAR
    i : INT;
    sum : INT := 0;
END_VAR

FOR i := 1 TO 10 DO
    sum := sum + i;
END_FOR
```
In this example, we have used the "FOR...TO...DO" loop to iterate over the integers 1 through 10. During each iteration, we add the value of "i" to the "sum" variable. At the end of the loop, "sum" contains the sum of the first 10 integers.

In conclusion, in this lesson 1, we have introduced the "IF...THEN...ELSE" and "FOR...TO...DO" control structures in ST and shown how to use them to create more complex programs in Omron PLCs. In the next lessons, we will explore more advanced concepts in ST for PLC programming.
