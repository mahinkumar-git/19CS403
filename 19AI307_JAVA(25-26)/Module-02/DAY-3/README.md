# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Person with private instance variables name, age. and country. Provide public getter and setter methods to access and modify these variables.



## AIM:
To write a Java program that defines a class Person with private variables and provides public getter and setter methods for encapsulation.

## ALGORITHM :
1. Create a class Person with private variables name, age, and country
2. Define public getter and setter methods for each variable.
3. In main(), create a Person object and set values using setters.
4. Retrieve and display values using getters.
5. End the program.





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Person {
    private String name;
    private int age;
    private String country;

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }

    public String getCountry() {
        return country;
    }
    public void setCountry(String country) {
        this.country = country;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Person p = new Person();

        String name = sc.nextLine();
        int age = sc.nextInt();
        sc.nextLine(); // consume newline
        String country = sc.nextLine();

        p.setName(name);
        p.setAge(age);
        p.setCountry(country);

        // Print heading before details
        System.out.println("Person 1");
        System.out.println("Name: " + p.getName());
        System.out.println("Age: " + p.getAge());
        System.out.println("Country: " + p.getCountry());

        sc.close();
    }
}

```






## OUTPUT:
<img width="1140" height="654" alt="image" src="https://github.com/user-attachments/assets/d9cffbf8-79b2-493c-813a-eadd64aa66c3" />



## RESULT:
The program successfully demonstrates encapsulation using getter and setter methods in Java.


