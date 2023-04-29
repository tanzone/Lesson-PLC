Welcome to Lesson 7 on Omron PLC programming using ladder logic. In this lesson, we will cover data manipulation instructions and functions.

Let's start by creating a program that uses a data manipulation instruction. Data manipulation instructions are used to manipulate data in memory.
```c
MOV #1, D0       ; Move value 1 to memory location D0
MOV #0, D1       ; Move value 0 to memory location D1
XOR D0, D1, D2   ; Exclusive OR operation between memory locations D0 and D1, result stored in memory location D2
OUT Y0.0         ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 1 to memory location D0 and the value 0 to memory location D1. The "XOR" instruction performs an exclusive OR operation between the values in memory locations D0 and D1, and the result is stored in memory location D2. The output signal is turned on.

Next, let's create a program that uses a data manipulation function. Data manipulation functions are used to manipulate data in memory.
```c
BSET D0, #4     ; Set the fourth bit of memory location D0
BCLR D0, #2     ; Clear the second bit of memory location D0
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "BSET" instruction sets the fourth bit of memory location D0, and the "BCLR" instruction clears the second bit of memory location D0. The output signal is turned on.

Finally, let's create a program that uses both data manipulation instructions and functions.
```c
MOV #10, D0     ; Move value 10 to memory location D0
ADD #5, D0      ; Add value 5 to the value in memory location D0
MOV D0, D1      ; Move the value in memory location D0 to memory location D1
BSET D1, #3     ; Set the third bit of memory location D1
BCLR D1, #1     ; Clear the first bit of memory location D1
CMP #15, D1     ; Compare memory location D1 to value 15
JGE 10          ; Jump to program step 10 if the comparison is greater than or equal to
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 to memory location D0, the "ADD" instruction adds the value 5 to the value in memory location D0, and the "MOV" instruction moves the value in memory location D0 to memory location D1. The "BSET" instruction sets the third bit of memory location D1, and the "BCLR" instruction clears the first bit of memory location D1. The "CMP" instruction compares the value in memory location D1 to the value 15. If the comparison is greater than or equal to 15, the "JGE" instruction jumps to program step 10. If the comparison is less than 15, the output signal is turned on.

In conclusion, in this lesson, we have covered how to use data manipulation instructions and functions using Omron PLCs. In the next lesson, we will cover how to use timer and counter instructions and functions.
