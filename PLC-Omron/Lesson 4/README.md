Welcome to Lesson 4 on Omron PLC programming using ladder logic. In this lesson, we will cover program control instructions and functions.

Let's start by creating a program that uses the JMP instruction. The JMP instruction is used to jump to a specific program step. We will use program steps 10 and 20 for this example.
```c
JMP 10          ; Jump to program step 10
MOV #1, D0      ; Move value 1 to memory location D0
JMP 20          ; Jump to program step 20
MOV #2, D0      ; Move value 2 to memory location D0
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "JMP" instruction jumps to program step 10. The next instruction moves the value 1 to memory location D0. The "JMP" instruction then jumps to program step 20, skipping the instruction that moves the value 2 to memory location D0. Finally, the output signal is turned on.

Next, let's create a program that uses the LBL and RET instructions. The LBL instruction is used to define a label in the program. The RET instruction is used to return to the main program after a subroutine is completed.
```c
LBL 10          ; Define label for subroutine
MOV #1, D0      ; Move value 1 to memory location D0
JSR 20          ; Jump to subroutine at label 20
OUT Y0.0        ; Output to output Y0.0

LBL 20          ; Define label for subroutine
MOV #2, D0      ; Move value 2 to memory location D0
RET             ; Return to main program
```
In this program, the "LBL" instruction defines a label for a subroutine at program step 10. The next instruction moves the value 1 to memory location D0. The "JSR" instruction jumps to the subroutine at label 20. The "MOV" instruction in the subroutine moves the value 2 to memory location D0. The "RET" instruction returns to the main program at the instruction following the "JSR" instruction. Finally, the output signal is turned on.

Finally, let's create a program that uses the FOR instruction. The FOR instruction is used to execute a block of instructions a certain number of times.
```c
FOR #0, #10, #1 DO  ; Execute loop 10 times
    MOV #1, D0      ; Move value 1 to memory location D0
    OUT Y0.0        ; Output to output Y0.0
NEXT                ; End of loop
```
In this program, the "FOR" instruction executes the instructions within the loop 10 times. The "MOV" instruction moves the value 1 to memory location D0, and the output signal is turned on. The "NEXT" instruction marks the end of the loop.

In conclusion, in this lesson, we have covered program control instructions and functions using Omron PLCs. In the next lesson, we will cover how to use timer and counter instructions and functions.
