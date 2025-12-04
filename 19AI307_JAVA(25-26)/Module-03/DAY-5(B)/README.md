# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Find the largest digit in a number using wrapper class methods.

## AIM:
To write a Java program to find the largest digit in a given number using Wrapper Class methods.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the number from the user.
4. Convert the number to a string using wrapper class Integer.toString().
5. Traverse each character, convert it back to an integer using Character.getNumericValue().
6. Compare digits and store the largest digit.
7. Display the largest digit.
8. Stop the program.

## PROGRAM:
 ```
Program to implement a Wrapper Class using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
```

## SOURCE CODE:
```java
import java.util.Scanner;

public class LargestDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine(); 

        int largest = 0;

        for (int i = 0; i < input.length(); i++) 
        {
            int digit = Character.getNumericValue(input.charAt(i));
            if (digit > largest) {
                largest = digit;
            }
        }

        System.out.println("The largest digit is: " + largest);
        sc.close();
    }
}
```



## OUTPUT:
<img width="792" height="306" alt="image" src="https://github.com/user-attachments/assets/b60fe0b0-ec0f-447f-b5f3-4b7d172efd32" />


## RESULT:
Thus, the program to find the largest digit in a number using Wrapper Class methods was successfully executed.
