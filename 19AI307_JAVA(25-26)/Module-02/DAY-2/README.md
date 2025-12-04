# Ex.No:2(B) METHODS

## QUESTION:
Write a method void modifyValue(int num) that tries to modify the passed value(add passed value with 10) and print "Inside method: "+num . 

Show in main() that the original value does not change.

After calling modifyValue(int num) method in main , print the "Outside method: "+num

## AIM:
To write a Java program that demonstrates how primitive data is passed by value in methods.

## ALGORITHM :
1.	Define a method modifyValue(int num) that adds 10 to num and prints it.
2.	In main(), declare num and assign a value (e.g., 20).
3.	Call modifyValue(num) to show modification inside the method.
4.	Print the value of num outside the method to show it remains unchanged.
5.	End the program.





## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog {
    public static void modifyValue(int num) {
        num = num + 10;
        System.out.println("Inside method: " + num);
    }

    public static void main(String[] args) {
 Scanner sc = new Scanner(System.in);
        int x = sc.nextInt();
        modifyValue(x);
        System.out.println("Outside method: " + x);
    }
}
```






## OUTPUT:
<img width="1154" height="333" alt="image" src="https://github.com/user-attachments/assets/64a2d168-cfd2-4e7e-b763-c56f18422db9" />



## RESULT:
The program successfully shows that primitive data types in Java are passed by value, so changes inside the method don’t affect the original variable.


****
