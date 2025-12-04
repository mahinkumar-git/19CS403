# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A dragon wakes based on temperature:

If temperature < 0, it hibernates.
If 0 ≤ temp ≤ 20, it snoozes.
If 21 ≤ temp ≤ 35, it wakes.
If temp > 35, it gets angry.

Write a java program to get the user input for temperature and display appropriate output.

For example:

Input	: -5
Result : Hibernating


## AIM:

To write a java program to get the user input for temperature and display appropriate output.


## ALGORITHM :
```
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4.Read an integer value and store it in the variable temp.
5.Check if temp < 0 : If true, print "Hibernating".
6.Else if temp is between 0 and 20 (inclusive) : Print "Snoozing".
7.Else if temp is between 21 and 35 (inclusive): Print "Awake".
8. Else (i.e., temp > 35): Print "Angry".
```




## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int temp=sc.nextInt();
        if(temp<0){
            System.out.println("Hibernating");
        }
        else if(temp>=0 && temp <=20){
            System.out.println("Snoozing");
        }
        else if(temp >=21 && temp <=35){
            System.out.println("Awake");
        }
        else{
            System.out.println("Angry");
        }
    }
}
```


## OUTPUT:

<img width="652" height="366" alt="image" src="https://github.com/user-attachments/assets/e3ad52a9-af69-45f5-98d7-07fddccacb65" />


## RESULT:

Thus, a java program to get the user input for temperature and display appropriate output is executed successfully.
