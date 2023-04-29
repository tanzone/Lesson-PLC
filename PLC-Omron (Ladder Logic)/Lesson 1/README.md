Welcome to Lesson 1 on Omron PLC programming using ladder logic. In this lesson, we will dive deeper into ladder logic and start creating our first program.

To create a program in ladder logic, you will need to understand the basic elements of the language. Ladder logic consists of rungs, which are arranged horizontally, and contain instructions. Each instruction is represented by a symbol, and they can be combined to create complex programs.

Let's start by creating a simple program that turns on an output when an input is activated. We will use input X0.0 and output Y0.0 for this example.
```c
LD X0.0     ; Load input X0.0
OUT Y0.0    ; Output to output Y0.0
```
In this program, the "LD" instruction loads input X0.0, and the "OUT" instruction outputs to output Y0.0. When the input signal is on, the output signal will also turn on.

Next, let's create a program that turns on an output when two inputs are activated. We will use inputs X0.0 and X0.1, and output Y0.0 for this example.
```c
LD X0.0     ; Load input X0.0
AND         ; Combine with the next instruction
LD X0.1     ; Load input X0.1
OUT Y0.0    ; Output to output Y0.0
```
In this program, the "LD" instruction loads input X0.0, and the "AND" instruction combines it with the next instruction. The next instruction, "LD X0.1", loads input X0.1. If both inputs are active, the output signal will also turn on.

In conclusion, in this lesson, we have covered the basics of ladder logic and created our first programs using Omron PLCs. In the next lesson, we will cover more complex programs and how to use other instructions and functions.
