In this lesson 9, we will continue our exploration of Structured Text (ST) programming for Omron PLCs.

Another important concept in ST programming is the use of structures. Structures allow us to group related variables together under a single name, making our code more organized and easier to read.

Here is an example program that uses a structure to store information about a person:
```c
TYPE Person :
STRUCT
    FirstName : STRING(30);
    LastName : STRING(30);
    Age : INT;
    Address : STRUCT
        Street : STRING(50);
        City : STRING(30);
        State : STRING(2);
        Zip : STRING(10);
    END_STRUCT
END_STRUCT
END_TYPE

PROGRAM Main
VAR
    MyPerson : Person;
END_VAR

BEGIN
    MyPerson.FirstName := "John";
    MyPerson.LastName := "Doe";
    MyPerson.Age := 30;
    MyPerson.Address.Street := "123 Main St";
    MyPerson.Address.City := "Anytown";
    MyPerson.Address.State := "CA";
    MyPerson.Address.Zip := "12345";
END_PROGRAM
```
In this example, we have defined a structure called "Person" that contains four variables: "FirstName", "LastName", "Age", and "Address". The "Address" variable is itself a structure that contains four variables: "Street", "City", "State", and "Zip".

We have then declared a variable "MyPerson" of type "Person" in the main program. We can then access the variables within the structure using dot notation, as shown in the example.

In conclusion, in this lesson 9, we have explored the use of structures in ST programming for Omron PLCs. Structures allow us to group related variables together under a single name, making our code more organized and easier to read. In the next lessons, we will continue to explore more advanced concepts in ST programming.
