Welcome to Lesson 5 on Omron PLC programming using ladder logic. In this lesson, we will cover timer and counter instructions and functions.

Let's start by creating a program that uses the timer instruction. The timer instruction is used to delay the execution of a block of instructions.
```c
TON 5.00, 1000, 200   ; Timer on delay for 1 second, memory location D200
MOV #1, D0            ; Move value 1 to memory location D0
OUT Y0.0              ; Output to output Y0.0
```
In this program, the "TON" instruction sets a timer with a delay of 1 second and stores the timer status in memory location D200. The next instruction moves the value 1 to memory location D0, and the output signal is turned on. The program will wait for 1 second before executing the instructions after the "TON" instruction.

Next, let's create a program that uses the counter instruction. The counter instruction is used to count the number of times a signal is inputted.
```c
CTU C0, 10, D0    ; Counter up for 10 counts, memory location D0
CMP #10, D0       ; Compare memory location D0 to value 10
JEQ 10            ; Jump to program step 10 if the comparison is equal
OUT Y0.0          ; Output to output Y0.0
```
In this program, the "CTU" instruction sets a counter that counts up to 10 and stores the count value in memory location D0. The "CMP" instruction compares the value in memory location D0 to the value 10. If the comparison is equal, the "JEQ" instruction jumps to program step 10. If the comparison is not equal, the output signal is turned on.

Finally, let's create a program that uses both timer and counter instructions.
```c
CTU C0, 10, D0        ; Counter up for 10 counts, memory location D0
TON 5.00, 1000, D200  ; Timer on delay for 1 second, memory location D200
CMP #10, D0           ; Compare memory location D0 to value 10
JEQ 10                ; Jump to program step 10 if the comparison is equal
OUT Y0.0              ; Output to output Y0.0

LBL 10                ; Define label for subroutine
MOV #2, D0            ; Move value 2 to memory location D0
RET                   ; Return to main program
```
In this program, the "CTU" instruction sets a counter that counts up to 10 and stores the count value in memory location D0. The "TON" instruction sets a timer with a delay of 1 second and stores the timer status in memory location D200. The "CMP" instruction compares the value in memory location D0 to the value 10. If the comparison is equal, the "JEQ" instruction jumps to program step 10. If the comparison is not equal, the output signal is turned on. The subroutine at program step 10 moves the value 2 to memory location D0 and then returns to the main program.

In conclusion, in this lesson, we have covered how to use timer and counter instructions and functions using Omron PLCs. In the next lesson, we will cover how to use mathematical and logical instructions and functions.
