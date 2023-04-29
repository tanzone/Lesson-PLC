
In this lesson 4, we will continue to explore Structured Text (ST) programming for Omron PLCs.

One important concept in ST programming is the use of arrays. An array is a collection of variables of the same type that are grouped together under a single name and accessed using an index. We can declare arrays of any of the basic data types, such as integers, reals, and booleans.

Here is an example program that demonstrates the use of an array:
```c
VAR
    My_Array : ARRAY[0..4] OF INT := [1, 2, 3, 4, 5];
    i : INT;
END_VAR

FOR i := 0 TO 4 DO
    My_Array[i] := My_Array[i] * 2;
END_FOR
```
In this example, we have declared an array "My_Array" of type integer with 5 elements using the "ARRAY[0..4] OF INT" syntax. We initialize the array with the values 1, 2, 3, 4, and 5 using the bracket notation.

We then declare an integer variable "i". We use a "FOR" loop to iterate through the array elements using the index "i". Inside the loop, we multiply each array element by 2 and assign the result back to the same element.

Another important concept in ST programming is the use of conditional statements. A conditional statement allows us to execute different code depending on whether a certain condition is true or false. The two most common types of conditional statements are "IF" statements and "CASE" statements.

Here is an example program that uses an "IF" statement to determine whether a number is positive, negative, or zero:
```c
VAR
    Num : INT := -5;
END_VAR

IF Num > 0 THEN
    // Number is positive
ELSIF Num < 0 THEN
    // Number is negative
ELSE
    // Number is zero
END_IF
```
In this example, we have declared an integer variable "Num" and initialized it with the value -5. We use an "IF" statement to check whether "Num" is greater than 0, less than 0, or equal to 0. Depending on the result of the comparison, we execute different code using the "THEN", "ELSIF", and "ELSE" keywords.

In conclusion, in this lesson 4, we have explored the concepts of arrays and conditional statements in ST programming for Omron PLCs. These concepts allow us to create more flexible and powerful programs. In the next lessons, we will continue to explore more advanced concepts in ST programming.
