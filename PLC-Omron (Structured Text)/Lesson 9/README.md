Welcome to Lesson 9 on Omron PLC programming using ladder logic. In this lesson, we will cover comparison and arithmetic instructions and functions.

Comparison instructions are used to compare values in a program. Let's start with the "EQU" instruction.
```c
MOV #10, D0         ; Move the value 10 into D0
EQU D0, #10         ; Compare the value in D0 with the value 10
MOV EQU, Y0.0       ; Output the result of the comparison to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 into D0. The "EQU" instruction compares the value in D0 with the value 10. The "MOV" instruction moves the result of the comparison to output Y0.0.

Next, let's move on to arithmetic instructions.
```c
MOV #10, D0         ; Move the value 10 into D0
ADD #5, D0          ; Add the value 5 to the value in D0
MOV D0, Y0.0        ; Output the result of the addition to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 into D0. The "ADD" instruction adds the value 5 to the value in D0. The "MOV" instruction moves the result of the addition to output Y0.0.

Finally, let's combine comparison and arithmetic instructions in a program.
```c
MOV #10, D0         ; Move the value 10 into D0
ADD #5, D0          ; Add the value 5 to the value in D0
EQU D0, #15         ; Compare the value in D0 with the value 15
MOV EQU, Y0.0       ; Output the result of the comparison to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 into D0. The "ADD" instruction adds the value 5 to the value in D0. The "EQU" instruction compares the value in D0 with the value 15. The "MOV" instruction moves the result of the comparison to output Y0.0.

In conclusion, in this lesson, we have covered how to use comparison and arithmetic instructions and functions using Omron PLCs. In the next lesson, we will cover how to use branch instructions and functions.
