In this lesson 2, we will explore more advanced concepts in Structured Text (ST) programming for Omron PLCs.

One important concept in ST programming is the use of functions and function blocks. A function is a reusable piece of code that performs a specific task. A function block is a collection of functions that work together to perform a larger task.

For example, Omron PLCs come with pre-built function blocks that perform tasks such as counting, timing, and comparing values. These function blocks can be used in our programs by calling them and passing in the necessary parameters.

Here is an example program that uses the built-in counter function block in Omron PLCs:
```c
VAR
    Counter : COUNTER;
    Count_Value : INT;
END_VAR

Counter(CLK := true);
Count_Value := Counter.CV;
```
In this example, we have declared a counter variable "Counter" of type COUNTER and an integer variable "Count_Value". We then call the "Counter" function block and pass in the "CLK" parameter with a value of true. This tells the function block to increment the counter.

After calling the function block, we retrieve the current value of the counter by accessing the "CV" property of the "Counter" variable and assign it to the "Count_Value" variable.

Another important concept in ST programming is the use of arrays. An array is a collection of values of the same type. We can access individual elements of an array using an index.

Here is an example program that uses an array to store 10 integer values and then displays them on a screen:
```c
VAR
    Values : ARRAY[0..9] OF INT := [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    i : INT;
END_VAR

FOR i := 0 TO 9 DO
    // Display value on screen
END_FOR
```
In this example, we have declared an array "Values" of size 10 and initialized it with the values 1 through 10. We have also declared an integer variable "i" to use as the array index.

We then use a "FOR...TO...DO" loop to iterate over the elements of the array and display them on a screen. We can access the value of each element using the array index "i".

In conclusion, in this lesson 2, we have explored more advanced concepts in ST programming for Omron PLCs, including functions and function blocks, as well as arrays. These concepts allow us to create more complex and powerful programs. In the next lessons, we will continue to explore more advanced concepts in ST programming.
