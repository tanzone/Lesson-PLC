In this lesson 6, we will continue our exploration of Structured Text (ST) programming for Omron PLCs.

Another important concept in ST programming is the use of arrays. An array is a collection of variables of the same data type that are accessed using an index. We can declare arrays of different data types, including integer, real, and boolean.

Here is an example program that demonstrates the use of an integer array:
```c
VAR
    Temp : ARRAY[1..4] OF INT := [20, 25, 30, 35];
    i : INT := 2;
    Val : INT;
END_VAR

Val := Temp[i];
```
In this example, we have declared an integer array called "Temp" with four elements, initialized with the values 20, 25, 30, and 35. We have also declared an integer variable "i" and initialized it with the value 2. We then use "i" as an index to access the second element of the "Temp" array and assign the value to "Val".

We can also declare multidimensional arrays, which are arrays with more than one index. Here is an example program that declares a 2D real array:
```c
VAR
    Data : ARRAY[1..3, 1..4] OF REAL;
    Row : INT := 2;
    Col : INT := 3;
    Val : REAL := 2.5;
END_VAR

Data[Row, Col] := Val;
```
In this example, we have declared a 2D real array called "Data" with 3 rows and 4 columns. We have also declared two integer variables "Row" and "Col" and initialized them with the values 2 and 3, respectively. We have also declared a real variable "Val" and initialized it with the value 2.5. We then use "Row" and "Col" as indices to access the element in the second row and third column of the "Data" array and assign the value "Val" to it.

In conclusion, in this lesson 6, we have explored the concept of arrays in ST programming for Omron PLCs. Arrays allow us to store and access multiple values of the same data type using a single variable name, making our programs more efficient and easier to read. In the next lessons, we will continue to explore more advanced concepts in ST programming.
