# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class Circle that uses a constructor to calculate area using radius.



## AIM:
To write a Java program that defines a class Circle and uses a constructor to calculate the area using the given radius.

## ALGORITHM :
1.	Create a class named Circle.
2.	Declare variables radius and area.
3.	Define a parameterized constructor that accepts radius and calculates area = π × r × r.
4.	Display the area inside the constructor.
5.	In main(), create an object of Circle and pass the radius.




## PROGRAM:
 ```

Program to implement a Variable scope and Constructor using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094

```

## SOURCE CODE:

```java
import java.util.Scanner;

class Circle {
    double area;

    
    Circle(double radius) {
        area = 3.14159 * radius * radius;
        System.out.printf("Area of the circle with radius %.2f is %.2f%n", radius, area);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        if (sc.hasNextDouble()) {           
            double radius = sc.nextDouble();
            Circle c = new Circle(radius);  
        }


    }
}

```






## OUTPUT:
<img width="1244" height="269" alt="image" src="https://github.com/user-attachments/assets/d836eba6-44e0-49ca-8f26-8e7e9e3133a4" />



## RESULT:
The program successfully calculates and displays the area of a circle using a constructor.




