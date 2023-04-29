In this lesson 0, we will introduce the basic concepts of ST and how to use this language to program an Omron PLC.

In ST, the syntax of the language is similar to that of C. We can declare variables and use mathematical and logical operations to create complex programs.

For example, to declare a variable in ST, we use the following format:
```c
VAR
    variable_name : data_type;
END_VAR
```
Where "variable_name" is the name we choose for our variable and "data_type" is the type of data we want to use.

For example, we can declare an integer variable in ST as follows:
```c
VAR
    x : INT;
END_VAR
```
In ST, we can use arithmetic operators such as "+", "-", "*", "/", and logical operators such as "AND", "OR", "NOT" to create complex expressions.

For example, the following ST program assigns the value of the sum between variables "x" and "z" to variable "y":
```c
VAR
    x : INT := 10;
    y : INT;
    z : INT := 5;
END_VAR

y := x + z;
```
In this example, we have declared variables "x", "y" and "z" as integer variables and assigned them values. We have then used the "+" operator to calculate the sum between variables "x" and "z" and assigned the result to variable "y".

In conclusion, in this lesson 0, we have introduced the basic concepts of ST and shown how to use it to program an Omron PLC. In the next lessons, we will further explore the capabilities of ST for PLC programming.
