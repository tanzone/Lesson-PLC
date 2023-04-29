Welcome to Lesson 2 on Omron PLC programming using ladder logic. In this lesson, we will cover more complex programs and introduce you to some new instructions and functions.

Let's start by creating a program that uses a timer. A timer is used to delay an output signal for a certain amount of time. We will use input X0.0 and output Y0.0 for this example.
```c
LD X0.0         ; Load input X0.0
TON T0          ; Timer on delay T0
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "TON" instruction turns on timer T0 when input X0.0 is activated. The timer will delay for a set amount of time before the output signal is turned on.

Next, let's create a program that uses a counter. A counter is used to count the number of times an input signal is activated. We will use input X0.0 and output Y0.0 for this example.
```c
LD X0.0         ; Load input X0.0
CTU C0, 10      ; Counter up C0 to 10
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "CTU" instruction counts up counter C0 every time input X0.0 is activated. The counter will count up to 10 before the output signal is turned on.

Finally, let's create a program that uses a comparison instruction. A comparison instruction is used to compare two values and determine if they are equal or not. We will use input X0.0 and X0.1 for this example.
```c
LD X0.0         ; Load input X0.0
EQ X0.1         ; Equal to input X0.1
OUT Y0.0        ; Output to output Y0.0
```
In this program, the "EQ" instruction compares input X0.0 to input X0.1. If they are equal, the output signal will be turned on.

In conclusion, in this lesson, we have covered more complex programs using Omron PLCs and introduced you to new instructions and functions. In the next lesson, we will cover how to use data manipulation instructions and functions.
