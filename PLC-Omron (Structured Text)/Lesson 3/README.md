In this lesson 3, we will continue to explore Structured Text (ST) programming for Omron PLCs.

One important concept in ST programming is the use of program organization units (POUs). POUs are reusable blocks of code that can be called from other parts of a program. They include function blocks, function declarations, and function calls.

Here is an example program that demonstrates the use of a function declaration and call:
```c
FUNCTION Add_Two_Numbers : INT
VAR_INPUT
    Num1 : INT;
    Num2 : INT;
END_VAR

VAR_OUTPUT
    Result : INT;
END_VAR

Result := Num1 + Num2;
Add_Two_Numbers := Result;
END_FUNCTION

VAR
    A : INT := 5;
    B : INT := 7;
    C : INT;
END_VAR

C := Add_Two_Numbers(Num1 := A, Num2 := B);
```
In this example, we have declared a function "Add_Two_Numbers" that takes two integer input parameters "Num1" and "Num2" and returns an integer output parameter "Result". The function adds the two input parameters together and assigns the result to the "Result" variable. It then returns the value of "Result" using the function name.

We then declare three integer variables "A", "B", and "C". We assign the values 5 and 7 to "A" and "B", respectively. We then call the "Add_Two_Numbers" function and pass in the values of "A" and "B" as input parameters. The function adds these values together and returns the result, which we assign to "C".

Another important concept in ST programming is the use of structures. A structure is a collection of variables of different types that are grouped together under a single name. We can access individual elements of a structure using dot notation.

Here is an example program that uses a structure to store information about a person and then displays that information on a screen:
```c
TYPE Person :
STRUCT
    Name : STRING(20);
    Age : INT;
    Height : REAL;
END_STRUCT
END_TYPE

VAR
    My_Person : Person := (Name := 'John', Age := 25, Height := 1.8);
END_VAR

// Display information on screen
```
In this example, we have declared a new data type "Person" using the "TYPE...STRUCT...END_STRUCT...END_TYPE" syntax. The "Person" data type contains three elements: a string variable "Name", an integer variable "Age", and a real variable "Height".

We then declare a variable "My_Person" of type "Person" and initialize it with values for the "Name", "Age", and "Height" elements using the dot notation.

We can access the values of the individual elements of the structure using the dot notation as well. For example, we can display the person's name on a screen by using "My_Person.Name".

In conclusion, in this lesson 3, we have explored the concepts of program organization units (POUs) and structures in ST programming for Omron PLCs. These concepts allow us to create more organized and structured programs. In the next lessons, we will continue to explore more advanced concepts in ST programming.
