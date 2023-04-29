In this lesson 7, we will continue our exploration of Structured Text (ST) programming for Omron PLCs.

One important concept in ST programming is the use of loops. Loops allow us to repeat a block of code a certain number of times or until a certain condition is met. There are two types of loops in ST programming: the "for" loop and the "while" loop.

Here is an example program that uses a "for" loop to calculate the sum of the first 10 integers:
```c
VAR
    Sum : INT := 0;
    i : INT;
END_VAR

FOR i := 1 TO 10 DO
    Sum := Sum + i;
END_FOR
```
In this example, we have declared an integer variable "Sum" and initialized it with the value 0. We have also declared an integer variable "i". We then use a "for" loop to iterate from 1 to 10, adding each value of "i" to "Sum" until the loop is complete.

Here is an example program that uses a "while" loop to calculate the factorial of a number:
```c
VAR
    Num : INT := 5;
    Fact : INT := 1;
    i : INT := 1;
END_VAR

WHILE i <= Num DO
    Fact := Fact * i;
    i := i + 1;
END_WHILE
```
In this example, we have declared an integer variable "Num" and initialized it with the value 5. We have also declared an integer variable "Fact" and initialized it with the value 1. We have also declared an integer variable "i" and initialized it with the value 1. We then use a "while" loop to iterate from 1 to "Num", multiplying each value of "i" by "Fact" until the loop is complete.

In conclusion, in this lesson 7, we have explored the use of loops in ST programming for Omron PLCs. Loops allow us to perform repetitive tasks more efficiently and with less code. In the next lessons, we will continue to explore more advanced concepts in ST programming.
