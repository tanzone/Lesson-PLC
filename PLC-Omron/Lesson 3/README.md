Welcome to Lesson 3 on Omron PLC programming using ladder logic. In this lesson, we will cover data manipulation instructions and functions.

Let's start by creating a program that uses the MOV instruction. The MOV instruction is used to move a value from one memory location to another. We will use memory locations D0 and D1 for this example.
```c
MOV #10, D0     ; Move value 10 to memory location D0
MOV D0, D1      ; Move value in D0 to memory location D1
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "MOV" instruction moves the value 10 to memory location D0. The next "MOV" instruction then moves the value in memory location D0 to memory location D1. Finally, the output signal is turned on.

Next, let's create a program that uses the ADD instruction. The ADD instruction is used to add two values together. We will use memory locations D0 and D1 for this example.
```c
MOV #10, D0     ; Move value 10 to memory location D0
MOV #20, D1     ; Move value 20 to memory location D1
ADD D0, D1      ; Add values in D0 and D1
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "ADD" instruction adds the values in memory locations D0 and D1 together. The output signal is turned on, which represents the result of the addition.

Finally, let's create a program that uses the CMP function. The CMP function is used to compare two values and determine which is greater. We will use memory locations D0 and D1 for this example.
```c
MOV #10, D0     ; Move value 10 to memory location D0
MOV #20, D1     ; Move value 20 to memory location D1
CMP D0, D1      ; Compare values in D0 and D1
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "CMP" function compares the values in memory locations D0 and D1. The output signal is turned on if the value in D1 is greater than the value in D0.

In conclusion, in this lesson, we have covered data manipulation instructions and functions using Omron PLCs. In the next lesson, we will cover how to use program control instructions and functions.
