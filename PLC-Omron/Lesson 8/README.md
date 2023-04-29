Welcome to Lesson 8 on Omron PLC programming using ladder logic. In this lesson, we will cover timer and counter instructions and functions.

Timers and counters are used to measure time and count events in a process. Let's start with timers.
```c
TIM #100, T0        ; Set timer T0 to 100 milliseconds
SET T0              ; Start timer T0
MOV T0.EN, Y0.0     ; Output timer T0's enable bit to output Y0.0
```
In this program, the "TIM" instruction sets timer T0 to 100 milliseconds. The "SET" instruction starts timer T0. The "MOV" instruction moves timer T0's enable bit to output Y0.0. The output signal is turned on when the timer is enabled.

Next, let's move on to counters.
```c
CTU #100, C0        ; Set counter C0 to count up to 100
MOV C0.CU, Y0.0     ; Output counter C0's current count up value to output Y0.0
```
In this program, the "CTU" instruction sets counter C0 to count up to 100. The "MOV" instruction moves counter C0's current count up value to output Y0.0.

Finally, let's combine timers and counters in a program.
```c
TIM #100, T0        ; Set timer T0 to 100 milliseconds
SET T0              ; Start timer T0
MOV T0.EN, Y0.0     ; Output timer T0's enable bit to output Y0.0
CTU #10, C0         ; Set counter C0 to count up to 10
MOV C0.CU, Y0.1     ; Output counter C0's current count up value to output Y0.1
```
In this program, the "TIM" instruction sets timer T0 to 100 milliseconds. The "SET" instruction starts timer T0. The "MOV" instruction moves timer T0's enable bit to output Y0.0. The output signal is turned on when the timer is enabled. The "CTU" instruction sets counter C0 to count up to 10. The "MOV" instruction moves counter C0's current count up value to output Y0.1.

In conclusion, in this lesson, we have covered how to use timer and counter instructions and functions using Omron PLCs. In the next lesson, we will cover how to use comparison and arithmetic instructions and functions.
