Welcome to Lesson 6 on Omron PLC programming using ladder logic. In this lesson, we will cover mathematical and logical instructions and functions.

Let's start by creating a program that uses a mathematical instruction. Mathematical instructions are used to perform arithmetic operations on data.
```c
MOV #5, D0      ; Move value 5 to memory location D0
ADD #3, D0      ; Add value 3 to the value in memory location D0
DIV #2, D0      ; Divide the value in memory location D0 by 2
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 5 to memory location D0. The "ADD" instruction adds the value 3 to the value in memory location D0. The "DIV" instruction divides the value in memory location D0 by 2, and the output signal is turned on.

Next, let's create a program that uses a logical instruction. Logical instructions are used to perform logical operations on data.
```c
MOV #1, D0       ; Move value 1 to memory location D0
MOV #0, D1       ; Move value 0 to memory location D1
AND D0, D1, D2   ; Logical AND operation between memory locations D0 and D1, result stored in memory location D2
OUT Y0.0         ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 1 to memory location D0 and the value 0 to memory location D1. The "AND" instruction performs a logical AND operation between the values in memory locations D0 and D1, and the result is stored in memory location D2. The output signal is turned on.

Finally, let's create a program that uses both mathematical and logical instructions.
```c
MOV #10, D0     ; Move value 10 to memory location D0
SUB #3, D0      ; Subtract value 3 from the value in memory location D0
CMP #5, D0      ; Compare memory location D0 to value 5
JGE 10          ; Jump to program step 10 if the comparison is greater than or equal to
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 to memory location D0. The "SUB" instruction subtracts the value 3 from the value in memory location D0. The "CMP" instruction compares the value in memory location D0 to the value 5. If the comparison is greater than or equal to 5, the "JGE" instruction jumps to program step 10. If the comparison is less than 5, the output signal is turned on.

In conclusion, in this lesson, we have covered how to use mathematical and logical instructions and functions using Omron PLCs. In the next lesson, we will cover how to use data manipulation instructions and functions.
