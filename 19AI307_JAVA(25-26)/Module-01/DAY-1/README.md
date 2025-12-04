# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:

A shop keeper would like to welcome their customers with their name.

Write a java program to get name from the user (String) and print it.

Input Format:

A single line string input.

Output Format:

Hello, [name]

For example:

Input	: Ajeesh 
Result : Hello, Ajeesh


## AIM:

Write a java program to get name from the user (String) and print it.


## ALGORITHM :
```
1.Start the program.
2.Import the necessary package 'java.util'
3.Create a Scanner object to read input from the user.
4.Read a string input (the user's name).
5.Store the input in the variable name.
6.Display the message: "Hello, " + name
```



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

```
import java.util.*;
public class prog{
    public static void main(String[] args){
        Scanner sc= new Scanner(System.in);
        String name = sc.next();
        
        System.out.print("Hello, "+name);
    }
}
```



## OUTPUT:

<img width="669" height="242" alt="Screenshot 2025-11-19 104928" src="https://github.com/user-attachments/assets/fec616b3-c127-4715-a786-c3fc853b67b2" />


## RESULT:

Thus, the java program to get name from the user (String) and print it is executed successfully.



